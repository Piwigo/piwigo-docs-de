---
title: FTP-Import und Synchronisierung - Piwigo-Dokumentation
description: Wenn Sie Piwigo auf Ihrem eigenen Server (oder einem von Ihrer Organisation verwalteten Server) installiert haben, können Sie Verzeichnisse von Ihrem Computer per FTP in Ihr Piwigo übertragen.
---

# FTP-Import und Synchronisierung

!!! info "Lesen Sie auch: [Fotos in Piwigo importieren](../fotos-importieren-und-verwalten/fotos-in-piwigo-importieren.md)"

## Einführung

Wenn Sie eine Piwigo-Galerie verwenden, die auf Ihrem eigenen Server (oder einem von Ihrer Organisation verwalteten Server) installiert ist, können Sie Verzeichnisse von Ihrem Computer per FTP in Ihre Piwigo-Galerie übertragen.

Diese Methode ist die älteste und am aufwendigsten einzurichten. Sie richtet sich an fortgeschrittene Benutzer mit einem eingespielten Arbeitsablauf.

Wenn Sie eine grosse Fotosammlung haben, ist diese Methode zum Hochladen möglicherweise genau das Richtige für Sie.

Es gibt auch andere Methoden, um Ihre Fotos hochzuladen: Mehr dazu erfahren Sie im Abschnitt [Fotos in Piwigo importieren](../fotos-importieren-und-verwalten/fotos-in-piwigo-importieren.md).

!!! warning "Achtung:"
    Diese Methode steht nur für selbst gehostete Piwigo-Galerien zur Verfügung. Für Kunden mit einem Piwigo-Cloud-Abonnement ist sie daher nicht verfügbar.

## Vor- und Nachteile dieser Methode

| Vorteile | Nachteile |
| --- | --- |
| ✅ Ideal für grosse Galerien | ⚠️ Sie müssen wissen, wie man Fotos vor der Veröffentlichung vorbereitet |
| ✅ Geeignet zum Hochladen anderer Dateien als Fotos | ⚠️ Kein Spielraum zum Umbenennen / Verschieben Ihrer Fotos und Alben |
| ✅ Freie Gestaltung der Verzeichnisse auf Ihrem Server | ⚠️ Ein FTP-Programm ist nötig |
|  | ⚠️ Piwigo muss mit Ihren Dateien synchronisiert werden |

## Ein erstes Album übertragen

1. Erstellen Sie ein Verzeichnis auf Ihrem Computer.
2. Legen Sie Fotos in dieses Verzeichnis.
    
!!! warning "Achtung:"
    Die Namen der Verzeichnisse und Dateien dürfen nur Buchstaben, Ziffern und die Zeichen "-", "_" oder "." enthalten. Keine Leerzeichen und keine Zeichen mit Akzenten.

3. Kopieren Sie das Verzeichnis mit einem FTP-Programm in das Verzeichnis `./galleries/` Ihrer Piwigo-Installation.
4. Melden Sie sich in Ihrer Piwigo-Galerie an und öffnen Sie im Administrationsbereich das Menü Werkzeuge > Synchronisieren. Wählen Sie die Optionen „Verzeichnisse und Dateien“ und „Synchronisieren von Metadaten“ und aktivieren Sie „Nur Simulation durchführen“ nicht.

Herzlichen Glückwunsch! In Ihrer Galerie wurde ein Album erstellt.

## Synchronisierung verstehen

Es reicht nicht, Dateien mit Ihrem FTP-Programm auf den Server zu kopieren, damit Ihre Fotos für alle sichtbar sind. Piwigo muss die vorgenommenen Änderungen *durchgehen*. Sie haben gerade Fotos hinzugefügt und müssen Ihrer Galerie nun mitteilen, dass sie diese anzeigen soll: Genau dafür gibt es die **Synchronisierung**.

Jedes Mal, wenn Sie Dateien per FTP in Piwigo übertragen möchten, erstellen Sie also ein Unterverzeichnis von `./galleries/` und legen Ihre Elemente dort ab (in einer für das Web geeigneten Grösse). 

Optional legen Sie Vorschaubilder in einem Unterverzeichnis des soeben erstellten Verzeichnisses ab. 

Anschliessend müssen Sie im Administrationsbereich die Datenbank ***synchronisieren***, damit sie Ihre neuen Elemente erkennt.

## Aufbau der Verzeichnisse und Dateien

Die Verzeichnisse, die Alben darstellen, befinden sich im Verzeichnis `./galleries/` Ihrer Piwigo-Installation.

Unten sehen Sie die Verzeichnisstruktur einer sehr kleinen Galerie.

```
galleries
|-- wedding
|   |-- ceremony
|   |   |-- entrance
|   |   |   |-- paul-arriving.jpg
|   |   |   +-- jane-arriving.jpg
|   |   +-- exit
|   |       |-- flower-children-exit.jpg
|   |       +-- paul-and-jane-exit.jpg
|   +-- cocktail
|       |-- speech001.jpg
|       |-- speech002.jpg
|       +-- speech003.jpg
+-- honeymoon
|   |-- hotel.png
|   |-- plane-takeoff-video.avi
|   +-- pwg_representative
|       +-- plane-takeoff-video.jpg
+-- photographer-session
    |-- img0001.jpg
    |-- img0002.jpg
    +-- pwg_format
        |-- img0001.cr2
        |-- img0001.cmyk.jpg
        |-- img0001.zip
        |-- img0002.cr2
        +-- img0002.cmyk.jpg
```

Einige Erklärungen zum besseren Verständnis dieses Schemas:

- Mit Ausnahme von „pwg_representative“ und „pwg_format“ erzeugt jedes Verzeichnis in `./galleries/` ein Album. Die Anzahl Ebenen (Tiefe) ist nicht begrenzt.
- Grundsätzlich wird ein Foto durch eine Datei dargestellt. Für Piwigo kann eine Datei ein Foto sein, wenn ihre Dateiendung in der Liste der Konfigurationseinstellung `file_ext` steht (siehe Datei include/config.inc.php). Eine Datei kann ein Foto sein, wenn ihre Dateiendung in der Liste der Konfigurationseinstellung `picture_ext` steht.
- Standardmässig werden Elemente, die keine Fotos sind (Töne, Textdateien, was immer Sie möchten …), durch ein Symbol dargestellt, das der Endung des Dateinamens entspricht. Optional kann ein Ersatzbild zugeordnet werden (siehe die Datei plane-takeoff-video.avi im Beispiel).
- Mehrere Formate: Sie können ein Foto in mehreren Formaten anbieten. In diesem Beispiel gibt es für img0001.jpg drei zusätzliche Formate. Sie aktivieren diese Funktion, indem Sie `$conf['enable_formats'] = true;` zu Ihrer lokalen Konfiguration hinzufügen und eine Liste von Formaten festlegen, zum Beispiel `$conf['format_ext'] = array('cmyk.jpg', 'cr2', 'zip');`. [Mehr über mehrere Formate erfahren](../fotos-importieren-und-verwalten/mehrere-formate.md)

!!! warning "Achtung:"
    Die Namen der Verzeichnisse und Dateien dürfen nur Buchstaben, Ziffern und die Zeichen "-", "_" oder "." enthalten. Keine Leerzeichen und keine Zeichen mit Akzenten.

!!! tip "Tipp:"
    Ein Album kann sowohl Fotos als auch Unteralben enthalten. Wir empfehlen jedoch dringend, sich für jedes Album zu entscheiden, ob es Fotos **oder** Unteralben enthält.

- Sobald die Dateien richtig in den Verzeichnissen abgelegt sind, öffnen Sie im Administrationsbereich die Seite Werkzeuge > Synchronisieren.

## Dateien synchronisieren

Sobald Sie Ihre Dateien per FTP übertragen, ist die Synchronisierung jedes Mal notwendig, wenn Sie bei Ihren Fotos *ein beliebiges Element* *hinzufügen* / *umbenennen* / *verschieben* / *löschen*.

!!! warning "Wenn Sie Ihre Dateien auf andere Weise übertragen, brauchen Sie diese Funktion nicht."

Öffnen Sie im Administrationsbereich Werkzeuge > Synchronisieren.

Sie gelangen dann zum unten abgebildeten Bildschirm.

![image.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-28b01f5b.png)

Auf dieser Seite wählen Sie die Einstellungen der Synchronisierung und starten sie.

Folgende Optionen stehen zur Verfügung:

### Dateistruktur mit Datenbank synchronisieren

Damit sagen Sie Piwigo: „Hallo, es gibt neue Dateien, es ist Zeit, sie anzusehen und zu berücksichtigen.“

Drei Optionen stehen zur Verfügung:

- Nichts: In diesem Fall wird nichts synchronisiert. Diese Option wählen Sie, wenn Sie nur die Metadaten synchronisieren möchten.
- Nur Verzeichnisse: Mit dieser Option werden nur die Verzeichnisse synchronisiert. Das ist nützlich, wenn Sie nicht Ihre ganze Galerie synchronisieren müssen.
- Verzeichnisse und Dateien: Mit dieser Option synchronisieren Sie nicht nur die Verzeichnisse, sondern auch die Elemente, die sie enthalten. Wenn Sie diese Option wählen, erscheinen weitere Optionen.
    
    ![Option de synchronisation.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-62d9274c.jpg)
    
    „Alle Informationen anzeigen“ liefert Ihnen Statistiken zu den Ergebnissen der Synchronisierung.
    
    „Neue Fotos zum Sammelkorb hinzufügen“ legt alle hinzugefügten Fotos in den Sammelkorb (um sie danach zum Beispiel mit der [Stapelverarbeitung](../fotos-importieren-und-verwalten/stapelverarbeitung.md) zu bearbeiten).
    
    Mit „Wer soll diese Fotos sehen können?“ legen Sie die [Datenschutzstufe](../benutzer-verwalten/datenschutzstufen.md) der hinzugefügten Fotos fest.
    

### Datei-Metadaten mit den Fotoinformationen der Datenbank synchronisieren

Dieser Bereich bietet eine Option mit zwei Unteroptionen:

- Synchronisieren von Metadaten (Dateigrösse, Breite, Höhe): Hier legen Sie fest, ob die Metadaten der Dateien synchronisiert werden sollen.
    - Bereits synchronisierte Fotos miteinbeziehen: Wenn Sie diese Option wählen, werden auch die Elemente aktualisiert, die sich bereits in Ihrer Galerie befinden. Das ist nützlich, wenn Sie die Metadaten Ihrer Fotos geändert haben.
    - Alle in der Datenbank vorhandenen Werte zurücksetzen: Wenn Sie diese Option wählen, werden die alten Werte durch die neuen ersetzt, auch wenn diese leer sind.

### Simulation

Piwigo ermöglicht es Ihnen, Änderungen nicht sofort vorzunehmen, damit Sie sich vergewissern können, dass die Synchronisierung reibungslos abläuft.

Wie der Name schon sagt, simuliert diese Funktion also das Ergebnis der Synchronisierung.

!!! warning "Wenn Sie Ihre Dateien wirklich synchronisieren möchten, achten Sie darauf, dass dieses Kästchen nicht angekreuzt ist!"

### Auf einzelne bestehende Alben reduzieren

In diesem Bereich können Sie Ihre Alben und Unteralben durchsuchen, damit Piwigo die zu synchronisierenden Elemente findet. Eine ganze Galerie zu synchronisieren, wenn man das richtige Verzeichnis kennt, ist unnötig (und manchmal sogar gefährlich).

Die kleine Option „*Suche in Unteralben*“ verhindert, dass Sie die Suche nach dem zu synchronisierenden Ordner zu stark einschränken müssen. Mit etwas Erfahrung wissen Sie, wie Sie sie sinnvoll einsetzen.

## Häufige Fehler

Bei einem Problem informiert Sie Piwigo über die aufgetretenen Fehler.

Sehen wir uns diese Fehler gemeinsam an.

- **PWG-UPDATE-1**: Die Namen der Verzeichnisse und Dateien dürfen *nur* aus Buchstaben, Ziffern sowie "-", "_" und "." bestehen. Also keine *ausgefallenen* Zeichen und keine Zeichen mit Akzenten.
- **PWG-ERROR-NO-FS**: Auf die Datei oder das Verzeichnis kann nicht zugegriffen werden (entweder existiert sie bzw. es nicht oder der Zugriff wurde verweigert).
- **PWG-ERROR-VERSION**: Die Version von `create_listing_file.php` auf der entfernten Website und in Piwigo muss gleich sein.
- **PWG-ERROR-NOLISTING**: Die Datei listing.xml wurde auf der entfernten Website nicht gefunden. Diese Datei wird mit dem Befehl „Liste erzeugen“ in der Seitenverwaltung erstellt.

## Weitere Informationen

- **pwg_representative**: (optional) für Elemente, die keine Bilder sind. Beispiel: eine ZIP-Datei. Da die ZIP-Datei kein Bild ist, wird in der Galerie das .jpg-Bild mit demselben Namen angezeigt, und die ZIP-Datei kann über das Disketten-Symbol heruntergeladen werden.

## Tipps

- Deaktivieren Sie *Suche in Unteralben* nicht.
- Verwenden Sie einfache Namen, es gibt Einschränkungen (bedingt durch das Web, siehe unten).
- Regeln für die Schreibweise der Namen von Verzeichnissen und Bildern:
    - keine Leerzeichen und keine Akzente
    - also nur Buchstaben, Ziffern oder die Zeichen "-", "_" und ".".
- Bereiten Sie Ihre Elemente vor, bevor Sie sie auf dem Server ablegen.

## Einzelne Synchronisierung

Im Administrationsbereich von Piwigo können Sie die Metadaten eines einzelnen Fotos erneut synchronisieren, indem Sie auf der Bearbeitungsseite des Fotos auf das Symbol „Synchronisieren von Metadaten“ klicken.

![Synchroniser unitaire.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-ada63451.jpg)
