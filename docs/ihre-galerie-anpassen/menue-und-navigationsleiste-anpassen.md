---
title: Menü anpassen - Piwigo-Dokumentation
description: Wie passen Sie die Navigationsleiste Ihrer Piwigo-Galerie an, ändern die Baumstruktur und fügen neue Menüpunkte hinzu? Das erklären wir in diesem Artikel.
---

# Menü Ihrer Galerie anpassen

Wie passen Sie die Menüleiste Ihrer Galerie an, ändern die Baumstruktur und fügen neue Menüpunkte hinzu? Das erklären wir Ihnen in diesem Artikel.

## Das Standardmenü von Piwigo

Alle Galerien werden standardmässig mit demselben Navigationsmenü erstellt. Mit **dem Menü** sind die Links gemeint, die in der Leiste oben auf allen Seiten der Galerie angezeigt werden.

![Das Navigationsmenü mit dem Erscheinungsbild Modus](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-19542d3a.jpg)

Das Navigationsmenü mit dem Erscheinungsbild Modus

![Das Navigationsmenü mit Bootstrap Darkroom](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-edcd40fb.jpg)

Das Navigationsmenü mit Bootstrap Darkroom

An den Beispielen oben sehen Sie:

- dass die angezeigten Menüpunkte je nach Erscheinungsbild Ihrer Galerie unterschiedlich sind;
- dass das Menü davon abhängt, ob man als Benutzer angemeldet ist oder nicht.

Einige Menüpunkte öffnen eine Liste mit Untermenüs:

- Der Link „Alben“ zeigt die Liste der Alben mit der Anzahl der enthaltenen Fotos.
- Das Menü „Schlagworte“ zeigt die Liste der Schlagworte und ermöglicht die Suche nach Fotos per Schlagwort.
- Das Menü „Erkunden“ (bei Modus) bzw. „Entdecken“ (bei Bootstrap Darkroom) enthält viele Untermenüs.

![Zusätzliches Menü](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-4cf49a38.jpg)

## Das Menü anpassen: grundlegende Optionen

Um das Navigationsmenü Ihrer Galerie anzupassen, gehen Sie im Administrationsbereich in das Menü Konfiguration > Menü.

Auf dieser Seite sehen Sie die Links im Menü, können sie neu anordnen und einige davon ausblenden.

![Liste der Menüs](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-82955015.jpg)

Es ist wichtig zu verstehen, wofür jede Zeile auf dieser Seite steht:

- Die Zeile „Erweitert“ steht für eine Liste von Links, die beim Klick auf den Menüpunkt „Erkunden“ bei Modus bzw. „Entdecken“ bei Bootstrap Darkroom erscheint. Folgende Seiten gehören zu „Erweitert“:
    - Meine Favoriten (für angemeldete Benutzer)
    - Am häufigsten angesehen
    - Am besten bewertet
    - Neueste Fotos
    - Neueste Alben
    - Zufällige Fotos
    - Kalender

![Die Blöcke „Menü“ und „Erweitert“ in einer Galerie mit dem Erscheinungsbild Modus](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-8461e87c.jpg)

Die Blöcke „Menü“ und „Erweitert“ in einer Galerie mit dem Erscheinungsbild Modus

- Die Zeile „Menü“ steht für eine weitere Liste von Links, die beim Klick auf den Menüpunkt „Erkunden“ bei Modus bzw. „Entdecken“ bei Bootstrap Darkroom erscheint. Der Block „Menü“ enthält folgende Links:
    - Schlagworte
    - Suchen
    - Kommentare
    - RSS-Feed
- Die Zeile „Verwandte Alben“ wird nur auf einer Fotoseite angezeigt
- Die Zeile „Links“ steht für externe Links, die in der Konfiguration von Piwigo hinzugefügt werden können (mit [LocalFiles Editor](../piwigo-selbst-hosten/lokale-konfiguration-bearbeiten-localfiles-editor.md), wenn Sie Ihre Piwigo-Galerie selbst hosten, oder mit dem Plugin [Advanced Menu Manager](menue-und-navigationsleiste-anpassen.md))

Um die Reihenfolge der Menüpunkte zu ändern, verschieben Sie sie einfach per Drag-and-drop und speichern die Einstellungen.

![Menüliste ändern](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-47022628.gif)

Wenn Sie ein Element im Menü ausblenden möchten, aktivieren Sie „Ausblenden“.

## Das Menü mit Plugins anpassen

Mit mehreren Plugins können Sie Ihr Menü noch weiter anpassen.

### Advanced Menu Manager: erweiterte Menüanpassung

Das Plugin Advanced Menu Manager bietet zusätzliche Optionen, um Ihr Navigationsmenü anzupassen. Öffnen Sie nach der Aktivierung die Konfigurationsseite des Plugins.

Dort stehen Ihnen 5 Tabs zur Verfügung.

**Tab „Menu management“**

Wie die Menü-Konfigurationsseite im Administrationsbereich ermöglicht Ihnen dieser Tab, die Menüpunkte per Drag-and-drop neu anzuordnen. Ausserdem können Sie die Sichtbarkeit einiger Menüpunkte je nach Benutzer festlegen:

- nach [Benutzerstatus](../benutzer-verwalten/benutzerstatus.md) in der linken Spalte (Administrator, Webmaster, Besucher, Gast…)
- nach [Benutzergruppe](../benutzer-verwalten/benutzergruppen.md) in der rechten Spalte

![Plugin Advanced Menu Manager](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-2e2eff09.jpg)

Im selben Tab können Sie mit einem Klick auf „Content for 'Menu' & 'Specials' menus“ die Seiten anpassen, die in den Blöcken „Menü“ und „Erweitert“ angezeigt werden (siehe vorheriger Abschnitt).

![Plugin Advanced Menu Manager, weiteres Menü](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-95b63dc2.jpg)

Auf dieser Seite können Sie also die Links in diesen beiden Menüblöcken neu anordnen. Mit einem Klick auf das Schloss legen Sie ausserdem die Sichtbarkeit dieser Links nach Benutzerstatus und Benutzergruppe fest.

**Tab „Links“**

In diesem Tab fügen Sie externe Links hinzu, die in die Gruppe „Links“ eingefügt werden (zum Beispiel, wenn Sie in Ihrer Galerie einen Link zu Ihrer Website einbinden möchten).

Hier können Sie:

- einen oder mehrere externe Links hinzufügen
- den in Ihrer Galerie angezeigten Menüpunkt „Links“ umbenennen
- weitere Optionen bearbeiten

**Tab „Random picture“**

Das Plugin Advanced Menu Manager fügt Ihrer Galerie den Menüpunkt „A random picture“ hinzu. Wenn man mit der Maus darüberfährt, wird ein zufällig ausgewähltes Bild angezeigt.

![Zufälliges Bild](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-4997c09f.jpg)

Im Tab „Random picture“ passen Sie den Titel dieses Blocks im Menü und die angezeigten Daten an. Ausserdem können Sie festlegen, dass dieser Block nur in bestimmten Alben sichtbar ist.

**Tab „Personalized menu“**

In diesem Tab fügen Sie dem Menü beliebige Menüpunkte hinzu.

**Tab „Album ⇒ Menu“**

In diesem Tab erstellen Sie Menüpunkte aus einem Album.

Das ist praktisch, wenn Sie ein bestimmtes Album im Navigationsmenü hervorheben möchten.

### RV Menu Tree: Durch die Albumstruktur navigieren

Das Plugin RV Menu Tree verändert die Funktionsweise des Menüpunkts „Alben“ in Ihrer Galerie.

Damit können Sie durch die Baumstruktur der Unteralben navigieren, was standardmässig nicht möglich ist.

![Menü „Alben“ mit dem Standard-Erscheinungsbild Modus](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-bca5c267.jpg)

Menü „Alben“ mit dem Standard-Erscheinungsbild Modus

![Menü „Alben“ mit dem Erscheinungsbild Modus UND RV Menu Tree](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-139dbda1.jpg)

Menü „Alben“ mit dem Erscheinungsbild Modus UND RV Menu Tree

### See my photos: Ein Menü „Meine Fotos“ hinzufügen

Das Plugin **See My Photos** fügt der Galerie im Block „Erweitert“ den Menüpunkt „Meine Fotos“ hinzu.

!!! info "Wenn Sie Kunde von Piwigo Cloud sind, ist dieses Plugin erst ab dem Tarif Team verfügbar."

Über diesen Link sehen Benutzer alle Fotos, die sie selbst in Piwigo importiert haben. Das ist besonders nützlich, wenn Sie das Plugin [Community](../benutzer-verwalten/mitwirkende-community-plugin.md) verwenden.

### See photos by user: Ein Menü „Benutzer“ hinzufügen

Mit dem Plugin **See photos by user** können Besucher der Galerie Fotos ganz einfach nach dem Benutzer filtern, der sie hinzugefügt hat.

!!! info "Wenn Sie Kunde von Piwigo Cloud sind, ist dieses Plugin erst ab dem Tarif Team verfügbar."

Auf der Konfigurationsseite des Plugins im Administrationsbereich können Sie die Einstellungen verfeinern:

- Mindestanzahl an Fotos, ab der ein Benutzer in der Galerie angezeigt wird
- maximale Anzahl der Benutzer, die auf der Seite angezeigt werden
- Reihenfolge der Benutzer auf der Seite (alphabetisch, nach Anzahl der Fotos…)
- Position der Seite in der Galerie:
    - Menü „See photos by user“ unter dem Menü „Erkunden“
    - oder ein Menü „Benutzer“ im Hauptmenü, mit einem Untermenü für jeden Benutzer
- Methode zum Filtern nach Benutzern in der Galerie:
    - klassische Benutzerwolke anzeigen
    - animierte und farbige Benutzerwolke anzeigen
    - Dropdown-Liste der Benutzer anzeigen

Unten sehen Sie ein Beispiel für eine Seite „Benutzer“ mit dem Menü „Benutzer“ und der klassischen Benutzerwolke als Anzeigeoption.

![Fotos nach Benutzer anzeigen](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-00e893c3.jpg)

!!! info "Dieses Plugin ist nur teilweise mit dem Erscheinungsbild Bootstrap Darkroom kompatibel."

### Menu Random Photo: Ein zufälliges Foto hinzufügen

Das Plugin **Menu Random Photo** fügt einen Menüpunkt hinzu, der ein zufällig ausgewähltes Bild aus Piwigo anzeigt.

![Plugin Menu Random Photo](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-500bc174.jpg)

Diese Funktion ist auch im Plugin Advanced Menu Manager enthalten.

### Menu Tags

Das Plugin **Menu Tags** fügt auf allen Seiten ohne zugehörige Schlagworte ein Menü „Schlagworte“ hinzu.

Wenn Sie dieses Plugin aktivieren, wird auf der Seite eines Albums weiterhin das Menü mit den zugehörigen Schlagworten angezeigt (es zeigt nur die Schlagworte der Fotos dieses Albums).

Auf der Startseite erscheint dagegen statt des Menüs mit den zugehörigen Schlagworten ein Menü „Schlagworte“. Es zeigt alle Schlagworte Ihrer Galerie in einer Grösse, die ihrer Häufigkeit entspricht.

![Plugin Menu Tags](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-0238d1ec.jpg)

[Mehr über Schlagworte in Ihrer Galerie erfahren](../ihre-piwigo-galerie-erkunden/schlagworte-in-ihrer-galerie.md)

### Upload 1 Menu: Ein Menü „Fotos hinzufügen“ hinzufügen

!!! info "Wenn Sie Kunde von Piwigo Cloud sind, ist dieses Plugin erst ab dem Tarif Team verfügbar."

Wenn das Plugin [Community](../benutzer-verwalten/mitwirkende-community-plugin.md) aktiviert ist, zeigt das Plugin **Upload 1 Menu** das Menü „Fotos hinzufügen“ im Hauptmenü der Galerie neben dem Menü „Erkunden“ an.

![Plugin Upload 1 Menu](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-55e5277b.jpg)
