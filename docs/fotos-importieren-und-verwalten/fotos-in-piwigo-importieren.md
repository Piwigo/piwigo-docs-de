---
title: Fotos in Piwigo importieren - Piwigo-Dokumentation
description: "Dieser Artikel zeigt Ihnen, wie Sie Dateien aus verschiedenen Quellen zu Piwigo hinzufügen: aus dem Administrationsbereich, aus Ihrer Galerie, mit der mobilen App von Piwigo, mit anderer Software …"
---

# Fotos in Piwigo importieren

Es gibt viele Möglichkeiten, Dateien in Piwigo zu importieren.

!!! tip "Tipp"
    Meistens ist von Fotos die Rede. Was für Fotos gilt, gilt aber allgemein auch für alle anderen Bild-, Video- und Dokumenttypen (siehe Artikel: [Kompatible Dateiformate](kompatible-dateiformate.md)).

In diesem Artikel erfahren Sie, wie Sie Dateien hinzufügen:

- aus dem Administrationsbereich von Piwigo
- aus Ihrer Galerie (für Benutzer, die keine Administratoren sind)
- aus anderen Quellen

!!! warning "Einige Optionen, zum Beispiel der Upload per FTP, stehen nur Benutzern einer selbst gehosteten Galerie zur Verfügung."

## Fotos aus dem Administrationsbereich von Piwigo importieren

Um Fotos (oder Dateien eines anderen Typs) aus dem Administrationsbereich von Piwigo zu importieren, öffnen Sie den Administrationsbereich.

Wählen Sie im linken Menü Fotos > Hinzufügen. Sie gelangen auf die Seite „Bilder hochladen“.

![image.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-b175687b.png)

### Das Zielalbum für Ihre Fotos auswählen

Um Dateien in Piwigo zu importieren, müssen Sie zuerst ein Album auswählen. Klicken Sie dazu auf das Symbol neben „Ein Album auswählen“. Es öffnet sich ein Fenster mit allen vorhandenen Alben. Alben mit Unteralben haben links einen Pfeil. Mit einem Klick auf den Pfeil klappen Sie die Baumstruktur auf. Sie können das gewünschte Album auch über seinen Namen suchen.

![image.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-b4272d6b.png)

![image.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-cd92b583.png)

![image.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-bafc87cd.png)

Klicken Sie auf das + neben einem Album, um es auszuwählen.

Sie können auch ein neues Album erstellen, indem Sie auf „Erstellungsmodus“ klicken. Wählen Sie das übergeordnete Album in der Liste, um ein Unteralbum zu erstellen, oder klicken Sie auf „Ein Stammalbum erstellen“, um ein Album auf der obersten Ebene Ihres Piwigo-Bereichs zu erstellen. Geben Sie dem Album einen Namen, legen Sie fest, ob es am Anfang oder am Ende der Albenliste erscheinen soll, und klicken Sie auf „Erstellen und auswählen“.

![image.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-d655458a.png)

### Dateien in Piwigo importieren

Sobald das Album ausgewählt ist, haben Sie zwei Möglichkeiten, Dateien von Ihrem Computer zu importieren:

- Klicken Sie auf die Schaltfläche „Fotos hinzufügen“ und wählen Sie die gewünschten Dateien auf Ihrem Computer aus.
- Ziehen Sie die Dateien direkt aus dem Ordner auf Ihrem Computer in den grauen Bereich, wie im Beispiel unten.

![Glisser déposer.gif](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-8066d9b3.gif)

Nach und nach werden die Dateien auf dem Bildschirm angezeigt. Sie befinden sich in einer Art Warteschlange. Sie sehen ihren Namen und ihre Grösse. Wenn Sie eine der Dateien doch nicht importieren möchten, klicken Sie einfach rechts auf das Kreuz.

![Attente de transfert.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-43a211fc.jpg)

Wenn alles passt, klicken Sie auf die Schaltfläche „Upload starten“.

Während Piwigo Ihre Dateien importiert, verschwinden sie aus der Warteschlange. Nach dem Import haben Sie folgende Möglichkeiten:

- die Eigenschaften der Fotos gesammelt ändern, indem Sie auf „Dieses Set von … Fotos verwalten“ klicken
- oder weitere Dateien hinzufügen, indem Sie auf „Ein weiteres Fotoset hinzufügen“ klicken

![Importer des photos.gif](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-0f178ec0.gif)

## Duplikate beim Import erkennen

Wenn Sie Dateien in Piwigo importieren, kann Piwigo Duplikate erkennen und verhindern, dass sie importiert werden.

Wenn Sie beim Hinzufügen von Fotos eine Datei importieren, die mit einer anderen Datei in Ihrer Piwigo-Galerie identisch ist, fügt Piwigo die vorhandene Datei dem Zielalbum hinzu, legt die Datei aber kein zweites Mal an.

Sie können diese Funktion im Administrationsbereich ein- oder ausschalten, und zwar im Menü Konfiguration > Optionen, im Tab „Allgemein“ und dort im Abschnitt „Verschiedenes“.

![Détecter doublons.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-87ce4644.jpg)

## Fotos beim Import verkleinern

Um die Grösse der in Ihre Galerie importierten Dateien anzupassen, öffnen Sie den Administrationsbereich und klicken im linken Menü auf Konfiguration > Optionen. Klicken Sie dann auf den Tab „Bildgrössen“.

![Tailles de photos.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-1a2a40a9.jpg)

Standardmässig importiert Piwigo die Datei in ihrer Originalgrösse.

Wenn Sie möchten, kann Piwigo die Dateien beim Import automatisch verkleinern.

**❓ Warum Fotos beim Import verkleinern?**

Das kann sinnvoll sein, wenn Ihre Originalfotos eine sehr hohe Auflösung haben und Sie Ihre Fotos in Ihrer Fotothek nicht in optimaler Auflösung anzeigen müssen. Das hat folgende Vorteile:

- Die Dateien werden kleiner, und Sie benötigen weniger Speicherplatz.
- Der Server benötigt weniger Ressourcen.

Wir raten jedoch davon ab, Ihre Fotos zu verkleinern, wenn Piwigo der Hauptspeicherort für Ihre Dateien ist. Beim Verkleinern geht Qualität verloren. Wenn Sie eine Version Ihrer Bilder in geringerer Qualität an Piwigo senden, bewahren Sie die Originale unbedingt an einem anderen sicheren Ort auf (zum Beispiel als Sicherung auf einer Festplatte).

Um Ihre Fotos automatisch zu verkleinern, aktivieren Sie im Menü Konfiguration > Optionen, Tab „Bildgrössen“, das Kästchen „Grösse nach dem Upload anpassen“. Sie können Folgendes festlegen:

- die maximale Breite Ihrer Fotos (in Pixeln)
- die maximale Höhe Ihrer Fotos (in Pixeln)
- die Bildqualität nach dem Verkleinern (in Prozent)

![Redimensionner photo.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-7a39c4b3.jpg)

## Dateien nach dem Import bearbeiten

Wenn Sie gerade ein Set von Fotos in Piwigo importiert haben, können Sie ihre Eigenschaften direkt im Anschluss bearbeiten. Klicken Sie dazu auf „Dieses Set von … Fotos verwalten“.

![Gérer lot photos.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-5f6e10f7.jpg)

Die ausgewählten Fotos werden dadurch in Ihre Ablage gelegt. Sie gelangen dann auf die Seite „Stapelverarbeitung“, gefiltert auf die Fotos, die Sie gerade hochgeladen haben.

Sie können Änderungen an den importierten Dateien vornehmen:

- gesammelt, indem Sie im aktuellen Tab bleiben („Übersicht“)
- oder einzeln, Datei für Datei, indem Sie auf den Tab „Einzelmodus“ klicken.

![Sélection photos.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-6d37ff62.jpg)

Wie Sie die Stapelverarbeitung nutzen, [erfahren Sie in diesem Artikel](stapelverarbeitung.md).

## Fotos aus Ihrer Galerie importieren

Soll ein Benutzer Fotos zu Ihrer Piwigo-Galerie hinzufügen können, ohne Administrator zu sein? Das geht mit dem Plugin Community.

Mit diesem Plugin können Sie Benutzern ohne Administratorrechte erlauben, über eine eigene Seite in Ihrer Galerie Fotos zu Piwigo hinzuzufügen.

[Zur Dokumentation des Plugins Community](../benutzer-verwalten/mitwirkende-community-plugin.md)

## Dateien von Ihrem Mobilgerät importieren

Sie können Ihr Smartphone oder Tablet mit Piwigo verbinden, um Alben zu erstellen und Fotos und Videos zu Ihrer Galerie hinzuzufügen. Installieren Sie dazu eine der offiziellen [Mobile Apps](../mobile-apps/index.md) von Piwigo.

## Dateien aus einem Ordner auf Ihrem Computer mit Piwigo Remote Sync importieren

Sie können einen Ordner auf Ihrem Computer automatisch mit Piwigo synchronisieren und sogar eine ganze Ordnerstruktur hinzufügen.

Bei jeder Synchronisierung werden nur neue Fotos hinzugefügt.

Dazu müssen Sie die App [Piwigo Remote Sync](https://de.piwigo.org/ext/index.php?eid=851) auf Ihrem Computer installieren. Die Software läuft unter Mac, Windows und Linux.

Mehr dazu erfahren Sie in der zugehörigen Dokumentation unter dem folgenden Link:

[Dokumentation: Piwigo Remote Sync](fotos-in-piwigo-importieren/piwigo-remote-sync.md)

## Eine Ordnerstruktur von Ihrem Computer per FTP importieren und synchronisieren

Wenn Ihr Piwigo auf Ihrem eigenen Server läuft und nicht in der [Piwigo Cloud](https://de.piwigo.org/piwigo-bekommen), können Sie einen Ordner auf Ihrem Computer mit Ihrer Galerie synchronisieren.

Dazu benötigen Sie ein FTP-Programm.

Mehr dazu erfahren Sie im folgenden Artikel.

[FTP-Import und Synchronisierung](../piwigo-selbst-hosten/fotos-per-ftp-importieren-und-synchronisieren.md)

## Dateien aus Adobe Lightroom importieren

Wenn Sie die Fotoverwaltung Adobe Lightroom verwenden, können Sie ein Plugin installieren, mit dem Sie Fotos direkt in Ihre Piwigo-Galerie übertragen. Dieses Plugin wird nicht von Piwigo entwickelt. Sein Entwickler verkauft es für 15 $.

[Mehr dazu auf dieser Seite](https://alloyphoto.com/plugins/piwigo/)

## Dateien aus Digikam importieren

[Digikam](https://www.digikam.org/) ist eine kostenlose Fotoverwaltung für Linux, Windows und Mac. Sie enthält ein Plugin „Export nach Piwigo“, mit dem Sie Fotos von Digikam zu Piwigo übertragen können.

[Mehr dazu auf dieser Seite](https://docs.digikam.org/en/export_tools/piwigo_export.html)

## Dateien aus Shotwell importieren

[Shotwell](https://wiki.gnome.org/Apps/Shotwell) ist eine Open-Source-Fotoverwaltung für Linux. Unter Ubuntu und Fedora ist sie standardmässig installiert. Mit einem Plugin für Shotwell können Sie Fotos zu Piwigo exportieren.

[Den Connector auf GitHub herunterladen](https://github.com/guillaumev/piwigoshotwell)

## Dateien aus Ihrem Flickr-Konto importieren

Sie haben Fotos in einem Flickr-Konto und möchten sie zu Piwigo hochladen? Das ist möglich!

Installieren Sie dazu das Plugin Flickr2Piwigo.

!!! warning "Wenn Sie eine selbst gehostete Galerie verwenden, achten Sie darauf, die neueste Version des Plugins zu installieren."

Auf der Einstellungsseite des Plugins werden die einzelnen Schritte erklärt, um Ihre Piwigo-Galerie mit Flickr zu verbinden.

![Plugin Flickr.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-3c5ca4d4.jpg)

Melden Sie sich zuerst in Ihrem Flickr-Konto an und öffnen Sie [diese Seite](https://www.flickr.com/services/apps/create/apply/), um Ihren API-Schlüssel zu erstellen.

Wählen Sie auf der ersten Seite die Option „Apply for a non-commercial key“.

Füllen Sie auf der nächsten Seite die Felder „Name“ und „Description“ für Ihren Schlüssel aus, zum Beispiel wie unten gezeigt. Aktivieren Sie die beiden Kästchen, um den Nutzungsbedingungen zuzustimmen, und klicken Sie auf „Submit“.

![API key request.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-67d95267.jpg)

Flickr zeigt Ihnen dann zwei Zeichenketten an: „Key“ und „Secret“.

Kehren Sie zur Konfiguration des Plugins Flickr2Piwigo zurück und fügen Sie diese beiden Zeichenketten in die Felder „API-Schlüssel“ und „API-Geheimnis“ ein. Speichern Sie die Einstellungen.

Öffnen Sie in der Konfiguration des Plugins den Tab „Import“ und klicken Sie auf „Verbinden“. Sie werden auf eine Seite von Flickr weitergeleitet. Klicken Sie dort auf „OK, ich autorisiere es“.

![Page Flickr.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-03eecec1.jpg)

Fertig, Sie sind verbunden!

![Flickr fini.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-0e6397d8.jpg)

Sie haben jetzt folgende Möglichkeiten:

- Ihre Flickr-Alben auflisten und für jedes Album auswählen, welche Fotos Sie zu Piwigo hochladen möchten;
- alle Fotos aus Ihrem Flickr-Konto hochladen.

### Ihre Flickr-Alben auflisten

Wenn Sie diese Option wählen, wird die Liste der Alben in Ihrem Flickr-Konto angezeigt. Klicken Sie auf ein Album, um die Fotos auszuwählen, die zu Piwigo hochgeladen werden sollen. Sie können die zu importierenden Fotos auswählen und festlegen, in welches Album sie importiert werden. Ausserdem können Sie entscheiden, ob die beschreibenden Daten Ihrer Fotos von Flickr zu Piwigo übernommen werden sollen (Name des Fotos, Autor, Aufnahmedatum, Schlagworte …).

![Import album.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-272bf490.jpg)

### Alle Fotos aus Ihrem Flickr-Konto importieren

Wenn Sie diese Option wählen, können Sie entweder alle Ihre Flickr-Alben in Piwigo nachbilden oder alle Ihre Flickr-Fotos in ein Album Ihrer Wahl importieren. Ausserdem können Sie entscheiden, ob die beschreibenden Daten Ihrer Fotos von Flickr zu Piwigo übernommen werden sollen (Name des Fotos, Autor, Aufnahmedatum, Schlagworte …).

![Importer tout.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-5408c32d.jpg)

Und schon ist es geschafft!

Wie Sie sehen, ist es ganz einfach, Fotos aus Ihrem Flickr-Konto in Piwigo zu importieren 🙂
