---
title: Die Fotoseite in Ihrer Galerie - Piwigo-Dokumentation
description: Wie die Fotoseite in Ihrer Piwigo-Galerie funktioniert und wie Sie sie anpassen, erfahren Sie in diesem Artikel!
---

# Die Fotoseite in Ihrer Galerie

Sobald Sie in der Piwigo-Galerie eine Datei (ein Bild oder eine andere Datei) öffnen, ob über ein Album, eine Suche oder auf anderem Weg, gelangen Sie auf die Fotoseite.

Auf dieser Seite sehen Sie ein Foto und seine Details und können verschiedene Aktionen mit dieser Datei ausführen.

In diesem Artikel erfahren Sie, wie die Fotoseite aufgebaut ist, welche Funktionen es gibt und wie Sie sie standardmässig oder mit Plugins anpassen können.

!!! note "Hinweis"
    Die meisten Screenshots in diesem Artikel zeigen eine Galerie mit dem Erscheinungsbild Modus. Je nach Erscheinungsbild Ihrer Galerie werden Informationen und Symbole nicht unbedingt gleich dargestellt.

## Aufbau der Fotoseite

Unabhängig vom Erscheinungsbild Ihrer Galerie enthält die Fotoseite immer dieselben Elemente, zusätzlich zum Menü und zur Fusszeile, die auf jeder Seite angezeigt werden:

- eine Brotkrumennavigation, die zeigt, wo sich das Foto in der Albumstruktur befindet, und mit der Sie durch diese Struktur navigieren können;
- eine Werkzeugleiste mit Symbolen, über die Sie bestimmte Aktionen mit dem Foto ausführen können;
- Navigationspfeile, mit denen Sie innerhalb des Albums von Foto zu Foto blättern;
- die Informationen zum Foto (Eigenschaften, Metadaten);
- das Foto selbst (gegebenenfalls mit seiner Beschreibung);
- einen Kommentarbereich (wenn Kommentare in der Galerie aktiviert sind).

Unten sehen Sie den Aufbau der Fotoseite mit dem Standard-Erscheinungsbild (Modus).

![Page photo fini.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-fe68b5d6.jpg)

Wenn Sie ein anderes Erscheinungsbild verwenden, zum Beispiel Bootstrap Darkroom, ist die Seite anders aufgebaut, enthält aber dieselben Elemente.

![Jolie petite maison.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-9f7d9c10.jpg)

### Mit den Pfeilen navigieren

Auf der Fotoseite können Sie mit pfeilförmigen Symbolen durch eine Auswahl von Fotos blättern.

Mit dem Erscheinungsbild Modus befinden sich diese Pfeile oben rechts auf der Seite.

![Flèches.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-8206f097.jpg)

Welche Fotos zur Auswahl gehören, hängt davon ab, über welchen Weg Sie zum Foto gelangt sind:

- Kommen Sie von der Albumseite, blättern Sie mit den Pfeilen durch alle Fotos des Albums;
- Haben Sie auf ein Schlagwort geklickt, blättern Sie durch alle Fotos mit demselben Schlagwort;
- Kommen Sie von einer Suche, blättern Sie durch die Suchergebnisse;
- usw.

Mit dem linken und dem rechten Pfeil gelangen Sie zum nächsten bzw. zum vorherigen Foto.

Mit dem Pfeil nach oben kehren Sie zur vorherigen Seite zurück (Album, Schlagwort, Suche usw.).

### Eigenschaften und Metadaten

Die Fotoseite zeigt einige Eigenschaften und Metadaten Ihrer Datei an.

Mit dem Erscheinungsbild Modus erscheint dieser Bereich rechts neben dem Foto.

![Description.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-fd9b02f9.jpg)

Wenn Sie mehr über Eigenschaften und Metadaten erfahren möchten, zum Beispiel:

- wie Sie festlegen, welche davon in Ihrer Galerie angezeigt werden
- wie Sie die Reihenfolge der Eigenschaften festlegen
- wie Sie die Metadaten ein- oder ausblenden
- wie Sie eigene Eigenschaften erstellen
- usw.

Lesen Sie [den Artikel über Eigenschaften und Metadaten](../fotos-importieren-und-verwalten/eigenschaften-und-metadaten-von-fotos.md).

### Kommentare

Wenn Sie Kommentare in Ihrer Galerie aktiviert haben, wird auf der Fotoseite ein Kommentarbereich angezeigt.

Mehr dazu lesen Sie im [Artikel über die Verwaltung von Kommentaren](../kommentare-und-bewertungen/kommentare-verwalten.md).

### Verfügbare Aktionen für ein Foto

Über die Werkzeugleiste erreichen Sie verschiedene Funktionen.

![Untitled](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-036c3e5c.png)

**Die Grösse des angezeigten Fotos ändern**

Mit dem ersten Symbol wählen Sie, in welcher der in der Galerie verfügbaren Grössen das Foto angezeigt wird.

![Tailles photos.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-48bf7fe5.jpg)

Wie Sie die in der Galerie verfügbaren Bildgrössen festlegen, erfahren Sie im Kapitel [Die verfügbaren Dateigrössen in Ihrer Galerie verwalten.](die-fotoseite-in-ihrer-galerie.md)

**Eine Diashow starten**

Mit dem Wiedergabe-Symbol starten Sie eine Diashow im Vollbildmodus, die durch die Fotos Ihrer Auswahl blättert.

![Diaporama.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-a372817c.jpg)

**Metadaten anzeigen**

Mit dem Symbol in Form einer Kamera blenden Sie die Metadaten Ihres Fotos im seitlichen Eigenschaftenbereich ein oder aus. Mehr über das [Anzeigen der Metadaten](../fotos-importieren-und-verwalten/eigenschaften-und-metadaten-von-fotos.md)

**Das Foto herunterladen**

Mit dem Symbol in Form einer Diskette laden Sie das Foto auf Ihren Computer herunter.

Standardmässig wird das Original heruntergeladen.

Wenn Sie das Plugin **Download by Size** aktiviert haben, muss der Benutzer vorher die Grösse des Fotos wählen, das er herunterlädt.

![Télécharger tailles.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-44796342.jpg)

Ist das Benutzerrecht „Download erlauben“ in Ihrem Profil deaktiviert, steht die Originalversion des Fotos nicht zur Verfügung. Sie sehen nur die Grössen, die in Ihrer Galerie freigegeben wurden. So können Sie, wenn Sie möchten, in Ihrer Galerie nur Versionen Ihrer Fotos mit niedriger Auflösung anzeigen.

Wenn Sie die Schaltfläche zum Herunterladen in Ihrer Galerie ganz ausblenden möchten, gehen Sie im Administrationsbereich auf Konfiguration > Optionen, dann auf die Registerkarte „Anzeige“ und in den Abschnitt „Fotoseite“. Entfernen Sie dort das Häkchen bei *Symbol »Datei herunterladen« anzeigen*.

**Das Foto zu den Favoriten hinzufügen**

Mit dem Symbol in Form eines Herzens fügen Sie das Foto zu Ihren Favoriten hinzu. Ihre Favoriten finden Sie auf der Seite „Meine Favoriten“ im Menü „Erkunden“ (bzw. „Entdecken“, wenn Sie das Erscheinungsbild Bootstrap Darkroom verwenden). [Mehr über Favoriten erfahren](favoriten-verwalten.md)

**Das Foto als Album-Vorschaubild festlegen (nur für Administratoren)**

Das Symbol in Form eines Pokals ist nur für Administratoren sichtbar. Damit legen sie das aktuelle Foto als Vorschaubild fest, das das Album repräsentiert.

**Das Foto bearbeiten (nur für Administratoren)**

Das Symbol in Form eines Stifts ist nur für Administratoren sichtbar. Damit öffnen sie im Administrationsbereich von Piwigo die Bearbeitungsseite des aktuellen Fotos.

**Das Foto in den Sammelkorb legen (nur für Administratoren)**

Das Symbol in Form eines Einkaufswagens ist nur für Administratoren sichtbar. Damit legen sie das Foto in ihren Sammelkorb. Anschliessend ist der Sammelkorb im Administrationsbereich verfügbar, um über die [Stapelverarbeitung](../fotos-importieren-und-verwalten/stapelverarbeitung.md) Aktionen auf mehrere Fotos gleichzeitig anzuwenden.

## Die verfügbaren Dateigrössen in Ihrer Galerie verwalten

Um die in Ihrer Galerie verfügbaren Dateigrössen festzulegen, gehen Sie im Administrationsbereich auf Konfiguration > Optionen und dann auf die Registerkarte „Bildgrössen“.

Standardmässig bietet Piwigo mehrere Dateigrössen an. Tatsächlich importiert Piwigo nur die Originaldatei. Andere Grössen kann es aber bei Bedarf für die Benutzer erzeugen, je nachdem, welche Grössen Sie aktiviert haben.

![Tailles multiples.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-cf92d23b.jpg)

### Wozu dienen die verschiedenen Dateigrössen?

- Die Grössen „quadratisch“, „Vorschaubild“ und „mittel“ verwendet Piwigo, um die Fotos in der Galerie anzuzeigen. Deshalb können Sie diese nicht abwählen.
- Die anderen Grössen können Sie deaktivieren, indem Sie sie abwählen. In Ihrer Piwigo-Galerie können die Benutzer unter den verfügbaren Formaten wählen, in welcher Dateigrösse ein Foto auf ihrem Bildschirm angezeigt wird.

Wenn Sie mehr über die einzelnen Formate erfahren und sie gegebenenfalls anpassen möchten, klicken Sie auf „Details zeigen“ (rechts auf der Seite). Danach können Sie für jedes Format:

- die Grösse sehen, die Piwigo standardmässig erzeugt;
- diese Grösse anpassen, indem Sie neben dem jeweiligen Format auf „bearbeiten“ klicken;
- die Bildqualität anpassen (standardmässig 95 %);
- die Standardwerte wiederherstellen: So machen Sie Ihre bisherigen Änderungen rückgängig und kehren zu den Standardeinstellungen von Piwigo zurück;

![Montrer détails.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-7aad7329.jpg)

### Warum die verfügbaren Bildgrössen anpassen?

Das kann für verschiedene Zwecke nützlich sein.

Beispiel: Auf Ihrer Website verwenden Sie auf allen Seiten eine einheitliche Fotogrösse von 700 Pixeln Breite. In Ihrem Newsletter müssen dieselben Fotos 400 Pixel breit sein.

Sie können dann die Grösse XS auf eine Breite von 400 px und die Grösse S auf eine Breite von 700 px einstellen.

So wissen die Benutzer Ihrer Fotothek, dass sie für Ihre Website die Version S eines Fotos herunterladen müssen und für Ihren Newsletter die Version XS.

Wenn Sie das Plugin **Download by size** in Ihrer Galerie aktiviert haben, kann der Benutzer über die Download-Schaltfläche in Ihrer Galerie die Dateigrösse beim Herunterladen wählen.

Um die Grösse eines Dateiformats anzupassen, müssen Sie zuerst auf der Seite Konfiguration > Bildgrössen auf „Details zeigen“ klicken.

Klicken Sie neben dem Format, das Sie ändern möchten, auf „bearbeiten“. Dann können Sie die maximale Breite und Höhe des gewählten Formats ändern.

![Modifier détails.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-bc2fe3f8.jpg)

Wenn Sie „Zuschneiden“ auswählen, wird Ihre Datei von Piwigo automatisch auf die gewählten Masse „zugeschnitten“.

!!! danger "Mit dieser Wahl riskieren Sie, dass ein Teil Ihres Bildes verloren geht."

Wenn Sie mit dem Anpassen der Dateigrössen fertig sind, vergessen Sie nicht, auf „Einstellungen sichern“ zu klicken, um Ihre Konfiguration zu speichern.

## Optionen der Fotoseite

### Aktionen und Eigenschaften auf der Fotoseite

Im Administrationsbereich von Piwigo legen Sie fest, welche Aktionen in der Werkzeugleiste verfügbar sind, welche Eigenschaften auf der Fotoseite angezeigt werden, und weitere Anpassungsoptionen dieser Seite.

Mehr dazu lesen Sie im Artikel über die [Anpassungsoptionen Ihrer Galerie](../ihre-galerie-anpassen/anpassungsoptionen-fuer-ihre-galerie.md).

Weitere Informationen zur Anzeige von Eigenschaften und Metadaten finden Sie im Artikel über [Eigenschaften und Metadaten](../fotos-importieren-und-verwalten/eigenschaften-und-metadaten-von-fotos.md).

### Ihren Fotos ein Wasserzeichen hinzufügen

Wenn Sie ein Foto in Piwigo hochladen, kann Piwigo automatisch ein Wasserzeichen hinzufügen, also ein Bild, das „über“ Ihrem Foto angezeigt wird.

**Warum sollte ich meinen Fotos ein Wasserzeichen hinzufügen?**

Ein Wasserzeichen auf den Fotos der Galerie ist sinnvoll, wenn Sie Ihr Urheberrecht schützen möchten.

Mit einem Wasserzeichen sind Ihre Fotos in Ihrer Galerie sichtbar, das Original ist aber nicht verfügbar. Diese Option nutzen oft Fotografen, die ihre Arbeiten in ihrer Piwigo-Galerie zeigen, sich aber vor Verletzungen ihres Urheberrechts schützen möchten.

**Wie füge ich meinen Fotos ein Wasserzeichen hinzu?**

Gehen Sie in den Administrationsbereich und klicken Sie im linken Menü auf Konfiguration > Optionen.

Klicken Sie dann auf die Registerkarte „Wasserzeichen“. Hier wählen Sie eine Bilddatei, die allen Fotos Ihrer Galerie hinzugefügt wird, und legen verschiedene Anzeigeoptionen für das Wasserzeichen fest.

![Filigrane.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-9cdf5a09.jpg)

Um zu sehen, wie das aussieht, können Sie es mit einer der Dateien testen, die Piwigo mitliefert.

Wählen Sie neben „Eine Datei auswählen“ zum Beispiel Owned.png aus. Sie können die Position des Wasserzeichens ändern (in der Bildmitte oder in einer der Bildecken). Wählen wir zum Beispiel „Rechte untere Ecke“.

![Filigrane owned.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-533bc214.jpg)

Speichern Sie die Einstellungen: In Ihrer Galerie werden nun alle Fotos mit diesem Wasserzeichen in der rechten unteren Ecke angezeigt.

![Filigrane test.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-34ba3a9c.jpg)

Selbstverständlich können Sie auch Ihr eigenes Wasserzeichen hinzufügen.

Wir empfehlen dafür eine PNG-Datei mit transparentem Hintergrund.

## Die Fotoseite mit Plugins anpassen

Hier finden Sie eine Auswahl an Plugins, mit denen Sie der Fotoseite Funktionen hinzufügen können.

### Custom Download Link: Eine grosse Download-Schaltfläche hinzufügen

Das Plugin Custom Download Link fügt der Fotoseite eine grosse Download-Schaltfläche hinzu.

![Bouton télécharger.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-5f35d7ea.jpg)

Mit dieser Schaltfläche laden Sie direkt die Originalversion des Fotos herunter. Sie wird nicht angezeigt, wenn beim angemeldeten Benutzer das Recht „Download erlauben“ im Profil nicht aktiviert ist.

### Download by size: Die Grösse der heruntergeladenen Datei wählen

Wir haben es weiter oben in diesem Artikel bereits erwähnt: Mit dem Plugin **Download by Size** können Benutzer beim Klick auf das Download-Symbol die Grösse des heruntergeladenen Fotos wählen.

![Télécharger tailles.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-44796342.jpg)

### Private Share: Ein Foto per E-Mail über einen sicheren Link teilen

Mit dem Plugin Private Share können berechtigte Benutzer einen Freigabelink für ein Foto erzeugen und per E-Mail versenden. Besonders praktisch: So lässt sich ein Foto aus einem privaten Album teilen, sogar mit Personen ohne Piwigo-Konto.

Sobald dieses Plugin aktiviert ist, müssen Sie zuerst festlegen, welche Benutzer es verwenden dürfen. Öffnen Sie dazu die Konfiguration des Plugins. In der ersten Registerkarte legen Sie fest, welche Benutzergruppen es verwenden dürfen. [Mehr über Benutzergruppen erfahren](../benutzer-verwalten/benutzergruppen.md)

![Partage privé.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-7a18ccbb.jpg)

Die berechtigten Benutzer sehen bei jedem Foto Ihrer Piwigo-Galerie ein Symbol „Teilen“.

![private-share.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-0613b9fa.png)

Wenn Sie auf dieses Symbol klicken, öffnet sich ein Fenster. Dort geben Sie die E-Mail-Adresse ein, an die das Foto gesendet werden soll, und wie lange der Link gültig ist (1 Woche, 2 Wochen, 1 Monat oder 3 Monate).

![Partager cette photo.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-7e0d92f6.jpg)

Der Empfänger erhält einen Link, über den er das Foto ansehen kann.

![Envoi de photo.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-7ba56cdf.jpg)

Der erzeugte Link ist vollkommen sicher und gewährt nur Zugriff auf dieses eine Foto: Der Empfänger hat keine Möglichkeit, auf den Rest der Galerie zuzugreifen.

![Partage photo.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-e54ff42e.jpg)

Über die Konfiguration des Plugins (Registerkarte „Aktivität“) können Administratoren jederzeit den Nutzungsverlauf von Private Share einsehen: Sie sehen die geteilten Links, die Empfänger, das Freigabe- und das Ablaufdatum und können einen Freigabelink bei Bedarf ablaufen lassen.

![Liens envoyés.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-0028a962.jpg)

### Loupe: In ein Foto hineinzoomen

Mit dem Plugin **Loupe** können Benutzer ein Detail eines Fotos vergrössern bzw. hineinzoomen, indem sie mit der Maus darüberfahren.

Sobald dieses Plugin aktiviert ist, verwandelt sich der Mauszeiger in eine Lupe, wenn der Benutzer mit der Maus über ein Foto fährt. Mit dem Mausrad zoomen Sie hinein und heraus.

![Loupe.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-bde6ce16.jpg)

### Social Buttons: Schaltflächen zum Teilen in sozialen Netzwerken hinzufügen

Mit dem Plugin Social Buttons zeigen Sie auf der Fotoseite Schaltflächen an, mit denen sich die Seite in sozialen Netzwerken teilen lässt.

![Social buttons.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-507e15f1.jpg)

Für eine optimale Darstellung empfehlen wir folgende Optionen auf der Konfigurationsseite des Plugins Social Buttons:

- Position der Schaltflächen auf der Fotoseite: oben oder unten
- Schaltflächen anzeigen: nur beim Foto
- Grösse des geteilten Bildes: Wir empfehlen, nicht das Original zu teilen, sondern ein kleineres Format
- Light-Modus: Ein (wenn Sie den Light-Modus ausschalten, werden auf den Computern Ihrer Benutzer Cookies gesetzt, mit denen die Plattformen sie verfolgen können. Ausserdem ist der Light-Modus eleganter).

![Social buttons paramètres.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-0e95eaba.jpg)

!!! info "Info:"
    Wenn Sie das Erscheinungsbild Bootstrap Darkroom verwenden, brauchen Sie dieses Plugin nicht, da das Erscheinungsbild bereits Schaltflächen zum Teilen in sozialen Netzwerken enthält.

### Back2Front: Beidseitige Bilder verwalten

Mit dem Plugin **Back2Front** zeigen Sie auf der Fotoseite eine alternative Version desselben Fotos an. Es wird meist für beidseitige Bilder verwendet.

Eingesetzt wurde es zum Beispiel für Galerien mit Postkarten oder Sammelkarten.

Ist das Plugin aktiviert, können Sie auf der Bearbeitungsseite eines Fotos im Administrationsbereich festlegen, dass dieses Bild die Rückseite eines anderen Bildes (der Vorderseite) ist, und dazu die ID der Vorderseite angeben. Sie können wählen, ob die Rückseite im Album ausgeblendet wird.

![Recto verso.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-f1c307b0.jpg)

Wurde für ein Foto eine Rückseite festgelegt, erscheint auf der Fotoseite eine Schaltfläche „Rückseite ansehen“. Ein Klick darauf zeigt das Bild der Rückseite an.

![Verso.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-692be821.jpg)

### AlwaysShowMetadata: Die Metadaten der Dateien immer anzeigen

Standardmässig sind die Metadaten auf der Fotoseite Ihrer Galerie ausgeblendet: Sie müssen auf ein Symbol klicken, um sie anzuzeigen.

Wenn sie immer angezeigt werden sollen, installieren Sie das Plugin **AlwaysShowMetadata**.

Mehr über Metadaten erfahren Sie in [diesem Artikel](../fotos-importieren-und-verwalten/eigenschaften-und-metadaten-von-fotos.md).

### RightClick: Den Rechtsklick auf der Fotoseite sperren

Wenn Sie verhindern möchten, dass Benutzer ein Foto per Rechtsklick herunterladen, können Sie das Plugin **rightClick** installieren.

Sobald dieses Plugin aktiviert ist, funktioniert der Rechtsklick auf der Fotoseite und auch auf anderen Seiten nicht mehr, ausser für Administratoren.

!!! warning "Warnung:"
    Dieses Plugin garantiert nicht, dass Ihre Bilder vollständig geschützt sind. Nur wenn Sie Ihre Alben auf privat stellen, sind Ihre Fotos wirklich geschützt.

### Hide title: Den Namen des Fotos in der Brotkrumennavigation ausblenden

Standardmässig zeigt die Brotkrumennavigation auf der Fotoseite den Namen des Fotos an.

![Titre.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-c8fa5581.jpg)

Um ihn auszublenden, aktivieren Sie einfach das Plugin **Hide Title on Browse Path**.

![Sans titre.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-4f6f1c97.jpg)

### Automatic size: Automatische Dateigrösse je nach Bildschirmgrösse

Mit dem Plugin Automatic Size passt sich die standardmässig angezeigte Dateigrösse an die Bildschirmgrösse des Benutzers an. Es wurde für Galerien mit dem Erscheinungsbild **Elegant** entwickelt.

Dieses Plugin **ist nicht sinnvoll, wenn Ihre Galerie das Erscheinungsbild Modus verwendet**, da Modus bereits standardmässig automatisch die Grösse anzeigt, die zur Auflösung Ihres Bildschirms passt.

Ausserdem ist dieses Plugin nicht mit dem Erscheinungsbild **Bootstrap Darkroom** kompatibel.

### Color Palette: Die Farben eines Fotos extrahieren

Mit dem Plugin Color Palette extrahieren Sie automatisch die Farben eines Fotos und können Fotos nach Farbe suchen.

Sobald dieses Plugin aktiviert ist, finden Sie bei jedem Foto Ihrer Galerie die Palette der im Foto enthaltenen Farben.

![Palette écran complet.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-b2cd7de3.jpg)

Wenn Sie auf eine oder mehrere Farben der Palette klicken, suchen Sie nach allen Fotos Ihrer Galerie, die dieselben Farben enthalten.

![Palette.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-2222c058.jpg)

![Recherche palette.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-d926b5ba.jpg)

Auf der Konfigurationsseite des Plugins können Sie einige Optionen einstellen, zum Beispiel die Anzahl der Farben pro Palette.

![Palette config.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-7830d4e6.jpg)

!!! warning "Warnung:"
    Das Aktivieren des Plugins erzeugt nicht für alle Bilder Ihrer Fotothek eine Palette. Die Palette eines Fotos wird erzeugt, wenn es nach dem Aktivieren des Plugins zum ersten Mal angezeigt wird. Anfangs liefert die Suche nach Farbe daher nur sehr wenige Ergebnisse, weil die Paletten Ihrer Fotos noch nicht erzeugt wurden.
