---
title: Fotos bearbeiten oder löschen - Piwigo-Dokumentation
description: Wie bearbeite ich ein Foto in Piwigo? Wie können Administratoren eine vorhandene Datei ändern oder löschen?
---

# Fotos bearbeiten oder löschen

Als Administrator von Piwigo müssen Sie vielleicht jederzeit ein Bild oder eine Datei eines anderen Typs ändern.

Wenn Sie eine bestimmte Datei bearbeiten möchten, geht das am einfachsten über Ihre Galerie!

Öffnen Sie die Seite Ihres Fotos und klicken Sie in der Werkzeugleiste auf die Schaltfläche mit dem Stift.

![edit-photo.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-c6929531.png)

!!! info "Info:"
    Je nach Erscheinungsbild befindet sich die Schaltfläche nicht immer an derselben Stelle. Wenn Sie Administrator sind und die Schaltfläche zum Bearbeiten in Ihrer Galerie nicht sehen, wurde sie ausgeblendet. Um sie anzuzeigen, gehen Sie im Administrationsbereich von Piwigo zu Konfiguration > Optionen, öffnen Sie den Tab „Anzeige“ und aktivieren Sie im Abschnitt „Fotoseite“ die Option „Symbol »Foto bearbeiten« anzeigen“. [Mehr über die Konfiguration von Piwigo erfahren](../ihre-galerie-anpassen/anpassungsoptionen-fuer-ihre-galerie.md)

Danach öffnet sich die Bearbeitungsseite des Fotos, auf der Sie seine Eigenschaften ändern können.

!!! info "Sie können ein Foto auch im Administrationsbereich bearbeiten, und zwar in der [Stapelverarbeitung](stapelverarbeitung.md)."

![image.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-ee638764.png)

## Vorschau, Herunterladen, Löschen, Metadaten synchronisieren

Wenn Sie sich im Administrationsbereich auf der Bearbeitungsseite des Fotos befinden, sehen Sie links ein Vorschaubild Ihrer Datei.

![image.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-985955e0.png)

In diesem Bereich stehen Ihnen mehrere Aktionen zur Verfügung:

- Foto vergrössern: Klicken Sie auf das Symbol zum Vergrössern.
- Foto in Ihrer Galerie anzeigen: Bewegen Sie dazu die Maus über das Bild und klicken Sie auf die Schaltfläche „In Galerie öffnen“. Die Seite dieses Fotos in Ihrer Galerie wird in einem neuen Tab angezeigt.
- Foto herunterladen: Klicken Sie auf das 2. Symbol mit dem Pfeil. Die Originaldatei wird auf Ihren Computer heruntergeladen.
- Besuchsverlauf dieses Fotos ansehen: Klicken Sie auf das Symbol mit dem Diagramm.
- Metadaten synchronisieren: Klicken Sie dazu auf das 4. Symbol mit den zwei Pfeilen. Das ist nur nötig, wenn die Konfiguration der Metadaten geändert wurde. [Mehr über Metadaten erfahren](eigenschaften-und-metadaten-von-fotos.md)
- Foto löschen: Klicken Sie auf das 5. Symbol mit dem Papierkorb.

## Die Metadaten Ihrer Datei

Oben rechts im Foto-Editor werden einige Metadaten Ihrer Datei angezeigt (Dateiname, Abmessungen und Dateigrösse, Dateiformat). Dazu kommen Angaben, die Sie auf dieser Seite nicht bearbeiten können (Datum des Uploads, Benutzer, der die Datei hochgeladen hat, Anzahl der Aufrufe …).

![File metadata.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-b873a50a.jpg)

Metadaten sind Informationen, die zu Ihren Fotos gehören und automatisch aus den Metadaten der Quelldatei ausgelesen werden (mehr dazu im Artikel [Eigenschaften und Metadaten](eigenschaften-und-metadaten-von-fotos.md)).

## Die Eigenschaften Ihrer Datei bearbeiten

Im rechten Teil der Seite sehen Sie die Eigenschaften Ihrer Datei, die Sie bearbeiten können: Titel, Beschreibung, Autor, Aufnahmedatum …

![image.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-4c7c49b8.png)

!!! warning "Vergessen Sie nicht, auf die Schaltfläche „Einstellungen sichern“ zu klicken, um Ihre Änderungen zu speichern!"

Mehr über die Eigenschaften Ihrer Dateien, ihre Rolle, warum und wie Sie sie bearbeiten und welche erweiterten Optionen es gibt, erfahren Sie im Artikel [Eigenschaften und Metadaten](eigenschaften-und-metadaten-von-fotos.md).

## Den Bildschwerpunkt eines Fotos ändern

Die Bearbeitungsseite eines Fotos hat einen zweiten Tab: **Bildschwerpunkt**.

In diesem Tab legen Sie den wichtigsten Teil Ihres Fotos fest. Dieser Teil bleibt sichtbar, wenn das Foto zugeschnitten wird, zum Beispiel im quadratischen Format.

Oben auf der Seite sehen Sie, wie Ihr Foto im quadratischen Format aussieht, darunter das Original.

Manchmal passt das quadratische Format nicht, weil Piwigo automatisch einen wichtigen Teil Ihres Bildes abschneidet. Im Beispiel unten soll das Foto unten nicht abgeschnitten werden.

![Center of interest.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-492ee557.jpg)

Um den Bildschwerpunkt zu ändern, markieren Sie mit der Maus den interessantesten Teil Ihres Fotos auf dem Bild unter dem Vorschaubild. Klicken Sie dann auf „Absenden“.

![Crop.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-eda08564.jpg)

Das quadratische Format wird entsprechend Ihren Änderungen aktualisiert.

Das ist besonders nützlich, wenn Ihre Galerie Vorschaubilder in einem anderen Format als üblich anzeigt, zum Beispiel im Querformat, obwohl das Originalfoto im Hochformat ist. Das ist etwa beim Erscheinungsbild [Bootstrap Darkroom](../erscheinungsbilder/bootstrap-darkroom-erscheinungsbild.md) der Fall.

## Photo Update: Eine Datei ersetzen, ohne ihre Eigenschaften zu ändern

Auf der Bearbeitungsseite eines Fotos können Sie eine neue Datei hochladen, um die Originaldatei zu ersetzen. Die Eigenschaften des Fotos bleiben dabei erhalten.

Dazu müssen Sie das Plugin **Photo Update** installieren.

Sobald das Plugin aktiviert ist, erscheint auf der Bearbeitungsseite des Fotos ein neuer Tab „Aktualisieren“. Über diesen Tab können Sie eine neue Datei importieren, die die vorhandene Datei ersetzt.

![Plugin Photo Update.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-b1a77acc.jpg)

Damit können Sie auch das Bild aktualisieren, das eine Datei ohne Bildinhalt darstellt (Video, Audio, Dokument usw.).

![Ohne Titel](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-adb35d74.png)

## Rotate Image: Ein Bild drehen

Auf der Bearbeitungsseite eines Fotos können Sie ein Bild drehen, wenn es nicht richtig ausgerichtet ist.

Dazu müssen Sie das Plugin **Rotate Image** installieren.

Sobald das Plugin aktiviert ist, erscheint auf der Bearbeitungsseite des Fotos ein neuer Tab „Drehen“.

![Plugin Rotate Image.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-e216d6fb.jpg)
