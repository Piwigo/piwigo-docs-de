---
title: Piwigo auf einen anderen Server umziehen
description: Sie möchten mit Ihrem Piwigo zu einem neuen Webhoster wechseln, von Piwigo Cloud in Ihre eigene Umgebung umziehen oder Ihre Galerie in ein Unterverzeichnis verschieben? Dann sind Sie hier richtig!
---

# Piwigo auf einen anderen Server umziehen

Sie möchten mit Ihrem Piwigo zu einem neuen Webhoster wechseln, von Piwigo Cloud in Ihre eigene Umgebung umziehen oder Ihre Galerie in ein Unterverzeichnis verschieben? Dann sind Sie hier richtig!
## Piwigo auf einen neuen Server umziehen

Um Ihr Piwigo zu einem neuen Webhoster umzuziehen, führen Sie die folgenden Schritte in der richtigen Reihenfolge aus.

1. Sichern Sie Ihre Datenbank (DB)

Meistens verwenden Sie dafür den Standard-Datenbankmanager **phpMyAdmin.**

1. Sichern Sie alle Ihre Dateien per FTP

Wählen Sie in Ihrem FTP-Programm den Ordner aus, in dem Ihre Galerie installiert ist. Das Standardverzeichnis ist: ./piwigo

1. Importieren Sie Ihre DB beim neuen Webhoster

Dabei führen Sie den umgekehrten Vorgang von Punkt 1 aus, das heisst, Sie „importieren“ die zuvor erstellte Sicherung im Manager phpMyAdmin. Wenn Ihre Sicherung zu gross ist, müssen Sie den Verlauf Ihrer Galerie (beim ersten Hoster) löschen. Reicht das nicht aus, belegen möglicherweise einige Plugins viel Platz. Deinstallieren Sie diese und erstellen Sie eine Sicherung.

1. Übertragen Sie alle Dateien per FTP zum neuen Webhoster

Das ist das Gegenstück zu Punkt 2, das heisst, Sie „senden“ Ihre Dateien in den neuen Installationsordner.

1. Bearbeiten Sie den Inhalt der Datei *./local/config/database.inc.php*

Hier ein Beispiel der Datei mit Kommentaren.

```php
<?php
$conf['dblayer'] = 'mysql'; // DB-Typ
$conf['db_base'] = 'piwigo'; // Name der DB
$conf['db_user'] = 'gotcha'; // Benutzername für Ihre DB
$conf['db_password'] = 'xxxxxx'; // Passwort für Ihre DB
$conf['db_host'] = 'localhost'; // Hostname der DB 
$prefixeTable = 'piwigo_'; // Tabellenpräfix
 
define('PHPWG_INSTALLED', true);
define('PWG_CHARSET', 'utf-8');
define('DB_CHARSET', 'utf8');
define('DB_COLLATE', '');
 
?>
```

## Von Piwigo Cloud umziehen

Sie haben bereits ein Piwigo bei Piwigo Cloud und möchten es in Ihre eigene Umgebung umziehen? Folgen Sie dieser Anleitung.

- Fordern Sie in Ihrem Piwigo-Cloud-Konto auf der Seite [Administration > Mein Konto > Verwalten > Reiter Meine Daten] Ihre Daten an. Sie werden als Liste von ZIP-Dateien zu je 500 MB bereitgestellt. Sie können auch einen FTP-Zugang anfordern, wenn Sie dafür den Support von Piwigo Cloud kontaktieren.
- Entpacken Sie den Inhalt der ZIP-Dateien. In der ersten ZIP-Datei finden Sie den SQL-Dump der Datenbank und das Verzeichnis „local“. Alle ZIP-Dateien, einschliesslich der ersten, enthalten das Verzeichnis „upload“.
- Laden Sie die neueste Version von Piwigo herunter (nicht netInstall), entpacken Sie die Dateien und übertragen Sie sie auf Ihr Hosting, starten Sie aber nicht die Installation.
- Bearbeiten Sie die Datei local/config/database.inc.php so, dass sie den Zugangsdaten Ihrer Datenbank auf dem neuen Server entspricht. Beachten Sie, dass die Tabellen bei Piwigo Cloud kein Präfix haben. Setzen Sie daher `$prefixeTable = '';`
- Übertragen Sie die Verzeichnisse „local“ und „upload“ auf Ihren neuen Server
- Importieren Sie Ihren Datenbank-Dump
- Fertig! Möglicherweise müssen Sie noch einige Plugins installieren bzw. aktivieren, die Sie bei Piwigo Cloud verwendet haben, aber Ihr Piwigo weist Sie darauf hin.

## Galerie aus dem Stammverzeichnis in ein Unterverzeichnis verschieben

### Ich möchte meine Fotos nicht verschieben

!!! info "Info:"
    Im folgenden Ablauf gilt die Konvention, dass der Punkt {.} [http://www.exemple.com](http://www.exemple.com/) entspricht.
    Für Ihre Datenbank (DB) gehen wir davon aus, dass Ihr Tabellenpräfix `piwigo_` lautet.

1. Aktivieren Sie zuerst den Wartungsmodus (Administrationsbereich, Werkzeuge, Wartung, Aktion „Zugriff auf die Galerie sperren“).
2. Rufen Sie nun die Adresse ./`my_gallery`/index.php auf und prüfen Sie, ob sich die Website im Wartungsmodus befindet.
3. Kopieren Sie alle Piwigo-Verzeichnisse und -Dateien aus dem Stammverzeichnis in das Verzeichnis ./`my_gallery`/, ausser ./galleries/ und ./uploads/.
4. Nun folgt die erste Änderung an Ihrer Datenbank (DB) ⇒ Geben Sie in Ihrer DB mit phpMyAdmin im Reiter „SQL“ folgenden Code ein:

```sql
UPDATE `piwigo_sites` SET `galleries_url` = '../galleries/' WHERE `id` =1 AND  `galleries_url` = './galleries/';
UPDATE `piwigo_sites` SET `galleries_url` = '../uploads/' WHERE `id` =2 AND  `galleries_url` = './uploads/';
```

1. Melden Sie sich unter ./`my_gallery`/identification.php an und prüfen Sie, ob ./galleries/ für die Albumverwaltung korrekt funktioniert. Öffnen Sie dazu Administrationsbereich > Werkzeuge > Synchronisieren, Reiter „Seitenverwaltung“. Dort sollte ./galleries/ angezeigt werden. Falls nicht, beginnen Sie von vorn.

![image.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-30c509c5.png)

1. Benennen Sie nun (im Stammverzeichnis) ./index.php in ./index.old.php um.
2. Die Galerie kann jetzt entsperrt werden (Administrationsbereich, Werkzeuge, Wartung, Aktion „Zugriff auf die Galerie sperren“).
3. Wir platzieren nun die neue index.php im Stammverzeichnis der Website:
    1. Benennen Sie die alte index.php in index.php.old um
    2. Ihre neue Datei index.php dient als Willkommensseite, wenn man http://www.exemple.com aufruft.
4. Um den Vorgang abzuschliessen, müssen Sie anschliessend (unter anderem) die Informationen zu den Pfaden aktualisieren. Öffnen Sie Administrationsbereich > Werkzeuge > Wartung und wählen Sie:
    1. Alben-Informationen aktualisieren
    2. Fotoinformationen aktualisieren
    3. Kompilierte Vorlagen entfernen
5. Letzte Kontrolle: Stellen Sie sicher, dass die Bilder auf der Website verfügbar sind.

In einigen Tagen (nachdem Sie geprüft haben, dass alles reibungslos funktioniert) können Sie alle alten Ordner und Dateien im Stammverzeichnis löschen, ausser: `./galleries/` `./uploads/` `./my_gallery/` `./index.php`

### Ich möchte alles verschieben (einschliesslich der Fotos)

Das ist sogar noch einfacher! :-)
Verschieben Sie alle Dateien und Ordner und … das war's!
