---
title: Eigenschaften und Metadaten von Fotos - Piwigo-Dokumentation
description: Dieser Artikel stellt alle Möglichkeiten vor, die Piwigo bietet, um Ihre Dateien mit Eigenschaften und Metadaten zu beschreiben, zu organisieren, zu präsentieren und zu indexieren.
---

# Eigenschaften und Metadaten Ihrer Dateien verwalten

**Dieser Artikel stellt alle Möglichkeiten vor, die Piwigo bietet, um Ihre Dateien mit Eigenschaften und Metadaten zu beschreiben, zu organisieren, zu präsentieren und zu indexieren.**

## Glossar

Zunächst ein paar Begriffsklärungen!

### Was sind Metadaten?

Metadaten sind Angaben aus der Originaldatei. Piwigo liest sie beim Import aus und übernimmt sie.

Metadaten sind vor allem bei Fotos relevant. Sie werden direkt vom Gerät bei der Aufnahme gespeichert oder von einer Fotoverwaltungssoftware, die der Fotograf verwendet.

Piwigo verarbeitet zwei Arten von Metadaten:

- **EXIF**: Diese Tags beschreiben in der Regel, wie ein Foto aufgenommen wurde. Sie können zum Beispiel Informationen über das verwendete Kamera- oder Smartphone-Modell, das Objektiv, die Blende, die Brennweite, die Belichtungszeit, Datum und Uhrzeit, GPS-Koordinaten usw. enthalten.
- **IPTC:** IPTC-Header beschreiben den Inhalt des Bildes. Bei manchen Kameras können Sie über diesen Header Ihren Namen und weitere Urheberrechtsangaben in einem digitalen Foto speichern. Manchmal wird später eine Bearbeitungssoftware verwendet, um Informationen wie Titel, Überschriften, Bildunterschriften, Beschreibungen, Stichwörter usw. hinzuzufügen.

Die grundlegenden Metadaten sind:

- Dateiname
- Dateigrösse
- Abmessungen der Datei
- Autor
- Aufnahmedatum

Es können viele weitere Metadaten vorhanden sein, etwa die Kameramarke, das Modell, Details zur Aufnahme, Stichwörter…

Wenn Sie Ihre Dateien aus einer externen Software wie Lightroom, Digikam, Shotwell oder Aperture in Piwigo importieren, werden die Metadaten aus dieser Software in Piwigo übernommen.

Standardmässig zeigt Piwigo auf der Fotoseite einige **grundlegende** Metadaten an (Abmessungen, Dateigrösse usw.). Wenn Sie auf das Symbol „Metadaten anzeigen“ klicken, werden weitere **EXIF**-Metadaten angezeigt: Kameramarke und -modell, Aufnahmedatum und -uhrzeit sowie die Blendenzahl. IPTC-Metadaten zeigt Piwigo standardmässig nicht an.

![Die Metadaten im Erscheinungsbild Modus](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-5b2fae89.jpg)

Die Metadaten im Erscheinungsbild Modus

![Die Metadaten im Erscheinungsbild Bootstrap Darkroom](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-e87db559.jpg)

Die Metadaten im Erscheinungsbild Bootstrap Darkroom

### Was sind Eigenschaften?

Eigenschaften sind Piwigo-eigene Felder, mit denen Sie Ihre Dateien beschreiben und sortieren.

Einige Eigenschaften werden von Piwigo erzeugt, zum Beispiel das Importdatum. Andere werden aus den Metadaten übernommen, zum Beispiel das Aufnahmedatum (das Datum, an dem das Foto aufgenommen wurde). Wieder andere legen Sie selbst fest.

Einige Eigenschaften können mit Plugins hinzugefügt werden. Mit dem Plugin **Manage Properties Photos** können Sie sogar eigene Eigenschaften erstellen (darauf gehen wir weiter unten in diesem Artikel ein).

In jedem Fall lassen sich diese Eigenschaften bearbeiten. Sie können in der Galerie angezeigt werden.

![Die Eigenschaften im Erscheinungsbild Modus](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-ce5c160e.jpg)

Die Eigenschaften im Erscheinungsbild Modus

![Die Eigenschaften im Erscheinungsbild Bootstrap Darkroom](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-78d870bc.jpg)

Die Eigenschaften im Erscheinungsbild Bootstrap Darkroom

## Metadaten Ihrer Fotos in Piwigo verwalten

Wie gesagt, werden Metadaten beim Import von Fotos automatisch in Piwigo übernommen.

Es gibt aber einige Optionen, die Sie kennen sollten, um diese Metadaten anzuzeigen und zu verwalten.

### Metadaten in der Piwigo-Galerie anzeigen

**Metadaten mit Modus anzeigen**

Im Erscheinungsbild [Modus](../erscheinungsbilder/modus-erscheinungsbild.md) können Sie die Metadaten über ein Kamerasymbol auf der Seite eines Fotos anzeigen.

![afficher-metadonnees.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-03424eb2.png)

Wenn Sie auf dieses Symbol klicken, werden im Bereich rechts einige Metadaten zu den Eigenschaften hinzugefügt.

![EXIF metadata.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-5b2fae89.jpg)

Wenn Sie das Symbol zur Anzeige der Metadaten in Ihrer Galerie ausblenden möchten, öffnen Sie den Administrationsbereich: Im Menü Konfiguration > Optionen, Tab „Anzeige“, Abschnitt „Fotoseite“ können Sie die Option „Symbol »Metadaten anzeigen« anzeigen“ aktivieren oder deaktivieren.

Wenn die Metadaten in Ihrer Galerie immer angezeigt werden sollen, ohne dass man auf dieses Symbol klicken muss, laden Sie das Plugin **AlwaysShowMetadata** herunter.

**Metadaten mit Bootstrap Darkroom anzeigen**

Im Erscheinungsbild [Bootstrap Darkroom](../erscheinungsbilder/bootstrap-darkroom-erscheinungsbild.md) werden die Metadaten, sofern vorhanden, standardmässig unter dem Foto in der rechten Spalte angezeigt.

Je nachdem, welche Option Sie bei der Einrichtung des Erscheinungsbilds gewählt haben, können sie auch in einem Tab oder in einer Seitenleiste angezeigt werden.

![Darkroom theme.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-423ae635.jpg)

Wenn Sie die Metadaten im Erscheinungsbild Bootstrap Darkroom ausblenden möchten, müssen Sie in der Konfiguration des Erscheinungsbilds auch die Eigenschaften ausblenden. Wählen Sie dazu die Option „Anzeigeposition der Bildinformationen = Deaktiviert“.

![Picture page display.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-7d14f38d.jpg)

### Metadaten synchronisieren

Auf der Bearbeitungsseite eines Fotos im Administrationsbereich können Sie die Metadaten einer Datei über eine Schaltfläche synchronisieren. Dabei werden die Metadaten Ihrer Dateien in Ihre Piwigo-Datenbank übernommen. Normalerweise geschieht das automatisch, wenn Sie die Dateien in Piwigo importieren.

Nützlich ist diese Funktion aber, wenn Fotos per FTP importiert wurden und der Synchronisierungsschritt ausgelassen wurde. 

Sie kann auch nach einer Änderung der Konfiguration hilfreich sein, um die neuen Einstellungen für den Metadaten-Import anzuwenden.

Wenn Sie Piwigo selbst hosten und Ihre Dateien per FTP-Synchronisierung importieren, können Sie die Metadaten auch gesammelt über das Menü „Synchronisieren“ in Ihrem Administrationsbereich synchronisieren. [Mehr über die FTP-Synchronisierung erfahren](../piwigo-selbst-hosten/fotos-per-ftp-importieren-und-synchronisieren.md)

### Read Metadata: Alle Metadaten einer Datei anzeigen

Wenn Sie im Administrationsbereich alle Metadaten einer Datei aus Ihrer Galerie anzeigen möchten, müssen Sie das Plugin **Read Metadata** installieren.

Auf der Konfigurationsseite dieses Plugins können Sie die Metadaten einer Datei auslesen, entweder über ihre ID oder durch Auswahl in einer Dropdown-Liste.

![Read metadata.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-b8adfb2b.jpg)

### Weitere EXIF-Metadaten anzeigen

Wie gesagt, zeigt Piwigo standardmässig einige EXIF-Metadaten an. Sie können aber auf Wunsch weitere EXIF-Felder anzeigen. 

Wenn Sie Kunde von Piwigo cloud sind, wenden Sie sich an den Support.

Wenn Sie eine selbst gehostete Piwigo-Galerie verwalten, bearbeiten Sie einfach die Konfigurationsdatei mit [LocalFiles Editor](../piwigo-selbst-hosten/lokale-konfiguration-bearbeiten-localfiles-editor.md).

- Klicken Sie hier, um zu sehen, wie Sie Ihrer Piwigo-Galerie neue EXIF-Felder hinzufügen
    
    Standardmässig werden diese EXIF-Felder angezeigt:
    
    ```php
    $conf['show_exif_fields'] = array(
      'Make',
      'Model',
      'DateTimeOriginal',
      'COMPUTED;ApertureFNumber'
      );
    ```
    
    Um *weitere* EXIF-Felder anzuzeigen, fügen Sie einfach deren Schlüssel mit LocalFiles Editor in Ihre Konfigurationsdatei ein. Wenn Sie den folgenden Beispielcode in Ihre Konfiguration einfügen, werden einige zusätzliche Kameraeinstellungen angezeigt:
    
    ```php
    $conf['show_exif_fields'] = array(
      'DateTimeOriginal',
      'Make',
      'Model',
      'ExposureProgram',
      'FocalLengthIn35mmFilm',
      'FNumber',
      'ExposureTime',
      'ISOSpeedRatings',
      'Flash',
      'WhiteBalance',
      'UserComment'
      );
    ```
    
    Alle verfügbaren EXIF-Metadaten sehen Sie mit dem Plugin Read Metadata, das im vorherigen Kapitel vorgestellt wurde.
    
    Wenn Sie in Ihrer Galerie überhaupt keine EXIF-Metadaten anzeigen möchten, fügen Sie einfach folgenden Code in Ihre Konfigurationsdatei ein:
    
    ```php
    $conf['show_exif'] = false;
    ```
    

### IPTC-Metadaten anzeigen

Wie gesagt, zeigt Piwigo IPTC-Metadaten standardmässig nicht an. Möglich ist es aber!

 Wenn Sie Kunde von Piwigo cloud sind, wenden Sie sich an den Support.

Wenn Sie eine selbst gehostete Piwigo-Galerie verwalten, bearbeiten Sie einfach die Konfigurationsdateien mit [LocalFiles Editor](../piwigo-selbst-hosten/lokale-konfiguration-bearbeiten-localfiles-editor.md).

- Klicken Sie hier, um zu sehen, wie Sie IPTC-Felder in Ihrer Piwigo-Galerie anzeigen
    
    Fügen Sie diesen Parameter mit LocalFiles Editor in Ihre Konfigurationsdatei ein.
    
    ```php
    $conf['show_iptc'] = true;
    ```
    
    Anschliessend müssen Sie festlegen, welche Felder angezeigt werden sollen. Hier ein Beispiel:
    
    ```php
    $conf['show_iptc_mapping'] = array(
      'iptc_creator'         => '2#080',
      'iptc_title'           => '2#005',
      'iptc_headline'        => '2#105',
      'iptc_description'     => '2#120',
      'iptc_keywords'        => '2#025',
      );
    ```
    
    Alle verfügbaren IPTC-Metadaten sehen Sie mit dem Plugin Read Metadata, das weiter oben auf dieser Seite vorgestellt wurde.
    

### Metadaten Eigenschaften zuordnen

Standardmässig können EXIF- und IPTC-Metadaten auf der Fotoseite angezeigt werden, sie sind aber nicht durchsuchbar.

Bei Bedarf können Sie bestimmte Metadaten Piwigo-Eigenschaften zuordnen, damit sie zum Suchen und Sortieren von Fotos in Ihrer Galerie genutzt werden können. Zum Beispiel können Sie das EXIF-Feld „Model“ als Schlagwort übernehmen, wenn Sie Fotos nach Kameramodell filtern möchten.

 Wenn Sie Kunde von Piwigo cloud sind, wenden Sie sich dazu an den Support.

Wenn Sie eine selbst gehostete Piwigo-Galerie verwalten, bearbeiten Sie einfach die Konfigurationsdateien mit [LocalFiles Editor](../piwigo-selbst-hosten/lokale-konfiguration-bearbeiten-localfiles-editor.md).

- Klicken Sie hier, um zu sehen, wie Sie EXIF-Metadaten Eigenschaften zuordnen
    
    Standardmässig wird die EXIF-Angabe „DateTimeOriginal“ dank des folgenden Konfigurationsparameters als Aufnahmedatum in Piwigo übernommen.
    
    ```php
     $conf['use_exif_mapping'] = array('date_creation' => 'DateTimeOriginal' ); 
    ```
    
    Weitere Zuordnungen fügen Sie hinzu, indem Sie diesem Parameter neue Zeilen hinzufügen. 
    
    Dieses Beispiel übernimmt Kommentare in die Eigenschaft Beschreibung:
    
    ```php
    $conf['use_exif_mapping'] = array(
      'date_creation'        => 'DateTimeOriginal',
      'comment'              => 'UserComment',
      );
    ```
    
    Dieses Beispiel übernimmt Kameramodelle als Schlagworte:
    
    ```php
    $conf['use_exif_mapping'] = array(
      'date_creation'        => 'DateTimeOriginal',
      'tags'                 => 'Model',
      );
    ```
    
- Klicken Sie hier, um zu sehen, wie Sie IPTC-Metadaten Eigenschaften zuordnen
    
    Beispiel für eine erweiterte Zuordnung, die IPTC-Metadaten (oft mit Adobe Lightroom hinzugefügt) in die entsprechenden Piwigo-Felder übernimmt.
    
    ```php
    $conf['use_iptc_mapping'] = array(
      'author'          => '2#080',
      'name'            => '2#005',
      'comment'         => '2#120',
      'keywords'        => '2#025',
      );
    ```
    

### Write Metadata: Metadaten durch Eigenschaften ersetzen

Wenn Sie bestimmte IPTC-Metadaten in den Dateien Ihrer Galerie durch die Informationen aus den Piwigo-Eigenschaften (Titel, Beschreibung, Autoren, Schlagworte) ersetzen möchten, müssen Sie das Plugin **Write Metadata** installieren.

!!! info "Für Kunden von Piwigo Cloud ist dieses Plugin erst ab dem Team-Tarif verfügbar"

### Exif View: EXIF-Werte Ihrer Fotos übersetzen

Wenn Sie EXIF-Werte in die Sprache der Galerie übersetzen möchten, müssen Sie das Plugin **Exif View** installieren.

### IPTC from Mac: Probleme mit Sonderzeichen in Ihren Metadaten beheben

Wenn Sie in den IPTC-Metadaten Ihrer Fotos seltsame Zeichen sehen, können Sie das Plugin IPTC from Mac installieren. Es wandelt IPTC-Daten, die in MacRoman geschrieben wurden, in die Kodierung UTF-8 um.

## Eigenschaften in Piwigo verwalten

### Eigenschaften einer Datei bearbeiten

Anders als die Metadaten legen Sie die Eigenschaften Ihrer Dateien in Piwigo selbst fest. Sie können sie bearbeiten, wenn Sie ein Foto im Administrationsbereich bearbeiten.

![File properties.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-1c3748d1.jpg)

!!! info "Mehr zur Bearbeitung von Fotos erfahren Sie in diesen Artikeln:"
    
    - [Fotos bearbeiten oder löschen](fotos-bearbeiten-oder-loeschen.md)
    
    - [Stapelverarbeitung](stapelverarbeitung.md)

Diese Eigenschaften und Informationen bietet Piwigo standardmässig an, um eine Datei zu beschreiben.

### Titel

Dies ist der Name des Fotos, der in der Galerie angezeigt wird. Je nach Erscheinungsbild und gewählten Einstellungen erscheint der Titel an mehreren Stellen in Ihrer Galerie.

Standardmässig wird der Name aus dem Dateinamen gebildet, Sie können ihn aber ändern.

Über den Namen eines Fotos finden Sie es mit der Suchfunktion leicht wieder: Er ist also eine wichtige Einstellung.

### Autor

Mit dieser Eigenschaft nennen Sie den Urheber, zum Beispiel den Fotografen, der das Foto aufgenommen hat. Es handelt sich um ein freies Textfeld, das später in der Galerie angezeigt werden kann.

### Aufnahmedatum

Standardmässig wird das Aufnahmedatum aus den *Metadaten* der Datei übernommen.

Bei einem Foto ist das in der Regel das Datum, an dem es aufgenommen wurde. Bei anderen Dateitypen ist es das Erstellungsdatum der Datei.

Beim Bearbeiten eines Fotos können Sie auf „Einstellung löschen“ klicken, um diese Eigenschaft leer zu lassen, oder das Datum ändern, wenn Ihnen das standardmässig angezeigte Datum nicht gefällt.

### Verknüpfte Alben

Genau genommen sind verknüpfte Alben keine Eigenschaft, auch wenn sie in der Liste der Eigenschaften eines Fotos erscheinen.

Gemeint sind das Album oder die Alben, in denen sich dieses Foto befindet.

Zur Erinnerung: In Piwigo kann sich eine Datei in mehreren Alben befinden.

Klicken Sie beim Bearbeiten eines Fotos auf das Kreuz beim Namen eines Albums, um das Foto aus diesem Album zu entfernen.

Um das Foto einem weiteren Album hinzuzufügen, klicken Sie auf die Schaltfläche „Hinzufügen“.

![Linked albums.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-6d2c744f.jpg)

Es öffnet sich ein Fenster mit den vorhandenen Alben. Dort können Sie auch nach dem gewünschten Album suchen. Klicken Sie auf +, um das Foto dem ausgewählten Album hinzuzufügen. Sie können auch ein neues Album erstellen, indem Sie auf „Erstellungsmodus“ klicken.

![image.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-fc0d4b05.png)

Sobald Sie Ihre Alben ausgewählt haben, gelangen Sie zurück zur Bearbeitungsseite des Fotos. Vergessen Sie nicht, auf die Schaltfläche „Einstellungen sichern“ zu klicken, um Ihre Änderungen zu speichern!

Mehr über Alben erfahren Sie [in dieser Artikelreihe](../alben-organisieren/index.md).

### Album-Vorschaubild

Beim Bearbeiten eines Fotos zeigt diese Eigenschaft die Liste der Alben, für die das aktuelle Foto als Vorschaubild ausgewählt wurde.

![image.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-625b5c29.png)

Wenn ein Foto als Vorschaubild eines Albums ausgewählt ist, wird es in Ihrer Galerie in der Albenliste angezeigt.

Standardmässig wählt Piwigo als Vorschaubild eines Albums das erste Foto, das in das Album hochgeladen wurde. Sie können es aber jederzeit ändern.

Übrigens muss ein Foto nicht mit einem Album verknüpft sein, um als dessen Vorschaubild zu dienen.

Mehr über Alben erfahren Sie [in dieser Artikelreihe](../alben-organisieren/index.md).

### Schlagworte

Um Ihre Fotos zu organisieren und zu beschreiben, können Sie sie mit Schlagworten (auch Stichwörter oder Labels genannt) verknüpfen.

Schlagworte werden auf der Seite eines Fotos in Ihrer Galerie genauso wie die Eigenschaften angezeigt. Mit ihnen können Sie nach Fotos suchen, die einem oder mehreren Kriterien entsprechen.

Beim Bearbeiten eines Fotos im Administrationsbereich funktioniert das Feld Schlagworte genauso wie das Feld Alben, mit einem Unterschied: Wenn Sie den Namen eines Schlagworts eingeben, das noch nicht existiert, können Sie es direkt mit der Eingabetaste erstellen.

![Adding tags.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-d58bf57c.jpg)

Mehr über Schlagworte erfahren Sie [in dieser Artikelreihe](../schlagworte-verwalten/index.md).

### Beschreibung

Mit der Eigenschaft Beschreibung können Sie in Ihrer Galerie einen Begleittext zu Ihrem Foto anzeigen.

In der Regel wird die Beschreibung in Ihrer Galerie unter dem Foto angezeigt.

Standardmässig erscheint die Beschreibung auch als Tooltip, wenn Sie mit der Maus über das Foto fahren.

![Photo description.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-cd17604c.jpg)

Im Erscheinungsbild [Bootstrap Darkroom](../erscheinungsbilder/bootstrap-darkroom-erscheinungsbild.md) können Sie auf der Seite eines Albums die Beschreibung der Fotos anstelle ihres Titels anzeigen.

Um den Text Ihrer Beschreibung zu formatieren (fett schreiben, einen Link hinzufügen...), haben Sie zwei Möglichkeiten.

- Wenn Sie HTML beherrschen, können Sie HTML-Tags in Ihre Beschreibungen einfügen.
- Sie können auch das Plugin **FCKEditor** installieren, das dem Feld Beschreibung im Foto-Editor einen visuellen HTML-Editor hinzufügt.

![FCKEditor.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-b482ad9d.jpg)

Mehr über FCKEditor erfahren Sie [in diesem Artikel](../piwigo-administrieren/plugins-fuer-administratoren.md).

Um Beschreibungen in mehrere Sprachen zu übersetzen, verwenden Sie das Plugin **Extended Description**. Mehr über die Übersetzung von Inhalten mit Extended Description erfahren Sie [in diesem Artikel](../ihre-galerie-anpassen/verfuegbare-sprachen-der-galerie-verwalten.md).

### Wer soll dieses Foto sehen können? (Datenschutzstufe)

Mit dieser Eigenschaft legen Sie die Datenschutzstufe einer Datei fest.

Standardmässig ist die Datenschutzstufe auf „Jeder“ gesetzt: Wenn das Album privat ist, wird das Foto allen Benutzern angezeigt, die angemeldet und berechtigt sind, das Album anzusehen.

![Privacy level.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-0e6c29d2.jpg)

Sie können aber eine feinere Datenschutzstufe festlegen, indem Sie im Dropdown-Menü eine andere Option wählen.

![Other privacy levels.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-2737cf4d.png)

!!! warning "Achtung:"
    Verwechseln Sie diese Funktion nicht mit den Zugriffsrechten für Alben! Es handelt sich um eine fortgeschrittene Funktion von Piwigo, die etwas schwer zu verstehen sein kann.

Mehr über Datenschutzstufen erfahren Sie [in diesem Artikel](../benutzer-verwalten/datenschutzstufen.md).

### Eigenschaften in Ihrer Galerie anzeigen

**Eigenschaften im Erscheinungsbild Modus anzeigen**

Im Erscheinungsbild [Modus](../erscheinungsbilder/modus-erscheinungsbild.md) werden die Eigenschaften im Bereich rechts neben dem Foto angezeigt.

![Description.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-151d7151.jpg)

**Eigenschaften im Erscheinungsbild Bootstrap Darkroom anzeigen**

Im Erscheinungsbild [Bootstrap Darkroom](../erscheinungsbilder/bootstrap-darkroom-erscheinungsbild.md) werden die Eigenschaften standardmässig unter dem Foto in der rechten Spalte angezeigt.

Je nachdem, welche Option Sie in der Konfiguration des Erscheinungsbilds gewählt haben, können sie auch in einem Tab oder in einer Seitenleiste angezeigt werden.

![Darkroom theme.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-423ae635.jpg)

Wenn Sie die Eigenschaften im Erscheinungsbild Bootstrap Darkroom ausblenden möchten, wählen Sie in der Konfiguration des Erscheinungsbilds die Option „Anzeigeposition der Bildinformationen = Deaktiviert“.

**Eigenschaften in der Galerie ein- und ausblenden**

Wenn Sie festlegen möchten, welche Eigenschaften neben den Dateien in Ihrer Galerie angezeigt werden und welche nicht, öffnen Sie im Administrationsbereich das Menü Konfiguration > Optionen, dann den Tab „Anzeige“ und den Abschnitt „Fotoeigenschaften“.

![Photo properties.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-ec28a274.jpg)

Weitere Anzeigeoptionen für Eigenschaften erhalten Sie mit dem Plugin **Manage Properties Photos** (siehe nächstes Kapitel).

## Eigenschaften mit Plugins anpassen

### Manage Properties Photos: Eigenschaften anpassen

Sie möchten Ihrer Galerie eigene Eigenschaften hinzufügen oder die Anzeigereihenfolge der vorhandenen Eigenschaften ändern?

Dazu müssen Sie das Plugin **Manage Properties Photos** installieren.

!!! info "Für Kunden von Piwigo Cloud ist dieses Plugin erst ab dem Enterprise-Tarif verfügbar"

Sobald Manage Properties Photos in Ihrer Galerie aktiviert ist, öffnen Sie die Konfiguration des Plugins.

Der Tab Eigenschaften listet die vorhandenen Eigenschaften auf und ermöglicht es, eine neue zu erstellen.

![Manage photo properties.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-a47105d7.jpg)

In diesem Tab können Sie vorhandene Eigenschaften ausblenden: Fahren Sie einfach mit der Maus über eine Eigenschaft, um die Option „Ausblenden“ anzuzeigen.

Ausserdem können Sie die Anzeigereihenfolge der Eigenschaften auf der Fotoseite Ihrer Galerie per Drag-and-drop ändern.

**Eine neue eigene Eigenschaft erstellen**

Um eine eigene Eigenschaft zu erstellen, klicken Sie auf „Neue Fotoeigenschaft erstellen“.

![New photo property.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-6ae92c9a.jpg)

Im Feld Bezeichnung legen Sie den Namen der neuen Eigenschaft fest.

Ausserdem müssen Sie den Typ der Eigenschaft wählen. Es stehen mehrere Typen zur Verfügung:

**Text:**

Wählen Sie den Typ Text, wenn der Wert Ihrer Eigenschaft ein freier Text ist (zum Beispiel ein Name, eine Stadt...).

**Auswahl:**

Wählen Sie den Typ Auswahl, wenn der Wert Ihrer Eigenschaft aus einer begrenzten Liste von Optionen stammt.

Mit der Schaltfläche „Feld hinzufügen“ legen Sie die verfügbaren Optionen für Ihre Eigenschaft fest. Im folgenden Beispiel haben wir eine Eigenschaft Schule mit 4 möglichen Werten erstellt.

![Select property.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-5c728505.jpg)

Auf der Bearbeitungsseite eines Fotos können Administratoren den Wert dieser Eigenschaft über ein Dropdown-Menü wählen.

![School property.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-52cb3141.jpg)

**Optionsfeld:**

Der Typ Optionsfeld funktioniert genauso wie der Typ Auswahl. Auch hier wählen Sie den Wert der Eigenschaft aus einer vordefinierten Liste, die Eingabe erfolgt jedoch über Optionsfelder statt über eine Dropdown-Liste.

Im folgenden Beispiel haben wir eine Eigenschaft „Bildrechte“ mit zwei Optionen erstellt: Ja und Nein.

![Radio property.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-206e119f.jpg)

**Datum:**

Der Typ Datum ist für Eigenschaften gedacht, die ein Datum enthalten. Damit legen Sie den Wert der Eigenschaft über einen Kalender fest.

![Due date.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-c13aa5be.jpg)

**Typen EXIF und IPTC:**

Mit Eigenschaften vom Typ EXIF oder IPTC erstellen Sie eine eigene Eigenschaft, die den Wert einer EXIF- oder IPTC-Angabe übernimmt.

Um diesen Eigenschaftstyp zu nutzen, öffnen Sie zuerst den Tab Konfiguration des Plugins. Wählen Sie dort ein Referenzfoto aus Ihrer Galerie, das EXIF- oder IPTC-Metadaten enthält, indem Sie seine numerische ID eingeben.

![EXIF IPTC.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-f1ee4b64.jpg)

So kann das Plugin die Liste der EXIF- und IPTC-Metadaten laden, die in Ihrer Galerie verfügbar sind.

![EXIF example.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-23c439de.jpg)

Sie können zum Beispiel eine Eigenschaft Höhe erstellen, die automatisch den Wert der in Ihrem Foto gespeicherten Angabe „Height“ übernimmt. Die Höhe wird dann auf der Fotoseite Ihrer Galerie in Pixeln angezeigt.

![Height value.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-52f485f1.jpg)

**Eigene Eigenschaften anzeigen**

Sobald Sie eine eigene Eigenschaft erstellt haben, können Sie ihren Wert für jedes Foto im Tab „Zusätzliche Eigenschaften“ des Foto-Editors festlegen.

![Image rights.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-442b52a2.jpg)

Eigene Eigenschaften sind auch in der Stapelverarbeitung verfügbar, wenn Sie eine Auswahl von Fotos treffen und die Aktion „Fotoeigenschaften ändern“ wählen.

![Batch manager properties.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-97bdf9a6.jpg)

Wenn Sie eigene Eigenschaften anzeigen lassen, erscheinen sie in der Galerie zusammen mit den anderen Eigenschaften. Denken Sie daran, dass Sie im ersten Tab der Plugin-Konfiguration die Anzeigereihenfolge der Eigenschaften ändern und die gewünschten Eigenschaften ausblenden können.

![Image rights yes.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-47514661.jpg)

**Optionen von Manage Properties**

Der Tab Konfiguration von Manage Properties bietet mehrere Optionen, die wir im Folgenden auflisten.

![Manage properties configuration.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-b5559618.jpg)

- **Ein Feld hinzufügen, um Fotos zu einem bestimmten Datum automatisch zu löschen**

Mit dieser Option erstellen Sie ein Feld vom Typ „Datum“, mit dem Sie für jedes Foto ein Datum festlegen, an dem es automatisch gelöscht wird

![Delete photos.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-fcd8f683.jpg)

- **Beschreibung in die Informationstabelle verschieben**

Mit dieser Option wird die Beschreibung des Fotos zusammen mit den Eigenschaften in Ihrer Galerie angezeigt. Das Feld Beschreibung erscheint dann in der Eigenschaftenliste der Plugin-Konfiguration, und Sie können seine Anzeigereihenfolge festlegen.

![Description property.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-905437ee.jpg)

- **ID des Bildes anzeigen**

Mit dieser Option wird die numerische ID jeder Datei zusammen mit den Eigenschaften in der Galerie angezeigt. Diese Funktion bietet auch das Plugin **Show Photo Identifier**.

- **Maximale Anzahl der Felder für Auswahllisten und Optionsfelder**

Legen Sie hier die maximale Anzahl möglicher Werte für Eigenschaften vom Typ „Dropdown-Liste“ und „Optionsfeld“ fest.

- **Das Referenzfoto für die EXIF- und IPTC-Metadaten**

Siehe vorheriges Kapitel.

### Properties Mass Update: Eigenschaften gesammelt aus einer .csv-Datei aktualisieren

Sie möchten die Eigenschaften einer Reihe von Fotos aus einer vorhandenen Tabelle (zum Beispiel einer Excel-Datei) aktualisieren?

Dazu müssen Sie das Plugin **Properties Mass Update** installieren.

!!! info "Für Kunden von Piwigo Cloud ist dieses Plugin erst ab dem Enterprise-Tarif verfügbar"

### Show Photo Identifier: Die ID des Fotos bei den Eigenschaften anzeigen

Mit dem Plugin **Show Photo Identifier** zeigen Sie die numerische ID eines Fotos auf der Fotoseite an, zusammen mit seinen Metadaten und Eigenschaften.

![Image ID.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-2ca0d794.jpg)

### Download Counter: Die Anzahl der Downloads bei den Eigenschaften anzeigen

Mit dem Plugin **Download Counter** zählen Sie, wie oft ein Foto heruntergeladen wurde, und zeigen diese Zahl auf der Fotoseite zusammen mit den Metadaten und Eigenschaften des Fotos an.

![Download counter.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-294cb0db.jpg)

### Expiry Date: Einer Datei ein Ablaufdatum hinzufügen

Ein Ablaufdatum für eine Datei kann nötig sein, um das Gültigkeitsdatum einer Lizenz oder die Gültigkeit der Bildrechte eines Fotos zu verwalten.

Dazu müssen Sie das Plugin **Expiry Date** installieren.

!!! info "Für Kunden von Piwigo Cloud ist dieses Plugin erst ab dem Enterprise-Tarif verfügbar"

Sobald das Plugin aktiviert ist, erscheint bei jedem Foto sowie in der Stapelverarbeitung ein neues Feld „Ablaufdatum“.

![Expiry date empty.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-722d1d17.jpg)

Das Ablaufdatum wird in Ihrer Galerie neben den anderen Eigenschaften angezeigt.

![Expiry date.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-46807707.jpg)

Wenn Sie das Ablaufdatum in der Galerie ausblenden möchten, müssen Sie das Plugin **Manage Properties Photo** verwenden (siehe weiter oben auf dieser Seite).

Aber was passiert, wenn das Ablaufdatum näher rückt?

Das legen Sie in der Konfiguration des Plugins Expiry Date fest.

![Expiry date configuration.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-d7d99c2a.jpg)

Sie haben mehrere Möglichkeiten:

- **Festlegen, was Piwigo tun soll, wenn Fotos bald ablaufen**

Mit dem Plugin Expiry Date legen Sie fest, was geschieht, wenn das Ablaufdatum näher rückt: nichts tun, die Fotos automatisch löschen oder die Fotos automatisch archivieren.

Beim Archivieren werden die Fotos automatisch in ein Album Ihrer Wahl verschoben, das Sie vorher erstellt haben. So machen Sie abgelaufene Fotos unzugänglich, ohne sie aus Ihrer Galerie zu löschen.

![Archived photos.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-2903a3ff.jpg)

- **Benutzer benachrichtigen, die das Foto heruntergeladen haben**

Wählen Sie diese Option, um die Benutzer, die ein Foto heruntergeladen haben, per E-Mail zu benachrichtigen, wenn es abläuft.

Wenn Sie diese Option wählen, erscheinen weitere Einstellungen.

![User notifications.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-0c5881a2.jpg)

So können Sie eine E-Mail vor dem Ablaufdatum oder erst genau am Ablaufdatum senden und der E-Mail eine eigene Nachricht hinzufügen.

- **Administratoren benachrichtigen, wenn ein Foto abgelaufen ist**

Sie können den Administratoren eine E-Mail senden, sobald das Ablaufdatum eines Fotos erreicht ist.

Wie bei den Benachrichtigungen an Benutzer können Sie die E-Mail vor dem Ablaufdatum oder erst genau am Ablaufdatum senden und eine eigene Nachricht hinzufügen.

### Copyrights: Urheberrechte einer Datei verwalten

Möglicherweise müssen Sie einem Bild oder Video ein Copyright zuordnen, um die Rechte an dieser Datei festzulegen (Nutzung, Vervielfältigung, Verbreitung...).

Dazu müssen Sie das Plugin **Copyrights** installieren.

Sobald das Plugin aktiviert ist, erscheint beim Bearbeiten eines Fotos im Administrationsbereich eine neue Eigenschaft „Copyright“.

![Copyrights.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-8a90932e.jpg)

Wenn ein Wert aus der Liste der verfügbaren Copyrights ausgewählt ist, wird er in Ihrer Galerie zusammen mit den anderen Eigenschaften angezeigt.

![Ohne Titel](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-b486b74b.png)

Das Plugin wird mit einer vordefinierten Liste von Copyrights installiert. In der Konfiguration des Plugins Copyrights können Sie diese aber löschen, bearbeiten oder neue erstellen.

![Create copyright.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-b41d9515.jpg)

Die Beschreibung eines Copyrights wird angezeigt, wenn Sie in der Galerie mit der Maus darüberfahren. Ein Klick auf das Copyright öffnet den Link in einem neuen Tab.

![CC BY.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-ce81eb1d.jpg)

### Edit Filename: Den Namen einer Datei bearbeiten

Im Foto-Editor von Piwigo können Sie standardmässig den Titel ändern, unter dem die Datei in Ihrer Galerie angezeigt wird, nicht aber den Namen der Quelldatei.

Wenn Sie das benötigen, müssen Sie das Plugin **Edit Filename** installieren.

Sobald dieses Plugin aktiviert ist, können Sie den Namen der Quelldatei auf der Bearbeitungsseite des Fotos ändern.

![Edit Filename.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-632b69a5.jpg)
