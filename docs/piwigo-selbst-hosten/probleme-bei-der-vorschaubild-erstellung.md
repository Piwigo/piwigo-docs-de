---
title: Probleme bei der Erstellung von Vorschaubildern und Ersatzbildern
description: Wenn Sie Dateien zu Piwigo hochladen, läuft ein ganzer Prozess ab. Die Dateien werden auf den Server hochgeladen, aber auch in der Datenbank registriert, und einige weitere Dateien werden direkt erzeugt
---

# Probleme bei der Erstellung von Vorschaubildern und Ersatzbildern

!!! tip "Lesen Sie auch: [Fotos in Piwigo importieren](../fotos-importieren-und-verwalten/fotos-in-piwigo-importieren.md)"

Wenn Sie Dateien zu Piwigo hochladen, läuft ein ganzer Prozess ab. Die Dateien werden auf den Server hochgeladen, aber auch in der Datenbank registriert, und einige weitere Dateien werden direkt erzeugt:

- Wenn Piwigo mehrere Grössen Ihres Bildes erzeugt, entstehen mehrere Dateien, darunter die Vorschaubilder, die in Ihrer Galerie angezeigt werden;
- Für einige Dateiformate (Videos, PDF …) werden Bilder erzeugt, die in Ihrer Galerie anstelle der Quelldatei angezeigt werden: Diese nennen wir Ersatzbilder (Representatives).

Die Erstellung von Vorschaubildern und Ersatzbildern kann fehlschlagen, wenn auf Ihrem Server etwas nicht richtig konfiguriert ist. Piwigo verwendet für diese Arbeit nämlich externe Bibliotheken.

Wenn Sie Ihren Server selbst verwalten, müssen Sie dem Problem möglicherweise auf den Grund gehen, damit alles richtig funktioniert. Genau das erklären wir in diesem Artikel.

!!! warning "Achtung:"
    Dieser Artikel richtet sich nur an Webmaster einer selbst gehosteten Piwigo-Installation. Wenn Sie Kunde von [Piwigo Cloud](https://de.piwigo.org/piwigo-bekommen) sind, betrifft Sie das nicht: Die Hosting-Umgebung bei Piwigo Cloud ist optimiert.

## 1- Probleme bei der Erstellung von Vorschaubildern für Fotos

Sie haben Bilder in ein Album importiert, sehen aber keine Bilder in Ihrer Piwigo-Galerie? Das kann an einem Problem bei der Erstellung der Vorschaubilder liegen.

Um sicherzugehen, öffnen Sie im Administrationsbereich die Stapelverarbeitung und wählen Sie Ihr Album aus. Nachdem Sie den Filter angewendet haben, sollten Vorschaubilder erscheinen. Wenn Sie „XX Fotos im gegenwärtigen Set“ sehen, aber nur leere Quadrate, liegt ein Problem mit den Vorschaubildern vor.

### Prüfen, ob die URL i.php einen Fehler zurückgibt

!!! info "Info:"
    Piwigo ruft `i.php` auf, um das verkleinerte Bild in `./_data/i/` zu erzeugen, und ruft das verkleinerte Bild danach direkt aus `./_data/i/` ab. Dabei können viele Probleme auftreten: eine Überlastung des Servers, ein zu grosses Bild oder eines mit falscher Dateiendung, unzureichende Berechtigungen für Dateien/Ordner usw.

Klicken Sie in der Stapelverarbeitung mit der rechten Maustaste auf ein fehlerhaftes Bild und wählen Sie in Ihrem Browser „Bild anzeigen“ oder „Bildadresse kopieren“. Sie können auch den Quellcode der Seite anzeigen (meist mit Strg+U) und darin nach einer URL mit „i.php“ suchen (Strg+F). Rufen Sie diese URL dann in Ihrem Browser auf und notieren Sie die angezeigte Fehlermeldung.

Folgende Fehlermeldungen können auftreten:

1. „source not found“: Prüfen Sie per FTP, ob das Quellbild existiert und ob die Berechtigungen der Datei ausreichen (Chmod: 755 für Ordner, 644 für Dateien). Ist das Problem damit nicht gelöst, stellen Sie sicher, dass der PHP-Benutzer bzw. das System ausreichende Rechte auf Ihrem Server hat
2. „dir create error“: Prüfen Sie per FTP, ob die Berechtigungen der Ordner richtig gesetzt sind (Chmod: 755 für Ordner, 644 für Dateien). Ist das Problem damit nicht gelöst, stellen Sie sicher, dass der PHP-Benutzer bzw. das System ausreichende Rechte auf Ihrem Server hat
3. „Empty array while parsing Sizing“ „Sizing arr“ „Invalid chars in request“ …: Ein Erscheinungsbild oder Plugin funktioniert nicht. Schreiben Sie einen Beitrag im Forum mit einer Liste der verwendeten Plugins und Ihres Erscheinungsbilds.
4. Fehlerseite 404: Die Datei i.php fehlt. Laden Sie auf piwigo.org das ZIP-Archiv Ihrer aktuellen Piwigo-Version herunter, entpacken Sie es und laden Sie die Dateien per FTP hoch. Überschreiben Sie alle Dateien: Sie verlieren dabei keine Anpassungen und keine Bilder.
5. Fehlerseite 403: Prüfen Sie die Berechtigungen der Datei i.php (und auch der anderen Dateien). Chmod: 755 für Ordner, 644 für Dateien.
6. „500 Internal error page“ oder „PHP Fatal Error: Allowed memory size of …“: Dieser Fehler kann viele Ursachen haben. Wenn einige Bilder erzeugt werden und andere nicht, liegt es möglicherweise an einer Überlastung Ihres Servers (warten Sie einfach ein paar Stunden) oder an zu wenig Speicher für PHP (bitten Sie Ihren Hoster, die Option memory_limit zu ändern). Wenn als Grafikbibliothek GD verwendet wird, installieren Sie Imagemagick.

Keine Fehlermeldung?

1. Fügen Sie mit Localfiles Editor diese Variable zur lokalen Konfiguration hinzu: `$conf['enable_i_log'] = true;` Versuchen Sie dann, mit der Stapelverarbeitung einige Grössen zu erzeugen. Danach können Sie die Datei _data/tmp/i.log öffnen und nachsehen, ob sie eine Fehlermeldung enthält. Veröffentlichen Sie den Inhalt dieser Datei im Forum.
2. Sie können auch die Hinweise zu „500 Internal error page“ lesen und Imagemagick verwenden. Oder veröffentlichen Sie im Forum eine URL zu Ihrer Website mit öffentlich sichtbaren Bildern.

### ImageMagick installieren

GD Graphics Library und ImageMagick sind beides Open-Source-Bibliotheken zur dynamischen Erzeugung von Bildern. Wenn Ihr Server die GD Graphics Library verwendet, können (unter anderem) Probleme bei der Erstellung von Vorschaubildern auftreten. 

Deshalb empfehlen wir, zu Imagemagick zu wechseln. Imagemagick ist bei den meisten Hosting-Paketen verfügbar. Zuerst muss Imagemagick installiert werden, falls das noch nicht geschehen ist. Danach können Sie Piwigo mitteilen, wo sich die Dateien befinden.

Fügen Sie dazu mit [Localfiles Editor](lokale-konfiguration-bearbeiten-localfiles-editor.md) die folgenden Variablen hinzu. Fragen Sie zuerst Ihren Hoster nach dem Pfad zu den ImageMagick-Programmdateien.

```php
// Library used for image resizing. Value could be 'auto', 'imagick',
// 'ext_imagick' or 'gd'. If value is 'auto', library will be choosen in this
// order. If choosen library is not available, another one will be picked up.
$conf['graphics_library'] = 'ext_imagick';
// If library used is external installation of ImageMagick ('ext_imagick'),
// you can define imagemagick directory.
$conf['ext_imagick_dir'] = '/usr/local/bin/';//change with own path!
```

Um zu prüfen, welche Grafikbibliothek in Ihrer Umgebung verwendet wird, öffnen Sie im Administrationsbereich das Menü Werkzeuge > Wartung und wechseln Sie zum Reiter „Server-Umgebung“.

![ext-image-magick.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-7b656060.png)

!!! warning "Achtung:"
    Ihr Server verwendet möglicherweise nicht ImageMagick, sondern Imagick, eine PHP-Erweiterung, die ImageMagick „kapselt“, für bestimmte Dateiformate aber keine Vorschauen erzeugt. Verwenden Sie unbedingt External Image Magick.

## 2- Probleme bei der Erstellung von Vorschaubildern für Videos

Mit dem Plugin VideoJS und etwas Code in Ihrer lokalen Konfiguration können Sie Videos zu Piwigo hochladen ([wie hier erklärt](../fotos-importieren-und-verwalten/kompatible-dateiformate.md)).

Dieses Plugin benötigt jedoch die Bibliothek **ffmpeg**, um richtig zu funktionieren. Ist sie auf Ihrem Server nicht installiert, kann Piwigo den Befehl zur Erstellung der Vorschaubilder nicht ausführen.

Das kann zwei Folgen haben:

- Entweder wird das Video zu Ihrer Galerie hinzugefügt, aber es wird kein Bild erzeugt, sodass es durch ein Standardsymbol dargestellt wird;
- Oder das Video wird gar nicht zu Ihrer Galerie hinzugefügt.

Wenn Videos in Ihrem Piwigo richtig funktionieren sollen, müssen Sie also prüfen, ob **ffmpeg** installiert ist. Wenn ja, umso besser: Sie müssen Piwigo nur noch mitteilen, wo sich die Dateien befinden.

Fügen Sie dazu mit [Localfiles Editor](lokale-konfiguration-bearbeiten-localfiles-editor.md) die folgenden Variablen hinzu. Fragen Sie zuerst Ihren Hoster nach dem Pfad zu den **ffmpeg**-Programmdateien und ersetzen Sie den Pfad im Code durch den Pfad auf Ihrem eigenen Server.

```php
$conf['ffmpeg_dir'] = '../../apps/ffmpeg/';
```

Wenn Sie weitere technische Unterstützung zu diesem Thema benötigen, lesen Sie die [VideoJS-Dokumentation auf GitHub](https://github.com/Piwigo/piwigo-videojs/wiki/How-to-add-videos#step-2-install): Dort finden Sie eine ausführliche Anleitung zur Installation von **ffmpeg**.

!!! warning "Achtung:"
    Wenn ffmpeg bei Ihrem Webhoster nicht verfügbar ist, können Sie Videos mit Piwigo nicht richtig verwalten. Wir empfehlen, zu einem anderen Webhoster zu wechseln.

## 3- Probleme mit der Vorschau bestimmter Dateitypen (PDF, PSD, HEIC …)

Sie können PDF-Dateien zu Piwigo hochladen, [wie hier erklärt](../fotos-importieren-und-verwalten/kompatible-dateiformate.md).

Piwigo erzeugt ein Vorschaubild für Ihre Datei, indem es die erste Seite der Datei extrahiert und in ein Bild umwandelt.

Manchmal sehen Sie jedoch nach dem Hochladen einer PDF-Datei zu Piwigo statt des Vorschaubilds ein Symbol, wie im Beispiel unten.

![image.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-24a21bc4.png)

Auch in Ihrer Galerie wird Ihre PDF-Datei mit diesem Standardsymbol angezeigt.

![image.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-90ba4ef5.png)

In diesem Fall wurde die Datei korrekt zu Piwigo hochgeladen und kann über das Symbol „Datei herunterladen“ heruntergeladen werden. Die Vorschaubilder wurden jedoch nicht korrekt erzeugt.

Um dieses Problem zu beheben, prüfen Sie, ob die Bibliothek **External** **ImageMagick** installiert ist, und geben Sie falls nötig ihren Pfad in der lokalen Konfiguration an (wie in einem vorherigen Kapitel dieser Seite erklärt).
Dieses Problem betrifft nicht nur PDF-Dateien: Es verhindert auch die Erstellung von Vorschaubildern für PSD-, AI-, TIF-, TIFF- und HEIC-Dateien.
