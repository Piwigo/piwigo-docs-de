---
title: Eigenes Banner erstellen - Piwigo-Dokumentation
description: Wie erstellen Sie ein eigenes Banner für Ihre Piwigo-Galerie? Das zeigen wir in diesem Artikel.
---

# Eigenes Banner zur Galerie hinzufügen

**Viele Benutzer möchten ihrer Galerie ein eigenes Banner hinzufügen, sei es als Bild, als Text oder als Kombination aus beidem.**

Dafür gibt es zwei wesentliche Möglichkeiten, die wir in diesem Artikel vorstellen:

## Das Feld „Seitenbanner“ verwenden

Standardmässig richten Sie ein Banner für Ihre Galerie im Menü Konfiguration > Optionen im Feld „Seitenbanner“ ein.

![Grundeinstellungen Banner](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-bc1edea8.jpg)

In dieses Feld können Sie reinen Text, aber auch HTML-Code eingeben. Wenn Sie das Plugin FCKEditor aktiviert haben, können Sie den HTML-Code visuell bearbeiten.

![Galerie mit FCKEditor ändern](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-2c07f8bf.jpg)

Sie können ganz einfach ein Bild einfügen, das in Ihrer Piwigo-Galerie, auf Ihrem Server oder auf einer anderen Website liegt. Kopieren Sie einfach die URL des Bildes und fügen Sie den folgenden HTML-Code in das Feld „Seitenbanner“ ein. Ersetzen Sie dabei die URL durch die URL Ihres Bildes.

```html
<img src="https://piwigo.mysite.com/uploads/myimage.png">
```

Die im Feld „Seitenbanner“ eingerichteten Banner werden je nach Erscheinungsbild Ihrer Galerie etwas unterschiedlich dargestellt.

Sehen wir uns das Ergebnis für jedes Erscheinungsbild an.

### Seitenbanner mit Modus anzeigen

Wenn Sie das Erscheinungsbild Modus verwenden, erscheint das Banner oben auf allen Seiten, wie im Beispiel unten.

![Standard-Banner](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-b6aab97e.jpg)

Wenn das Banner nicht angezeigt wird, gehen Sie in das Menü Konfiguration > Erscheinungsbilder und öffnen die Einstellungen des Erscheinungsbilds Modus. Prüfen Sie, ob die Option „Display page banner“ aktiviert ist.

![Banner anzeigen](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-30eced1f.jpg)

### Seitenbanner mit Bootstrap Darkroom anzeigen

Beim Erscheinungsbild Bootstrap Darkroom werden Seitenbanner standardmässig nicht angezeigt. Um sie anzuzeigen, gehen Sie in das Menü Konfiguration > Erscheinungsbilder und öffnen die Einstellungen des Erscheinungsbilds Bootstrap Darkroom.

Im Feld „Page header“ wählen Sie zwischen drei Anzeigeoptionen für Ihr Banner.

![Banner mit Bootstrap Darkroom anzeigen](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-ea627ac3.jpg)

- Disabled: kein Banner.
- Jumbotron: Der Inhalt aus dem Feld „Seitenbanner“ erscheint oben auf allen Seiten.

![Beispiel Banner Bootstrap Darkroom](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-6878bfe5.jpg)

- Hero image: Mit dieser Option verwenden Sie ein Bild aus Ihrer Piwigo-Galerie als Hintergrund des Banners. Auf Wunsch können Sie dieses Bild in voller Höhe anzeigen. Der Inhalt aus dem Feld „Seitenbanner“ wird mittig darüber eingeblendet.
    
    ![Beispiel Banner mit Bild](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-a55748ff.jpg)
    

### Seitenbanner mit anderen Erscheinungsbildern anzeigen

Die meisten Erscheinungsbilder unterstützen das im Feld „Seitenbanner“ eingerichtete Banner.

Hier einige Beispiele zur Vorschau.

- Anzeige des Banners mit dem Erscheinungsbild Elegant
    
    ![Banner Elegant](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-508d8fec.jpg)
    
- Anzeige des Banners mit dem Erscheinungsbild Simple White
    
    ![Banner Simple White](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-584f14e9.jpg)
    
- Anzeige des Banners mit dem Erscheinungsbild Clear
    
    ![Banner Clear](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-9e42995b.jpg)
    

## Das Plugin Header Manager verwenden

Wenn Sie nach einer umfassenderen Möglichkeit suchen, Ihr Banner zu erstellen, installieren Sie das Plugin **Header Manager**.

In den Einstellungen des Plugins können Sie im Tab „Add a banner“ ein Bild hochladen, das als Banner Ihrer Website dient. Liegt das Bild bereits in Ihrer Galerie, geben Sie stattdessen seine ID ein.

![Plugin Header Manager hinzufügen](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-f0a9ecd7.jpg)

Sobald Sie das Foto ausgewählt haben, können Sie es ganz einfach auf die gewünschte Höhe und Breite zuschneiden.

![Bannerbild zuschneiden](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-bb39679c.jpg)

Im Tab „Configuration“ passen Sie Ihr Banner an:

- nur ein Bild anzeigen
- den Titel Ihrer Galerie über dem Bild anzeigen (als transparenten Text)
- das Bild und einen Text Ihrer Wahl anzeigen

![Banner mit Foto](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-495987f6.jpg)

Mit dem Plugin Header Manager können Sie mehrere Bilder für Ihr Banner verwenden und sie zufällig wechseln lassen.

Sie können sogar für jedes Album ein eigenes Banner festlegen.

Auf der Bearbeitungsseite eines Albums fügt das Plugin nämlich einen Tab „Banner“ hinzu. Dort wählen Sie für das jeweilige Album aus, welches der vorhandenen Banner angezeigt wird.
