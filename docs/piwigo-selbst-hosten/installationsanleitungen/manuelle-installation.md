# Manuelle Installation

!!! abstract "Voraussetzungen für die manuelle Installation"
    Diese Anleitung behandelt nur die Installation von Piwigo. Die benötigten Abhängigkeiten finden Sie in der Anleitung [Voraussetzungen](voraussetzungen.md) 

## Schritt 1 - Vollständiges Archiv herunterladen

[Laden Sie das vollständige Archiv herunter](https://de.piwigo.org/piwigo-bekommen) und entpacken Sie es.

## Schritt 2 - Inhalt des Archivs hochladen

Übertragen Sie den Inhalt des Archivs mit einem beliebigen FTP-Programm auf Ihren Webserver.

!!! info
    Das Piwigo-Team empfiehlt FileZilla als FTP-Programm, da es wie Piwigo kostenlos und mit Windows und Linux kompatibel ist.

Starten Sie FileZilla und tragen Sie die folgenden Verbindungsdaten ein, die Sie von Ihrem Webhoster erhalten haben:

- Server
- Benutzername
- Passwort

Klicken Sie auf die Schaltfläche „Verbinden“. Sie sind nun mit Ihrem Webserver verbunden.

![](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8//2026/06/26/20260626155500-5ba173ff.webp)

1.  Erstellen Sie auf Ihrem Webserver ein Verzeichnis `photos`.
2.  Öffnen Sie auf Ihrer Festplatte das entpackte Verzeichnis `piwigo`.
3.  Wählen Sie alle Dateien aus und übertragen Sie sie auf Ihrem Server in das Verzeichnis `photos`.

## Schritt 3 - Konfiguration

!!! info
    Sie können Piwigo auch im Stammverzeichnis der Website installieren, das Verzeichnis `piwigo` ist nicht zwingend. Unabhängig vom gewählten Verzeichnisnamen wird empfohlen, die Versionsnummer von Piwigo nicht sichtbar zu machen.

Sobald alle Dateien übertragen sind, rufen Sie die Webadresse in einem Webbrowser auf, zum Beispiel `http://example.com/photos`. Piwigo erkennt, dass noch nichts installiert ist, und leitet Sie zur Installationsseite weiter.

<figure markdown="span">
    ![](https://ressources.piwigo.com/i?/uploads/c/v/7/cv7jpz6hf8//2026/06/26/20260626155501-48828109-me.webp)
    <figcaption>Installationsseite</figcaption>
</figure>

Nun folgen die Einstellungen der MySQL-Datenbank und das Webmaster-Konto zur Verwaltung Ihrer Galerie.

Tragen Sie die Verbindungsdaten der MySQL-Datenbank ein, die Sie von Ihrem Webhoster erhalten haben:

- MySQL-Host 
- Benutzer (Achtung: Ihr Webhoster stellt möglicherweise getrennte Zugangsdaten für FTP und MySQL bereit.)
- Passwort
- Name der Datenbank
- Präfix der Datenbanktabellen

!!! note ""
    Meist erlauben Webhoster nur eine Datenbank pro Kunde, Sie können darin aber beliebig viele Tabellen anlegen.  
    Um Konflikte mit anderen Webanwendungen zu vermeiden oder mehrere Piwigo-Installationen auf derselben Website zu ermöglichen, erhalten die Tabellennamen ein Präfix. Standardmässig lautet dieses Präfix `piwigo_`, Sie können es aber ändern (nur alphanumerische Zeichen sind erlaubt).

Für das Webmaster-Konto sind folgende Angaben erforderlich:

- Ein Benutzername, den Sie selbst wählen
- Ein Passwort, das Sie zur Kontrolle zweimal eingeben
- Ihre E-Mail-Adresse, damit Besucher Sie kontaktieren können

Klicken Sie auf „Start der Installation“.  
Sie werden informiert, ob die Installation erfolgreich war oder fehlgeschlagen ist.

<figure markdown="span">
    ![](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8//2026/06/26/20260626155501-7b2c5f28.webp)
    <figcaption>Erfolgreiche Installation</figcaption>
</figure>

## Schritt 4 - Erste Anmeldung

Nach Abschluss der Installation können Sie Ihre Galerie aufrufen. Melden Sie sich mit Ihrem Webmaster-Konto an, dann gelangen Sie in den Administrationsbereich.

<figure markdown="span">
    ![](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8//2026/06/26/20260626155501-7cf8f4d0.webp)
    <figcaption>Piwigo ist installiert</figcaption>
</figure>
