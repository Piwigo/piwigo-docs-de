---
title: Mehrere Formate - Piwigo-Dokumentation
description: Erfahren Sie, wie Sie mit der Funktion für mehrere Formate verschiedene Versionen (JPG, PNG, PDF …) eines einzelnen Bildes in Ihrer Piwigo-Galerie anbieten.
---

# Mehrere Formate für ein einzelnes Foto

Mit mehreren Formaten können Sie beim Herunterladen eines einzelnen Fotos oder Bildes verschiedene Versionen anbieten. Zum Beispiel:

- eine JPG-Version und eine PNG-Version;
- eine JPG-Version, eine PSD-Version und eine PDF-Version
- usw.

!!! info "Wenn Sie Kunde der Piwigo Cloud sind, ist dieses Plugin erst ab dem Enterprise-Tarif verfügbar."

## Wie aktiviere ich mehrere Formate?

Die Antwort hängt davon ab, ob Sie eine selbst gehostete Piwigo-Galerie verwenden oder Kunde der Piwigo Cloud sind.

- Ich hoste meine Galerie selbst (oder meine Organisation tut das)
    
    Um diese Option zu aktivieren, verwenden Sie [LocalFiles Editor](../piwigo-selbst-hosten/lokale-konfiguration-bearbeiten-localfiles-editor.md) und fügen den folgenden Code in Ihre Konfigurationsdatei ein. Wenn Sie das nicht selbst tun können, wenden Sie sich an den Webmaster, der Ihre Galerie verwaltet.
    
    ```php
    // enable_formats: should Piwigo search for multiple formats?
    $conf['enable_formats'] = true;
    ```
    
    Mit der folgenden Einstellung können Sie die standardmässig akzeptierten Formate ändern.
    
    ```php
    // photo (or nay other file). Formats are in sub-directory pwg_format.
    $conf['format_ext'] = array('cr2', 'tif', 'tiff', 'nef', 'dng', 'ai', 'psd');
    ```
    
- Ich bin Kunde der Piwigo Cloud
    
    Diese Funktion steht Kunden der [Piwigo Cloud](https://de.piwigo.org/piwigo-bekommen) mit einem Enterprise- oder VIP-Tarif zur Verfügung. Um sie für Ihre Galerie zu aktivieren, wenden Sie sich an den Support.
    

## Mehrere Formate zu einem Foto hinzufügen

Sobald die Option für mehrere Formate aktiviert ist, erscheint beim Bearbeiten eines Fotos im Administrationsbereich von Piwigo ein neuer Tab „Formate“.

![Edit photo formats.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-ebaca22d.jpg)

Klicken Sie auf „Formate hinzufügen“, um eine oder mehrere Versionen des aktuellen Fotos hinzuzufügen.

Sie gelangen dann zum Upload-Formular. Dort wird Ihnen das Foto angezeigt, dem die neuen Formate zugeordnet werden. Sie können beliebig viele Formate hinzufügen, sofern Ihre Konfiguration sie akzeptiert.

![Formats Upload.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-59b21a2f.jpg)

Klicken Sie auf „Upload starten“, um die Dateien an den Server zu senden.

Sobald die Formate hinzugefügt sind, sehen Sie sie im Administrationsbereich im Tab „Formate“ Ihres Fotos.

![Edit photo TIFF.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-33a26685.jpg)

Wenn die Option für mehrere Formate aktiviert ist, können Sie neue Formate auch auf der Seite zum Hochladen von Fotos hinzufügen, indem Sie die Option „Upload-Formate“ wählen. In diesem Fall müssen die Dateien denselben Namen haben wie die Datei, der Sie die neuen Formate hinzufügen möchten.

![Upload formats.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-50117a2b.jpg)

## Mehrere Formate in meiner Galerie anzeigen

Um die verfügbaren Formate eines Fotos in Ihrer Galerie anzuzeigen, müssen Sie das Plugin **Download Formats Buttons** installieren.

Sobald das Plugin aktiviert ist, zeigt die Schaltfläche zum Herunterladen einer Datei die verfügbaren Formate und die jeweilige Dateigrösse an. Klicken Sie auf das gewünschte Format, um es herunterzuladen.

![Download formats.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-867a63cf.jpg)
