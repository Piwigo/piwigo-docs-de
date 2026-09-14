---
title: Schlagworte erstellen und verwalten - Piwigo-Dokumentation
description: In diesem Artikel erfahren Sie, wie Sie in Piwigo Schlagworte erstellen, ordnen und verwenden, um Ihre Fotos und anderen Medien zu indexieren und zu ordnen.
---

# Schlagworte erstellen und verwalten

Schlagworte sind ein unverzichtbares Werkzeug, um Ihre Fotosammlung zu ordnen und die Suche nach Inhalten zu erleichtern. Wie erstellen und ordnen Sie Schlagworte in Piwigo?

## Wie erstelle ich Schlagworte?

Es gibt mehrere Möglichkeiten, Schlagworte zu erstellen. Sie können sie selbst im Administrationsbereich von Piwigo anlegen. Sie können sie auch von Ihrem Computer importieren, wenn Sie Ihre Fotos bereits mit Stichworten ordnen, oder aus einer Software eines Drittanbieters wie Lightroom.

Mehr über den Import von Fotos erfahren Sie [in diesem Artikel](../fotos-importieren-und-verwalten/fotos-in-piwigo-importieren.md).

### Ein Schlagwort im Administrationsbereich erstellen

Um ein Schlagwort zu erstellen, öffnen Sie den Administrationsbereich und klicken links auf das Menü Fotos > Schlagworte.

Sie gelangen zur Schlagwortverwaltung. Dort werden die vorhandenen Schlagworte aufgelistet, und Sie können sie bearbeiten und neue erstellen.

![Liste des tags.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-9178cf82.jpg)

Um ein Schlagwort zu erstellen, klicken Sie auf „Schlagwort hinzufügen“, geben die Bezeichnung des Schlagworts ein und klicken auf die Schaltfläche + oder drücken die Eingabetaste. Das Schlagwort ist nun erstellt.

![Nouveau tag.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-017399c2.jpg)

Sie können ein Schlagwort auch überall dort direkt erstellen, wo Sie einem Foto ein Schlagwort zuweisen können:

- im Foto-Editor
- in der Stapelverarbeitung

### Add tags mass: Eine Liste von Schlagworten gesammelt erstellen

Wenn Sie eine vorhandene Liste von Schlagworten in Ihre Piwigo-Galerie importieren oder schnell mehrere Schlagworte erstellen möchten, aktivieren Sie einfach das Plugin „Add tags mass“.

!!! info "Wenn Sie Kunde von Piwigo Cloud sind, ist dieses Plugin erst ab dem Team-Paket verfügbar"

Nachdem Sie das Plugin aktiviert haben, öffnen Sie seine Konfiguration, um Schlagworte gesammelt hinzuzufügen.

![Ajouter tags en masse.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-f99f9b8e.jpg)

Geben Sie die Schlagworte im Formular einfach nacheinander ein, eines pro Zeile, und klicken Sie auf „Absenden“, um sie zu speichern.

!!! info "Sie können eine Liste von Schlagworten aus einer Tabellenkalkulation (zum Beispiel Excel) kopieren und in dieses Formular einfügen."

### Schlagworte aus Ihren IPTC-Stichworten importieren

Ihre Fotos sind vielleicht bereits mit Stichworten versehen, die Sie in einer Bildbearbeitungssoftware wie Lightroom hinzugefügt haben.

Diese Stichworte sind Teil der IPTC-Metadaten Ihrer Fotos und können als Schlagworte in Piwigo importiert werden.

Das ist standardmässig so eingestellt. Wenn Sie diese Einstellungen ändern möchten und Kunde eines Piwigo-Cloud-Pakets sind, wenden Sie sich an den Support.

!!! warning "Piwigo unterstützt nicht den Import von Schlagworten, die Sie einem Foto im Finder von macOS zuweisen."

## Wie verknüpfe ich Schlagworte mit meinen Fotos?

### Schlagworte im Foto-Editor verknüpfen

Um die Schlagworte eines einzelnen Fotos zu bearbeiten, bearbeiten Sie einfach dieses Foto.

Im Foto-Editor können Sie einem Foto über das Feld „Schlagworte“ ein oder mehrere Schlagworte hinzufügen.

[Mehr über das Bearbeiten von Fotos erfahren](../fotos-importieren-und-verwalten/fotos-bearbeiten-oder-loeschen.md)

Wenn Sie in das Eingabefeld klicken, erscheint die Auswahlliste der Schlagworte. Um nach einem bestimmten Schlagwort zu suchen, geben Sie einfach einige Zeichen ein: Die Liste wird sofort aktualisiert und zeigt nur noch die Schlagworte an, die zu Ihrer Eingabe passen.

![Ajouter un tag.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-b80f5e81.jpg)

Klicken Sie auf ein Schlagwort, um es mit Ihrem Foto zu verknüpfen: Es erscheint nun in Orange.

![Tag Espagne.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-87cd4f9d.jpg)

Um ein Schlagwort von dem gerade bearbeiteten Foto zu entfernen, klicken Sie auf das Kreuz neben dem Namen des Schlagworts. Das Schlagwort wird dadurch nicht aus Ihrer Fotosammlung gelöscht: Sie können es weiterhin für andere Fotos verwenden.

So können Sie Ihrem Foto nach und nach mehrere Schlagworte zuweisen.

Wenn Sie ein neues Schlagwort erstellen möchten, geben Sie einfach seinen Namen in das Eingabefeld ein. Die Option „Create ...“ erscheint: Klicken Sie darauf oder drücken Sie die Eingabetaste, um ein neues Schlagwort zu erstellen.

![Création de tag.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-4fae74ae.jpg)

!!! info "Denken Sie daran, Ihre Änderungen zu speichern, damit sie für Ihr Foto übernommen werden!"

### Schlagworte mit der Stapelverarbeitung gesammelt mit Fotos verknüpfen

In der Regel ist es besser, Fotos gesammelt zu verschlagworten, statt jedes Foto einzeln zu bearbeiten:

- entweder nach dem Import eines Stapels von Fotos in Piwigo
- oder um eine Liste von Fotos zu aktualisieren, die einem Kriterium entsprechen (Fotos eines Albums, Auswahl von Fotos in Ihrem Sammelkorb...)

Das geht ganz einfach mit der [Stapelverarbeitung](../fotos-importieren-und-verwalten/stapelverarbeitung.md).

Nachdem Sie Ihre Auswahl getroffen haben, können Sie die Aktion „Schlagworte hinzufügen“ wählen. Damit weisen Sie einem Stapel von Fotos vorhandene Schlagworte oder ein neu erstelltes Schlagwort zu.

In der Übersicht:

![Gestion lot créer tag.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-f5389291.jpg)

Im Einzelmodus:

![Créer tag gestion lot.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-13540705.jpg)

### Schlagworte mit der Stapelverarbeitung gesammelt von Fotos entfernen

Mit der Stapelverarbeitung können Sie auch Schlagworte von einer Liste von Fotos entfernen.

Wählen Sie dazu die Aktion „Schlagworte entfernen“ und wählen Sie die Schlagworte aus, die der Auswahl von Fotos nicht mehr zugewiesen sein sollen.

Die Schlagworte werden dadurch nicht aus Ihrer Fotosammlung gelöscht: Sie können sie weiterhin für andere Fotos verwenden.

## Schlagworte verwalten und bearbeiten

Um Schlagworte in Ihrer Fotosammlung zu verwalten, zu bearbeiten und zu löschen, öffnen Sie die Schlagwortverwaltung über das Menü Fotos > Schlagworte.

![Nouvelle liste de tags.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-ffa4fc28.jpg)

Mit einer Suchfunktion finden Sie ein Schlagwort ganz einfach: praktisch, wenn Sie sehr viele davon haben!

Wenn Sie auf die 3 Punkte neben einem Schlagwort klicken, sehen Sie die Anzahl der Fotos, die mit diesem Schlagwort verknüpft sind, sowie eine Liste der verfügbaren Aktionen.

![Actions tags.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-0dfe098a.jpg)

- Galerie-Ansicht: zeigt alle Fotos, die mit diesem Schlagwort verknüpft sind, in Ihrer Piwigo-Galerie an
- Fotos verwalten: Sie können die mit diesem Schlagwort verknüpften Fotos in der Stapelverarbeitung verwalten und bearbeiten
- Bearbeiten: Sie können das Schlagwort umbenennen
- Duplikat: erstellt eine Kopie des Schlagworts
- Löschen: Sie können das Schlagwort löschen

### Schlagworte gesammelt bearbeiten: der Auswahlmodus

Um eine Liste von Schlagworten gesammelt zu bearbeiten, wechseln Sie in den Auswahlmodus, indem Sie rechts auf dem Bildschirm auf die Schaltfläche „Auswahlmodus“ klicken.

Mit dieser Funktion können Sie:

- eine Liste von Schlagworten gesammelt löschen
- Schlagworte zusammenführen (praktisch bei Duplikaten)

Klicken Sie auf die Schlagworte, die Sie bearbeiten möchten: Sie erscheinen nacheinander in einer Liste rechts auf dem Bildschirm.

![Sélection de tags.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-126c5057.jpg)

Falls Sie sich vertan haben, können Sie ein Schlagwort aus der Auswahlliste entfernen, indem Sie auf das Kreuz neben seinem Namen klicken.

![Supprimer tag sélection.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-ef71c1cd.jpg)

Mit den Schaltflächen „Alles“, „Nichts“ und „Invertieren“ oben auf dem Bildschirm geht die Auswahl schneller, wenn Sie viele Schlagworte bearbeiten möchten.

- Ein Klick auf „Alles“ fügt alle Schlagworte auf dem Bildschirm Ihrer Auswahlliste hinzu
- Ein Klick auf „Nichts“ leert Ihre Auswahlliste
- Ein Klick auf „Invertieren“ fügt alle Schlagworte der Auswahl hinzu, ausser denen, die gerade ausgewählt sind.

Wenn Sie mit der Auswahl fertig sind, klicken Sie auf die gewünschte Aktion:

- Zusammenführen: Alle ausgewählten Schlagworte werden zu einem einzigen zusammengeführt (Sie wählen aus, welcher Name erhalten bleibt)
- Löschen: Alle ausgewählten Schlagworte werden gelöscht.

## Lesen Sie auch: Schlagworte in Ihrer Galerie

In diesem Artikel erfahren Sie, wie Sie Schlagworte in Ihrer Galerie verwenden, sowie Optionen und Plugins, mit denen Sie noch mehr aus Schlagworten herausholen.

[Schlagworte in Ihrer Galerie](../ihre-piwigo-galerie-erkunden/schlagworte-in-ihrer-galerie.md)
