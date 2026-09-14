---
title: Kompatible Dateiformate - Piwigo-Dokumentation
description: Welche Dateiformate sind mit Piwigo kompatibel? Bilder, Videos, PDFs … Wir erklären alles!
---

# Mit Piwigo kompatible Dateiformate

**Welche Dateiformate sind mit Piwigo kompatibel? Wir erklären alles!**

## Kunden der Piwigo Cloud und selbst gehostete Galerien: die Unterschiede

Zunächst gibt es kleine Unterschiede, je nachdem, ob Sie ein Konto in der [Piwigo Cloud](https://de.piwigo.org/piwigo-bekommen) haben oder eine selbst gehostete Galerie verwenden.

- Ich verwende eine selbst gehostete Galerie
    
    Bei einer selbst gehosteten Galerie können Sie standardmässig nur Dateien im Format jpg, jpeg und gif hochladen. Diese Einstellung lässt sich aber leicht ändern, indem Sie die lokale Konfiguration mit LocalFiles Editor bearbeiten ([mehr erfahren](../piwigo-selbst-hosten/lokale-konfiguration-bearbeiten-localfiles-editor.md)).
    
    Ausserdem müssen Sie bei einer selbst gehosteten Galerie das Plugin VideoJS installieren und aktivieren, um Multimediadateien (Video und Audio) in Ihre Galerie hochladen zu können.
    
- Mein Konto wird in der Piwigo Cloud gehostet
    
    Wenn Sie ein Konto in der Piwigo Cloud erstellt haben, ist die Verwaltung von Bild-, Video- und Audiodateien standardmässig aktiviert.
    
    Um „Premium“-Dateiformate (PDF, PSD, AI …) zu akzeptieren, benötigen Sie jedoch einen Team-, Enterprise- oder VIP-Tarif.
    

## Bilddateien

Mit Piwigo können Sie Bilddateien hochladen, die sich in einem Webbrowser öffnen lassen. Piwigo akzeptiert die folgenden Dateiendungen für Bilder:

- .jpg
- .jpeg
- .png
- .gif
- .webp
- .heic

Piwigo erkennt alle diese Formate und erstellt für die Bilder ein Vorschaubild, das sowohl im Administrationsbereich von Piwigo als auch in Ihrer Galerie sichtbar ist.

### Mehr zum Format .gif

Mit Piwigo können Sie auch animierte GIFs (Dateiendung .gif) importieren. Wenn die Originaldatei grösser ist als die Grösse der Vorschaubilder in Ihrer Galerie (standardmässig 144x144), zeigt die Galerie nur eine Vorschau der GIF-Datei an, die aus dem ersten Bild der Animation erstellt wird. Um die Animation „abzuspielen“, müssen Sie das Original anzeigen.

### Mehr zum Format .webp

Seit Version 14 von Piwigo können Sie auch Bilddateien im Format webp importieren.

Bei einer selbst gehosteten Galerie können Sie das Format über das Plugin [LocalFiles Editor](../piwigo-selbst-hosten/lokale-konfiguration-bearbeiten-localfiles-editor.md) hinzufügen, indem Sie `webp` in der Einstellung `$conf['picture_ext']` ergänzen, wie im Beispiel unten.

```php
$conf['picture_ext'] = array('jpg','jpeg','png','gif','webp');
```

!!! tip "Tipp"
    WebP ist das Format, das von Webbrowsern am breitesten als Ersatz für JPEG „akzeptiert“ wird. WebP wird sowohl beim Import als auch bei der Anzeige unterstützt, und Piwigo erstellt für jede in Ihrer Galerie angezeigte Grösse eine webp-Datei. WebP kann JPEG bei ähnlicher Dateigrösse mit besserer Qualität ersetzen, animierte GIFs bei einem Bruchteil der Grösse ersetzen und sogar PNGs ersetzen, mit einer Komprimierung, die weder das Bild noch die Transparenz beeinträchtigt.

!!! warning "Um animierte WebP-Dateien zu akzeptieren, müssen Sie bei einer selbst gehosteten Galerie eventuell das Betriebssystem Ihres Servers aktualisieren"

### Sonderfall HEIC-Format

HEIC ist ein Bildformat, das Piwigo seit Version 14 akzeptiert. Es ist das Standardformat unter iOS und auf einigen Android-Smartphones.

HEIC-Dateien können nicht in einem Webbrowser angezeigt werden. Deshalb erstellt Piwigo eine Vorschau der Datei.

Um die Unterstützung von HEIC-Dateien in einer selbst gehosteten Galerie zu aktivieren, müssen Sie das Format über das Plugin [LocalFiles Editor](../piwigo-selbst-hosten/lokale-konfiguration-bearbeiten-localfiles-editor.md) hinzufügen.

Falls noch nicht geschehen, aktivieren Sie zuerst die Einstellung `upload_form_all_types`, wie unten gezeigt.

```php
$conf['upload_form_all_types'] = true;
```

Fügen Sie dann `heic` in der Einstellung `$conf['file']` hinzu, wie im Beispiel unten.

```php
$conf['file_ext'] = array_merge(
  $conf['picture_ext'],
  array('jpg','jpeg','png','gif','heic')
  );
```

!!! warning "Um HEIC-Dateien zu akzeptieren, müssen Sie bei einer selbst gehosteten Galerie eventuell das Betriebssystem Ihres Servers aktualisieren"

## Video- und Audiodateien

Mit Piwigo können Sie Video- und Audiodateien mit den folgenden Dateiendungen importieren:

- .mp4
- .m4v
- .webm
- .webmv
- .ogg
- .ogv
- .mp3

!!! info "Info:"
    Bei einer selbst gehosteten Galerie müssen Sie das Plugin VideoJS installieren und aktivieren, um diesen Dateityp anzuzeigen. Wenn Sie Kunde eines Tarifs der Piwigo Cloud sind, ist dieses Plugin standardmässig aktiviert.

Wenn Sie eine Datei in Piwigo hochladen, wird aus dem ersten Bild Ihres Videos ein Vorschaubild erstellt. Das Video kann in Ihrer Galerie mit dem integrierten Videoplayer von Piwigo angesehen werden. Sie starten das Video mit der grossen „Play“-Schaltfläche.

![](https://s3.amazonaws.com/helpscout.net/docs/assets/61e7cec9c1b8c85d97faea30/images/62d9457979bb3605c3949821/file-JX0mTPdLyh.png)

Wenn Sie eine Audiodatei in Piwigo importieren, wird sie in Ihrer Galerie mit dem folgenden Symbol dargestellt. Sie können die Audiodatei in Ihrer Galerie mit dem integrierten Player von Piwigo anhören.

![](https://s3.amazonaws.com/helpscout.net/docs/assets/61e7cec9c1b8c85d97faea30/images/62d6e0c3c74a080359c8b31a/file-aSH00yRAHB.png)

Bei einer selbst gehosteten Galerie müssen Sie, um die Unterstützung von Videos zu aktivieren, zuerst die Einstellung `upload_form_all_types` über das Plugin [LocalFiles Editor](../piwigo-selbst-hosten/lokale-konfiguration-bearbeiten-localfiles-editor.md) aktivieren, wie unten gezeigt (falls noch nicht geschehen).

```php
$conf['upload_form_all_types'] = true;
```

Fügen Sie dann die gewünschten Dateiendungen in der Einstellung `$conf['file_ext']` hinzu, wie im Beispiel unten.

```php
$conf['file_ext'] = array_merge(
  $conf['picture_ext'],
  array('mp4','webmv','m4v','webm')
  );
```

!!! info "Info:"
    Wenn Sie eine selbst gehostete Galerie verwenden und Probleme beim Hochladen von Videos oder beim Erstellen der Vorschaubilder haben, [lesen Sie diesen Artikel](../piwigo-selbst-hosten/probleme-bei-der-vorschaubild-erstellung.md).

### 🎦 Sonderfall MOV-Videos

Wenn Sie Videos mit einem iPhone, einem iPad oder mit der Apple-Software QuickTime aufnehmen, haben die erzeugten Dateien die Endung .mov. Dieses Dateiformat ist nicht mit Piwigo kompatibel, da es in Webbrowsern nicht richtig angezeigt wird.

Es gibt aber mehrere Möglichkeiten, solche Videos trotzdem zu Piwigo zu übertragen.

**Mit der mobilen App von Piwigo für iOS**

Mit der [mobilen App von Piwigo für iOS](../mobile-apps/piwigo-ios-app.md) können Sie MOV-Videos an Piwigo senden. Die Videos werden bei der Übertragung in .mp4-Dateien umgewandelt. Danach können sie wie jedes andere Video in Ihrer Galerie angesehen werden.

**Über den Administrationsbereich von Piwigo (selbst gehostete Galerien)**

Sie können MOV-Videos auch über den Administrationsbereich von Piwigo hochladen. Standardmässig lassen sich die Videos dann aber nicht mit dem Videoplayer Ihrer Galerie abspielen: Sie müssen sie herunterladen, um sie anzusehen.

Damit Ihr Piwigo .mov-Dateien importieren kann, müssen Sie den Parameter `$conf['file_ext']` ändern und das Format mov hinzufügen, wie im Beispiel unten mit [LocalFiles Editor](../piwigo-selbst-hosten/lokale-konfiguration-bearbeiten-localfiles-editor.md).

```php
$conf['file_ext'] = array_merge(
  $conf['picture_ext'],
  array('mp4','webmv','m4v','webm','mov')
  );
```

Sie können Ihre .mov-Dateien auch vor dem Import in Piwigo in das MP4-Format umwandeln. Das hat zwei Vorteile:

- Die Videos lassen sich in Ihrer Piwigo-Galerie abspielen;
- Die Dateigrösse sinkt deutlich.

Wie Sie eine Datei umwandeln, erfahren Sie im nächsten Kapitel.

**Über den Administrationsbereich von Piwigo (nur für Kunden der Piwigo Cloud)**

Wenn Sie Kunde der Piwigo Cloud sind, können Sie beim Support die automatische Umwandlung von .mov- in .mp4-Dateien einrichten lassen.

Wenn wir diese Option aktivieren, werden .mov-Dateien, die Sie über den Administrationsbereich in Piwigo importieren, automatisch in .mp4 umgewandelt. Beim Herunterladen wählt der Benutzer, ob er die .mov- oder die .mp4-Version herunterladen möchte.

!!! warning "Achtung:"
    Wenn Sie diese Option aktivieren, belegt sie mehr Speicherplatz, da jedes Video in zwei Versionen gespeichert wird und .mov-Dateien sehr gross sind.

Sie können Ihre .mov-Dateien auch vor dem Import in Piwigo in das MP4-Format umwandeln. Das hat zwei Vorteile:

- Die Videos lassen sich in Ihrer Piwigo-Galerie abspielen;
- Die Dateigrösse sinkt deutlich.

Wie Sie eine Datei umwandeln, erfahren Sie im nächsten Kapitel.

### 🎦 Ihre Videodateien umwandeln

Wenn Sie eine Videodatei importieren möchten, die Piwigo nicht akzeptiert (zum Beispiel eine AVI-Datei), wandeln Sie Ihre Videodateien einfach in das MP4-Format um. Das geht mit vielen Videobearbeitungsprogrammen oder mit kostenlosen Online-Tools [wie diesem hier](https://video.online-convert.com/convert-to-mp4).

!!! tip "Tipp"
    Wir empfehlen das Dateiformat MP4 mit dem Videocodec H.264 und dem Audiocodec AAC. So bleibt die Qualität auch bei komprimierten Videos hoch. So kodierte MP4-Dateien sind kleiner: Sie belegen weniger Speicherplatz und sparen Bandbreite. Ausserdem ist so die Kompatibilität mit Videoplayern sichergestellt.

### ⚙️ Konfiguration des Plugins VideoJS

Wie wir gesehen haben, können Sie mit dem Plugin VideoJS Videodateien in Piwigo verwalten. Das Plugin verwendet den Open-Source-Videoplayer VideoJS.

In den Einstellungen des Plugins VideoJS stehen Ihnen verschiedene Optionen zur Verfügung:

- die Anzahl der Videos in Ihrer Galerie anzeigen
- das Verhalten des Videoplayers festlegen (Video vorab laden oder nicht, automatische Wiedergabe, Wiedergabe in Schleife, Play-/Pause-Schaltflächen anzeigen oder nicht, Lautstärke, Sprache des Players)
- das Aussehen des Videoplayers anpassen, indem Sie einen der verfügbaren Stile wählen oder eigenen CSS-Code hinzufügen
- die maximale Höhe der Videos festlegen
- usw.

Eine ausführliche Dokumentation zum Plugin VideoJS finden Sie [auf seiner GitHub-Seite](https://github.com/Piwigo/piwigo-videojs/wiki).

## ⭐️ Weitere Dateiformate

Diese Dateiformate stehen nur Kunden mit einem Team-, Enterprise- oder VIP-Tarif in der Piwigo Cloud zur Verfügung sowie Benutzern, die Piwigo selbst hosten.

- PDF-Dateien
- SVG-Dateien
- EPS-Dateien
- TIF- und TIFF-Dateien
- PSD-Dateien (von Adobe Photoshop erzeugt)
- AI-Dateien (von Adobe Illustrator erzeugt)

Piwigo erstellt für diese Dateitypen eine Vorschau, sodass sie im Administrationsbereich und in Ihrer Galerie angezeigt werden können.

Um die Unterstützung dieser Dateien in einer selbst gehosteten Galerie zu aktivieren, müssen Sie zuerst die Einstellung `upload_form_all_types` über das Plugin [LocalFiles Editor](../piwigo-selbst-hosten/lokale-konfiguration-bearbeiten-localfiles-editor.md) aktivieren, wie unten gezeigt (falls noch nicht geschehen).

```php
$conf['upload_form_all_types'] = true;
```

Fügen Sie dann die gewünschten Dateiendungen in der Einstellung `$conf['file_ext']` hinzu, wie im Beispiel unten.

```php
$conf['file_ext'] = array_merge(
  $conf['picture_ext'],
  array('pdf','ai','psd','eps')
  );
```

!!! info
    Wenn Sie eine selbst gehostete Galerie verwenden und Probleme beim Erstellen der Vorschaubilder für PDF-Dateien oder bei der Anzeige von AI-, PSD-, HEIC-, TIF- oder TIFF-Dateien haben, [lesen Sie diesen Artikel](../piwigo-selbst-hosten/probleme-bei-der-vorschaubild-erstellung.md).

### Sonderfall PDF-Dateien in Piwigo

Bei PDF-Dateien erstellt Piwigo eine Vorschau, indem es die erste Seite extrahiert und in ein Bild umwandelt. Dieses Bild wird auf der Albumseite angezeigt.

Seit Piwigo 15 enthält die Dateiseite einen PDF-Reader, mit dem Sie die Datei lesen können.

![image.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-7f81236f.png)

Sie können auch auf das Symbol „Datei herunterladen“ klicken: Das Dokument wird dann auf Ihren Computer heruntergeladen.

## 📄 Weitere Dokumentformate

Wenn Sie andere Dateiformate (Excel, Word, Open Office …) hochladen möchten, können Sie das als Kunde der Piwigo Cloud beim Support beantragen. Bei einer selbst gehosteten Galerie ändern Sie dazu Ihre Konfigurationsdatei.

Diese Dateien lassen sich nicht direkt in Piwigo lesen. Sie können sie aber herunterladen und dann im passenden Programm öffnen.

Da Piwigo keine Vorschau des Dokuments erstellen kann, zeigt es stattdessen ein allgemeines Symbol an.

![Ohne Titel](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-5a7b8379.png)

Mit dem Plugin **Photo Update** können Sie auch eine eigene Vorschau hinzufügen.

![Ohne Titel](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-adb35d74.png)

## Mehrere Formate: mehrere Formate für ein einzelnes Bild anbieten

Wenn Sie in Ihrer Galerie verschiedene Dateiformate für ein einzelnes Bild anbieten möchten (zum Beispiel ein JPG-, ein PNG- und ein PSD-Format), ist das möglich! Dazu müssen Sie die Option für mehrere Formate aktivieren.

[Mehr über mehrere Formate erfahren](mehrere-formate.md)

!!! info "Wenn Sie Kunde eines Tarifs der Piwigo Cloud sind, ist diese Funktion erst ab dem Enterprise-Tarif verfügbar"

## Embedded Videos: Dateien von anderen Plattformen (YouTube …) in Ihre Galerie einbinden

Möchten Sie in Ihrer Galerie Inhalte anzeigen, die bereits anderswo gehostet werden, zum Beispiel Videos von Ihrem YouTube-Kanal?

Das ist mit dem Plugin **Embedded Videos** möglich.

Mit diesem Plugin können Sie Videos von externen Plattformen wie YouTube, Vimeo oder Dailymotion in Alben Ihrer Wahl anzeigen.

Sobald das Plugin aktiviert ist, öffnen Sie seine Einstellungen, um externe Inhalte zu Ihrer Galerie hinzuzufügen.

Dort wählen Sie aus, zu welchem Album Sie ein Video hinzufügen möchten.

Standardmässig können Sie auf dieser Seite ein Video von den Plattformen YouTube, Dailymotion, Vimeo, Wat und Wideo hinzufügen, indem Sie einfach die URL des Videos eingeben.

![Plugin Embedded Videos.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-945faa03.jpg)

Sie können auswählen, in welchem Album das Video sichtbar sein soll, und weitere Einstellungen vornehmen (Grösse des Videos, Übernahme von Beschreibung und Schlagworten usw.).

Im Tab „Add video from embed code“ können Sie einen Einbettungscode direkt von einer anderen Plattform hinzufügen. Für die Plattformen YouTube, Dailymotion, Vimeo, Wat und Wideo dürfen Sie diesen Tab nicht verwenden.

Im Tab „Configuration“ legen Sie einige globale Einstellungen des Plugins fest:

- Standardgrösse der Videos
- automatische Wiedergabe aktivieren oder deaktivieren
- Beschreibung und Schlagworte des Videos automatisch übernehmen
- Einstellungen des Players (für Vimeo und Dailymotion)

![Plugin Embedded Videos Config.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-b8923ebe.jpg)

### Bekanntes Problem mit dem Plugin Embedded Videos

Wenn Sie eine selbst gehostete Galerie verwenden und bei der Nutzung dieses Plugins eine Fehlermeldung erhalten, fügen Sie über das Plugin LocalFiles Editor den folgenden Code in Ihre Konfigurationsdatei ein.

```php
$conf['show_php_errors'] = E_ALL ^ E_DEPRECATED ^ E_WARNING;
```

## Panorama: Panoramabilder verwalten

Panoramen sind gewöhnliche Fotos, die im Verhältnis zu ihrer Höhe jedoch sehr breit sind. Solche Fotos werden oft mit einem Gerät im „Panorama“-Modus aufgenommen.

Piwigo verarbeitet diese Fotos problemlos, bringt ihr besonderes Format aber nicht unbedingt zur Geltung.

![Ein Panoramafoto](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-e16b57d6.jpg)

Ein Panoramafoto

Wenn die Besucher Ihrer Galerie sich innerhalb eines Panoramafotos bewegen können sollen, verwenden Sie das Plugin **Panoramas**.

Sobald das Plugin aktiviert ist, zeigt es die von Ihnen ausgewählten Fotos in einem anderen Anzeigemodus an, wie Sie unten sehen.

![panorama.gif](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-72f8f3da.gif)

Die Einstellungen des Plugins bieten Ihnen viele Anpassungsmöglichkeiten.

![Plugin Panoramas Config.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-fbd0ede0.jpg)

Um zu erkennen, welche Fotos im Panorama-Modus (180 oder 360°) angezeigt werden sollen, richtet sich Piwigo nach ihrem Namen.

Standardmässig muss der Name der Fotos _180 oder _360 enthalten, damit sie im Panorama-Modus angezeigt werden. Das lässt sich aber anpassen.
