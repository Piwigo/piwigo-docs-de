---
title: In Ihrer Galerie suchen - Piwigo-Dokumentation
description: Wie suchen Sie ein Foto in Ihrer Piwigo-Galerie? Wie funktioniert die Suche mit mehreren Kriterien? Das sehen wir uns in diesem Artikel an.
---

# Ein Foto in Ihrer Galerie suchen

Für die Suche in Ihrer Piwigo-Galerie stehen Ihnen mehrere Möglichkeiten zur Verfügung: eine einfache Schnellsuche nach einem Suchbegriff oder eine Suche mit mehreren Kriterien, bei der Sie verschiedene Filter kombinieren.

In diesem Artikel erklären wir alles!

## Die Schnellsuche

### Das Feld der Schnellsuche verwenden

Wenn diese Funktion in Ihrer Galerie aktiv ist (bei den meisten Erscheinungsbildern ist das standardmässig der Fall), steht Ihnen ein Suchfeld zur Verfügung.

![Recherche.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-93100bee.jpg)

Bei manchen Erscheinungsbildern erreichen Sie die Suche über einen Menüpunkt (unten ein Beispiel mit der Standardkonfiguration des Erscheinungsbilds Bootstrap Darkroom).

![Recherche BD.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-09d801d5.jpg)

Geben Sie einen Begriff in die Schnellsuche ein und drücken Sie die Eingabetaste: Die Ergebnisse zeigen die Fotos, die zu Ihrer Suche passen.

![Résultats recherche.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-5675caaa.jpg)

Standardmässig sucht Piwigo den eingegebenen Begriff an folgenden Stellen, um die Ergebnisse zu filtern:

- im Namen (Titel) des Fotos in Piwigo
- im Dateinamen
- in der Beschreibung der Datei
- in den Schlagworten, die Ihren Fotos zugeordnet sind
- in der ID der Fotos

Wenn der eingegebene Begriff einem Schlagwort oder dem Namen eines Albums in Ihrer Galerie entspricht, erscheinen diese ausserdem in den Ergebnissen. Klicken Sie auf die Schaltfläche „Gefundene Tags“ oder „Gefundene Alben“, um die Liste der Schlagworte bzw. Alben zu sehen, die zu Ihrer Suche passen.

![Trouvailles.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-99ff55de.jpg)

### Eine Schnellsuche bearbeiten oder verfeinern

Seit Piwigo 14 erscheint bei jeder Schnellsuche eine Filterleiste über den Suchergebnissen. Im nächsten Kapitel gehen wir genauer darauf ein. Mit dieser Filterleiste können Sie Ihre Suche mit weiteren Kriterien verfeinern (Schlagwort, Album, Autor…).

Über die Filterleiste können Sie auch die aktuelle Suche bearbeiten. Klicken Sie dazu einfach auf den Bereich, der Ihren Suchbegriff anzeigt. Daraufhin öffnet sich ein Fenster.

![Recherche mots.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-899a93ba.jpg)

In diesem Fenster können Sie:

- den Inhalt Ihrer Suche bearbeiten;
- nach mehreren Begriffen suchen und dabei festlegen, ob alle Begriffe oder nur einer davon vorkommen müssen;
- festlegen, wo Piwigo sucht (zum Beispiel, indem Sie die Suche in den Fotobeschreibungen deaktivieren).

### RV Autocomplete: Automatische Vervollständigung für die Schnellsuche aktivieren

Möchten Sie bei der Suche nach einem Schlagwort oder einem Album in Ihrer Galerie noch mehr Zeit sparen?

Dann empfehlen wir Ihnen das Plugin **RV Autocomplete**.

Sobald das Plugin aktiviert ist, werden Ihnen bei der Eingabe eines Suchbegriffs automatisch die passenden Alben und Schlagworte vorgeschlagen.

![RV Autocomplète.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-8b1e3150.jpg)

## Die Suchfilter für mehrere Kriterien

### Eine Suche mit mehreren Kriterien starten

Seit Piwigo 14 ist die frühere erweiterte Suche durch eine Filterleiste ersetzt.

![Recherche début.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-4cb2eef4.jpg)

Es gibt mehrere Möglichkeiten, eine Suche zu starten:

- Über das Formular der Schnellsuche (im vorherigen Kapitel erklärt): Anschliessend können Sie Ihre Suche mit den Filtern verfeinern oder zurücksetzen.
- Über das Menü Erkunden > Suchen (Erscheinungsbild Modus) bzw. Entdecken > Suchen (Erscheinungsbild Bootstrap Darkroom), das die Suchseite anzeigt.
- Auf der Seite eines Albums oder eines Schlagworts über die Schaltfläche oder das Symbol „In dieser Gruppe suchen“ (sofern diese Schaltfläche in Ihrer Galerie aktiviert ist).

### Die angezeigten Filter auswählen

Die Filterleiste zeigt standardmässig 4 Filter an:

- Suche nach Begriffen (funktioniert wie die Schnellsuche)
- Filter nach Schlagwort
- Filter nach Album
- Filter nach Autor

![Filtres.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-09c3a22e.jpg)

Mit einem Klick auf „Filter wählen“ können Sie weitere Kriterien hinzufügen:

- Veröffentlichungsdatum (Datum, an dem die Datei in Piwigo hochgeladen wurde)
- Aufnahmedatum (Datum, an dem die Datei erstellt wurde)
- Hinzugefügt von (Benutzer, der die Datei hochgeladen hat)
- Dateityp (Dateiendung: JPG, PNG…)
- Verhältnis (Hochformat, quadratisch, Querformat…)
- Dateigrösse (in Bytes)
- Höhe (in Pixeln)
- Breite (in Pixeln)

![image.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-5c14739d.png)

Klicken Sie einfach auf ein Kriterium, um es der Filterleiste hinzuzufügen oder daraus zu entfernen, und speichern Sie. Die gewählten Kriterien werden hinzugefügt. Ihre Auswahl der sichtbaren Filter wird gespeichert, gilt aber nur für Ihren Benutzer.

![image.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-0c0eebd1.png)

### Fotos mit Filtern finden

**Suche nach Begriffen**

Dieser Filter funktioniert genau wie die Schnellsuche.

Sie können einen oder mehrere Begriffe eingeben, festlegen, ob die Ergebnisse alle Begriffe oder nur einen davon enthalten sollen, und wählen, wo nach dem eingegebenen Begriff gesucht wird (im Titel des Fotos, im Dateinamen, in der Beschreibung…).

![Recherche de mots.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-d982afdb.jpg)

Mit den beiden Schaltflächen „Löschen“ deaktivieren Sie den Filter bzw. setzen ihn zurück.

**Suche nach Schlagwort**

Mit dem Filter „Schlagwort“ zeigen Sie die Fotos an, denen ein oder mehrere Schlagworte zugeordnet sind.

Sie können festlegen, ob die Suche Fotos finden soll, denen alle ausgewählten Schlagworte zugeordnet sind, oder nur mindestens eines davon.

Wenn Sie in das Suchfeld klicken, erscheint eine Auswahlliste mit allen Schlagworten. Darin finden Sie das gewünschte Schlagwort, indem Sie die ersten Buchstaben eintippen.

![Recherche tags.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-8e5721b0.jpg)

Mit den beiden Schaltflächen „Löschen“ deaktivieren Sie den Filter bzw. setzen ihn zurück.

**Suche nach Veröffentlichungsdatum und Aufnahmedatum**

Mit dem Filter „Veröffentlichungsdatum“ filtern Sie Fotos nach dem Datum, an dem sie in Piwigo importiert wurden, mit dem Filter „Aufnahmedatum“ nach dem Datum, an dem die Datei erstellt wurde.

Mehrere Zeiträume stehen zur Auswahl: letzte 7 Tage, letzte 30 Tage, letzte 3 Monate… Zu jedem Zeitraum wird auch die Anzahl der passenden Fotos angezeigt. Nicht zutreffende Filter sind ausgegraut.

![image.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-5e047136.png)

Sie können auch auf „Benutzerdefinierte Daten“ klicken, um nach einem oder mehreren Zeiträumen Ihrer Wahl zu filtern. Das kann ein Jahr, ein Monat, ein Tag… oder eine Kombination davon sein.

![image.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-16beb8ca.png)

Mit den beiden Schaltflächen „Löschen“ deaktivieren Sie den Filter bzw. setzen ihn zurück.

**Suche nach Album**

Mit dem Filter „Album“ suchen Sie Fotos in einem oder mehreren Alben, wahlweise mit oder ohne Unteralben.

![filters-album.gif](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-800f9b4f.gif)

Mit den beiden Schaltflächen „Löschen“ deaktivieren Sie den Filter bzw. setzen ihn zurück.

**Suche nach Autor**

Mit dem Filter „Autor“ suchen Sie ein Foto nach seinem Autor. Wählen Sie dazu einen Autor aus der Auswahlliste der vorhandenen Autoren.

![Auteurs.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-c1cb3753.jpg)

Mit den beiden Schaltflächen „Löschen“ deaktivieren Sie den Filter bzw. setzen ihn zurück.

**Suche nach „Hinzugefügt von“ (Benutzer, der die Datei importiert hat)**

Der Filter „Hinzugefügt von“ listet die Benutzer auf, die Dateien in Ihre Piwigo-Galerie importiert haben, und filtert die Suchergebnisse entsprechend. Zu jedem Benutzer wird die Anzahl seiner Fotos angezeigt.

![image.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-611a803e.png)

Mit den beiden Schaltflächen „Löschen“ deaktivieren Sie den Filter bzw. setzen ihn zurück.

**Suche nach Dateityp (Format)**

Mit dem Filter „Dateityp“ filtern Sie die Ergebnisse nach Format (bzw. Dateiendung).

![image.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-e0b760d0.png)

**Suche nach Seitenverhältnis**

Mit dem Filter „Verhältnis“ filtern Sie Dateien nach ihrem Seitenverhältnis. Piwigo erkennt mehrere Seitenverhältnisse: Hochformat, quadratisch, Querformat, Panorama.

![image.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-0eb533ad.png)

**Suche nach Dateigrösse**

Mit dem Filter „Dateigrösse“ filtern Sie Dateien nach einer minimalen und/oder maximalen Dateigrösse in MB. Klicken Sie auf die Skala, um den Regler zu verschieben.

![image.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-e57b0a39.png)

**Suche nach Höhe / Breite**

Mit den Filtern „Höhe“ und „Breite“ filtern Sie Dateien nach einer minimalen und/oder maximalen Höhe bzw. Breite in Pixeln. Klicken Sie auf die Skala, um den Regler zu verschieben.

![image.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-ec54877f.png)

### Mehrere Filter kombinieren

Die Stärke dieser Suchfunktion liegt darin, dass Sie mehrere Filter kombinieren können und die Ergebnisse sofort aktualisiert werden.

Sie können jederzeit einen Filter hinzufügen oder entfernen, die Kriterien ändern und Ihre Suche verfeinern, wie in der folgenden Animation zu sehen ist.

![filters.gif](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-81aec1aa.gif)

### Ein Foto in einer Gruppe suchen (Album oder Schlagwort)

Auf der Seite eines Albums oder eines Schlagworts können Sie eine Schaltfläche oder ein Symbol anzeigen lassen, mit dem Sie eine Suche innerhalb dieser Gruppe von Fotos starten.

Die Schaltfläche „In dieser Gruppe suchen“:

![Recherche lot.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-12c769f9.jpg)

Das Symbol „In dieser Gruppe suchen“ in der Werkzeugleiste der Albumseite:

![icone-lot.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-9d25876d.png)

Klicken Sie auf diese Schaltfläche, um die Suchfilter auf der aktuellen Seite anzuzeigen.

Um diese Schaltfläche und dieses Symbol in Ihrer Galerie ein- oder auszublenden, öffnen Sie im Administrationsbereich das Menü Konfiguration > Optionen und dort den Tab „Anzeige“.

![Configuration.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-bc617af1.jpg)

## Mit verwandten Schlagworten suchen

Wenn Ihre Fotos sorgfältig mit Schlagworten versehen sind, ist die Suche nach Schlagworten ein sehr wirkungsvolles Mittel, um ein Foto zu finden. Sie können ein Foto nicht nur über die Suchfunktion nach Schlagwort suchen, sondern auch die Schlagworte durchstöbern, etwa über die Funktion „Verwandte Schlagworte“ oder eine Schlagwortwolke.

Mehr dazu erfahren Sie in diesem Artikel: [Schlagworte in Ihrer Galerie](schlagworte-in-ihrer-galerie.md)
