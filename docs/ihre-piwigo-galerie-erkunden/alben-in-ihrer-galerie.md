---
title: Alben in Ihrer Galerie - Piwigo-Dokumentation
description: Wie Sie in Ihrer Piwigo-Galerie durch Alben navigieren und deren Anzeige anpassen, erfahren Sie in diesem Artikel!
---

# Alben in Ihrer Galerie

In einer Piwigo-Galerie navigiert man meistens über die Alben. Zur Erinnerung: In Piwigo muss sich jedes Foto in einem Album befinden. Ein Album können Sie sich wie einen Ordner oder eine Kategorie vorstellen.

Alben sind baumartig aufgebaut. Sie können Unteralben enthalten, die wiederum selbst Unteralben enthalten können, und so weiter.

Sobald Sie in Ihrer Galerie auf ein Album klicken, gelangen Sie auf die Albumseite.

In diesem Artikel erfahren Sie, wie Sie durch die Alben navigieren, wie die Albumseite aufgebaut ist, welche Funktionen es gibt und welche Anpassungsmöglichkeiten Ihnen standardmässig oder mit Plugins zur Verfügung stehen.

!!! note "Hinweis"
    Die meisten Screenshots in diesem Artikel zeigen eine Galerie mit dem Erscheinungsbild Modus. Je nach Erscheinungsbild Ihrer Galerie können Informationen und Symbole anders dargestellt werden.

Mehr über Alben erfahren Sie in dieser Artikelreihe:

[Alben organisieren](../alben-organisieren/index.md)

## Vorbemerkung

In Ihrer Galerie werden alle Seiten, die Fotos auflisten (Suchergebnisse, Fotos zu einem Schlagwort, die Seite „Meine Fotos“ oder die Seite „Am häufigsten angesehen“ …), genauso dargestellt wie die Albumseite.

Das bedeutet: Die Funktionen der Albumseite sind im Wesentlichen dieselben wie auf den anderen Seiten, die Fotos auflisten.

![Albumseite](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-49b0922b.jpg)

Albumseite

![Schlagwortseite](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-00ec7d64.jpg)

Schlagwortseite

![Seite mit Suchergebnissen](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-f44e9417.jpg)

Seite mit Suchergebnissen

## Die Alben in Ihrer Galerie

Auf der Startseite Ihrer Galerie sehen Sie die Liste der Alben der ersten Ebene (Hauptalben).

![Albums.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-5b1f1709.jpg)

Angezeigt werden:

- alle öffentlichen Alben
- alle privaten Alben, die Sie sehen dürfen, sofern Sie angemeldet sind. [Mehr über Zugriffsrechte erfahren](../alben-organisieren/zugriffsrechte-und-sichtbarkeit-von-alben.md)

!!! info "Info:"
    Standardmässig zeigt die Startseite 12 Alben pro Seite an. Mit den Seitenlinks unten auf der Seite blättern Sie durch Ihre Alben. Um die Anzahl der Alben pro Seite zu ändern, gehen Sie im Administrationsbereich auf Konfiguration > Optionen, Registerkarte „Anzeige“.


Wenn Sie auf ein Album klicken, öffnet sich die Albumseite.

Was dort angezeigt wird, hängt vom Inhalt des Albums ab: Es enthält entweder direkt Fotos (oder andere Dateien) oder Unteralben.

!!! info "Info:"
    Das Konzept von Alben und Unteralben wird in [diesem Artikel](../alben-organisieren/alben-und-unteralben.md) erklärt. Ein Album kann zwar gleichzeitig Unteralben und Dateien enthalten, wir empfehlen das aber nicht.

## Album mit Unteralben

Enthält das Album Unteralben, zeigt die Seite des übergeordneten Albums die Vorschaubilder dieser Unteralben an, und so weiter.

Am Navigationspfad (Brotkrumennavigation) oben links sehen Sie, wo Sie sich in der Baumstruktur befinden.

![Beispiel: ein Album „Gebäude“ mit zwei Unteralben „Kirchen“ und „Häuser“](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-fab9f046.jpg)

Beispiel: ein Album „Gebäude“ mit zwei Unteralben „Kirchen“ und „Häuser“

Die Werkzeugleiste bietet verschiedene Aktionen an. Welche das sind, hängt von Ihren Benutzerrechten, Ihrem Erscheinungsbild und den Einstellungen Ihrer Galerie ab.

Unter anderem können Sie alle Dateien des Albums (aus allen Unteralben zusammen) anzeigen, indem Sie auf das entsprechende Symbol klicken (es sieht je nach Erscheinungsbild anders aus). Mit dem Symbol in Form eines Baumdiagramms kehren Sie zur normalen Ansicht zurück.

## Anzeige der Fotos auf der Albumseite

Enthält das Album keine Unteralben, sondern nur Fotos, zeigt die Albumseite die Vorschaubilder der Fotos des Albums an.

Wenn das Album viele Dateien enthält, erscheinen unten Seitenlinks, mit denen Sie durch das Album blättern können.

![Pagination.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-41c3c554.jpg)

Möchten Sie alle Fotos auf der Albumseite anzeigen, können Sie das Plugin **RV Thumb Scroller** aktivieren. Dieses Plugin lädt die Fotos nach und nach, während der Benutzer auf der Seite nach unten scrollt.

!!! info "Info:"
    Um die Anzahl der Fotos auf einer Albumseite zu ändern, öffnen Sie Ihre [Benutzereinstellungen](../benutzer-verwalten/benutzer-erstellen-und-verwalten.md). Sie erreichen sie über das Menü „Anpassen“ in der Galerie oder indem Sie Ihr Benutzerprofil im Administrationsbereich bearbeiten.

## Die Werkzeugleiste der Albumseite

Über die Werkzeugleiste erreichen Sie verschiedene Funktionen.

![Untitled](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-6b027860.png)

!!! note "Hinweis"
    Welche Symbole und Funktionen in Ihrer Galerie verfügbar sind, hängt vom gewählten Erscheinungsbild, von der Konfiguration von Piwigo, von den aktivierten Plugins usw. ab. Die Beispiele auf dieser Seite zeigen die Standardmöglichkeiten des Erscheinungsbilds [Modus](../erscheinungsbilder/modus-erscheinungsbild.md). Wenn Sie zum Beispiel das Erscheinungsbild [Bootstrap Darkroom](../erscheinungsbilder/bootstrap-darkroom-erscheinungsbild.md) verwenden, sind die Funktionen im Allgemeinen dieselben, die Symbole sehen aber etwas anders aus.

### Die Sortierreihenfolge der Fotos ändern

Mit dem Symbol „Sortierreihenfolge“ können Sie die Standardsortierung ändern. So sortieren Sie Ihre Fotos zum Beispiel nach Veröffentlichungsdatum, alphabetisch oder nach Anzahl der Aufrufe …

![Ordre de tru.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-1e01d25d.jpg)

!!! info "Info"
    Die Standardsortierung ändern Sie im Administrationsbereich unter Konfiguration > Optionen.

### Die Grösse der angezeigten Fotos ändern

Um die Grösse der Vorschaubilder auf dem Bildschirm zu ändern, klicken Sie auf das Symbol „Bildgrössen“.

![Tailles de photos.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-814fc23e.jpg)

Beispiel einer Anzeige in der Grösse „Vorschaubild“:

![Taille miniature.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-000dc2e6.jpg)

### In den Sammelkorb (nur für Administratoren)

Als Administrator können Sie mit dem Symbol in Form eines Einkaufswagens alle Fotos des Albums in Ihren Sammelkorb legen. Den Sammelkorb finden Sie anschliessend im Administrationsbereich. Dort können Sie über die [Stapelverarbeitung](../fotos-importieren-und-verwalten/stapelverarbeitung.md) Aktionen auf diese Fotos anwenden.

### Album bearbeiten (nur für Administratoren)

Als Administrator gelangen Sie mit dem Symbol in Form eines Werkzeugs in den Administrationsbereich, um [das Album zu bearbeiten](../alben-organisieren/ein-album-bearbeiten.md).

### Fotos im Kalendermodus anzeigen

Möchten Sie die Fotos nach ihrem Hochladedatum anzeigen, klicken Sie auf das Kalendersymbol. Sie können Ihre Fotos dann nach dem Jahr und dem Monat filtern, in dem sie zu Piwigo hinzugefügt wurden.

![Date de publication.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-01c39b75.jpg)

Mit dem Symbol in Form einer Kamera filtern Sie die Fotos nach ihrem Aufnahmedatum (und nicht nach dem Datum, an dem sie zu Piwigo hinzugefügt wurden).

![Date de création.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-56fff16b.jpg)

Um zur normalen Ansicht zurückzukehren, klicken Sie auf das Symbol in Form eines Baumdiagramms.

### Eine Diashow starten

Mit einem Klick auf das Wiedergabe-Symbol in der Werkzeugleiste starten Sie eine Diashow im Vollbildmodus.

![Diaporama.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-a372817c.jpg)

### Albumbeschreibung

Wenn Sie ein Album im Administrationsbereich bearbeiten, können Sie eine Beschreibung für dieses Album eingeben.

Sie wird auf der Albumseite und in der Albumliste angezeigt (abhängig vom Erscheinungsbild und dessen Konfiguration).

Mit dem Erscheinungsbild Modus erscheint die Beschreibung standardmässig oben auf der Albumseite.

![Description album.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-5dc7059e.jpg)

## Optionen der Albumseite

### Die verfügbaren Aktionen auf der Albumseite festlegen

Wie einige Funktionen auf der Albumseite angezeigt werden, können Sie im Administrationsbereich von Piwigo unter Konfiguration > Optionen anpassen.

In der Registerkarte „Anzeige“ legen Sie fest, welche Aktionen in der Werkzeugleiste der Albumseite verfügbar sind.

- Symbol »Sortierreihenfolge« anzeigen
- Symbol »Alle Fotos aller Unteralben anzeigen« anzeigen
- Symbol »Fotos nach Veröffentlichungsdatum anzeigen« anzeigen
- Symbol »Fotos nach Aufnahmedatum anzeigen« anzeigen
- Symbol »Diashow« anzeigen
- Symbol »Bildgrössen« anzeigen
- Symbol »Album bearbeiten« anzeigen (nur für Administratoren verfügbar)
- Symbol »In den Sammelkorb« anzeigen (nur für Administratoren verfügbar)

![Affichage.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-b38cee21.jpg)

### Optionen der Erscheinungsbilder

Je nach Erscheinungsbild Ihrer Galerie stehen Ihnen weitere Gestaltungsoptionen für die Albumseite zur Verfügung.

Mehr dazu finden Sie in der Dokumentation Ihres Erscheinungsbilds:

- [Dokumentation zu Modus](../erscheinungsbilder/modus-erscheinungsbild.md)
- [Dokumentation zu Bootstrap Darkroom](../erscheinungsbilder/bootstrap-darkroom-erscheinungsbild.md)

### Die Anzahl der Fotos auf der Albumseite ändern

Standardmässig zeigt Piwigo 15 Vorschaubilder auf einer Albumseite an. Sie können aber auch mehr (oder weniger) anzeigen.

Um die Anzahl der Fotos auf einer Albumseite zu ändern, öffnen Sie Ihre Benutzereinstellungen. Sie erreichen sie über das Menü „Anpassen“ in der Galerie oder indem Sie Ihr Benutzerprofil im Administrationsbereich bearbeiten.

[Mehr über Einstellungen erfahren](../benutzer-verwalten/benutzer-erstellen-und-verwalten.md)

## Die Albumseite mit Plugins anpassen

### Comments on Albums: Kommentare zu Alben anzeigen

Standardmässig können die Benutzer Ihrer Galerie [Kommentare](../kommentare-und-bewertungen/plugins-zur-kommentarverwaltung.md) zu Fotos schreiben, aber nicht zu Alben.

Wenn Sie diese Möglichkeit aktivieren möchten, aktivieren Sie einfach das Plugin **Comments on Albums**.

[Mehr erfahren](../kommentare-und-bewertungen/plugins-zur-kommentarverwaltung.md)

### Batch Downloader: Alle Dateien eines Albums (oder einer Auswahl) als ZIP herunterladen

Mit dem Plugin **Batch Downloader** können berechtigte Benutzer mit einem Klick eine ZIP-Datei mit mehreren Dateien herunterladen. Das geht unter anderem über die Albumseite.

Sobald das Plugin aktiviert ist, erscheint in der Werkzeugleiste der Albumseite ein neues Symbol. Damit laden Sie alle Dateien der Auswahl herunter.

![Télécharger toutes les photos.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-766e8b93.jpg)

Dieses Symbol gibt es nicht nur auf der Albumseite, sondern auf allen Seiten, die Fotos auflisten:

- Suchergebnisse
- Fotos zu einem oder mehreren Schlagworten
- Seite „Meine Favoriten“
- usw.

Mit einem Klick auf das Symbol wählen Sie die Grösse der heruntergeladenen Fotos. Zur Auswahl stehen die Bildgrössen, die in Ihrer Galerie verfügbar sind.

![Téléchargement.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-e568972c.jpg)

Nachdem Sie die Grösse gewählt haben, beginnt der Download.

Über das neue Menü „Downloads“ in der Galerie kann der Benutzer jederzeit den Verlauf seiner heruntergeladenen Dateien einsehen.

Diese Seite fasst die heruntergeladenen Dateien zusammen. Sie können dort einen Download abbrechen oder die Datei über den Link „Archiv (bereit)“ auf Ihren Computer herunterladen.

![Archive prête.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-56875108.jpg)

Die Einstellungen des Plugins Batch Downloader bestehen aus einer Seite mit zwei Registerkarten:

**Verlauf**

Diese Seite zeigt den Verlauf der Downloads über das Plugin Batch Downloader. Sie sehen dort:

- den Benutzer, der den Download angefordert hat
- das heruntergeladene Paket
- das Datum
- die Grösse
- die Anzahl der Fotos
- den Status

![Téléchargement masse.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-0f8b9a69.jpg)

**Konfiguration**

In der Registerkarte „Konfiguration“ legen Sie genau fest, welche Optionen in Ihrer Galerie verfügbar sind.

![Config téléchargement masse.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-49bb67a4.jpg)

- Wer Fotos gesammelt herunterladen darf
- Welche Art von Fotozusammenstellung heruntergeladen werden kann (nur Alben oder auch „spezielle“ Seiten wie „Am häufigsten angesehen“, „Am besten bewertet“ …)
- Welche Bildgrösse für Downloads erlaubt ist

Ausserdem können Sie Regeln festlegen, etwa wie lange Archive auf dem Server gespeichert werden, wie viele Fotos ein Paket höchstens enthalten darf, wie gross ein Archiv höchstens sein darf …

Die erweiterten Funktionen listen die Optionen auf, die sich über die Konfigurationsdatei von Piwigo bearbeiten lassen.

Wenn Sie Piwigo selbst hosten, können Sie diese mit [LocalFile Editor](../piwigo-selbst-hosten/lokale-konfiguration-bearbeiten-localfiles-editor.md) bearbeiten. Wenn Sie Kunde eines Piwigo-Cloud-Angebots sind, wenden Sie sich an den Support, um eine dieser Einstellungen ändern zu lassen.

### ShareAlbum: Einen sicheren Link zu einem Album teilen

Mit dem Plugin **ShareAlbum** können berechtigte Benutzer einen Freigabelink zu einem Album erzeugen. Besonders praktisch: So lässt sich der Inhalt eines privaten Albums teilen, sogar mit Personen ohne Piwigo-Konto.

Sobald dieses Plugin aktiviert ist, finden Sie bei jedem Album Ihrer Piwigo-Galerie ein Symbol „Teilen“.

![sharealbum.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-8fb407d2.png)

Wenn Sie auf dieses Symbol klicken, erscheint eine Schaltfläche „Dieses Album teilen“.

![sharealbum.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-23bfb0b4.png)

Nachdem das Album geteilt wurde, klicken Sie erneut auf das Symbol, um den Freigabelink anzuzeigen.

![Sharealbum lien.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-46564762.jpg)

Wenn Sie den Freigabelink nicht mehr brauchen, können Sie ihn aufheben. Er ist danach nicht mehr erreichbar.

Mit „Link erneuern“ können Sie ausserdem einen neuen Link erzeugen (der zuvor erzeugte Link ist dann nicht mehr erreichbar).

Wenn Sie Piwigo in einem Unternehmen einsetzen, ist das sehr nützlich, um den Inhalt eines Albums gelegentlich mit Personen ausserhalb Ihrer Organisation zu teilen (Kunden, Partnern, Journalisten …).

Die Konfiguration des Plugins ShareAlbum besteht aus zwei Registerkarten:

**Registerkarte „Konfiguration“**

Hier finden Sie die Konfigurationsoptionen von ShareAlbum.

- Menüs für Albumbesucher ausblenden: Ist diese Option aktiviert, zeigt der Freigabelink nur den Inhalt des Albums an, ohne das Navigationsmenü oben auf dem Bildschirm. In diesem Fall können Sie wählen, ob auf der geteilten Seite ein Anmeldemenü angezeigt wird.
- Automatische Anmeldung aktivieren
- Brotkrumennavigation durch den Albumnamen ersetzen: blendet die Baumstruktur des Albums aus
- Freigaben auf Unteralben anwenden: legt fest, ob die Freigabe eines Albums auch Zugriff auf seine Unteralben gewährt
- Freigabe von Alben für Benutzer ohne Administratorrechte erlauben: erlaubt Benutzern ohne Administratorrechte, Freigabelinks zu erstellen

![Sharealbum.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-d9f770d4.jpg)

**Registerkarte „Geteilte Alben“**

In der zweiten Registerkarte sehen Sie den Verlauf der mit dem Plugin ShareAlbum erzeugten Freigabelinks. Sie sehen, wer die Links erstellt hat, wie oft sie aufgerufen wurden und zu welchem Album sie gehören. Ausserdem können Sie bestehende Freigabelinks erneuern und löschen.

Auf diesem Bildschirm können Sie auch Freigabelinks erstellen, ohne den Umweg über Ihre Galerie.

![Albums partagés.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-7d51229c.jpg)

### GThumb+: Vorschaubilder als Mosaik anzeigen

Standardmässig werden die Vorschaubilder auf den Albumseiten und den anderen Seiten Ihrer Galerie, die Fotos auflisten, in einem Raster angezeigt. Alle Vorschaubilder haben dieselbe Höhe.

Mit dem Plugin GThumb+ können Sie sie als Mosaik mit unterschiedlichen Höhen anzeigen.

![Standardanzeige](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-df0b6b3a.jpg)

Standardanzeige

![Anzeige mit Gthumb+](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-712ffb35.jpg)

Anzeige mit Gthumb+

In der Konfiguration des Plugins passen Sie die Standardoptionen an, zum Beispiel:

- maximale Höhe der Vorschaubilder
- Abstand zwischen den Vorschaubildern
- Anzahl der Vorschaubilder pro Seite
- usw.

### Image Preview: Vorschaubilder beim Überfahren mit der Maus vergrössern

Mit dem Plugin **Image Preview** werden Vorschaubilder vergrössert, sobald man mit der Maus darüberfährt, auf der Albumseite oder jeder anderen Übersichtsseite der Galerie.

![Miniature.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-dff2e378.jpg)

In der Konfiguration des Plugins legen Sie die Grösse des angezeigten Bildes fest (standardmässig höchstens 400 px breit und 600 px hoch).

Ausserdem können Sie wählen, ob der Name des Bildes angezeigt wird, ob beim Überfahren ein Transparenzeffekt angewendet wird und ob die Bilder vorab geladen werden (aus Leistungsgründen nicht empfohlen).

!!! warning "Warnung:"
    Wenn Sie das Erscheinungsbild Modus verwenden, müssen Sie zuerst das Plugin **GThumb+** aktivieren, um das Plugin Image Preview nutzen zu können (siehe vorheriges Kapitel).

### Lightbox: Das Foto in einem Pop-in-Fenster statt auf der Fotoseite anzeigen

Standardmässig gelangen Sie auf die Fotoseite, wenn Sie in einem Album auf ein Foto klicken.

Das Plugin Lightbox ändert dieses Verhalten von Piwigo: Ist es aktiviert, wird ein angeklicktes Foto in einem Pop-in-Fenster (modales Pop-up) über der Albumseite angezeigt, wie im Beispiel unten.

![Untitled](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-0068cdc1.png)

Mit den Pfeilen blättern Sie durch das Album.

In den Konfigurationsoptionen des Plugins können Sie einige Einstellungen anpassen:

- ob der Titel des Bildes angezeigt wird
- ob man mit einem Klick auf den Titel des Bildes zur Fotoseite gelangt
- ob die Navigationspfeile angezeigt werden
- das Aussehen der Lightbox (dunkler oder heller Hintergrund …)
- die Abmessungen der Lightbox

### Permalink Generator: Die URL einer Albumseite anpassen

Wenn Sie ein neues Album erstellen, zum Beispiel mit dem Namen „Shooting“, hat seine URL (Webadresse) standardmässig folgende Form: mypiwigo.com/index?/category/XX_shooting (XX ist die ID dieses Albums in der Datenbank von Piwigo)

Wenn Sie den Namen des Albums ändern, ändert sich auch seine URL.

Mit dem Plugin **Permalinks Generator** können Sie eindeutige URLs für Ihre Alben erzeugen, die auch dann gültig bleiben, wenn Sie den Namen ändern.

Sobald das Plugin aktiviert ist, öffnen Sie seine Konfiguration und klicken auf „Fehlende Permalinks erzeugen“. Die URLs Ihrer Alben haben sich dann geändert und haben nun folgendes Format: mypiwigo.com/index?/category/shooting.

Wenn Sie den Namen des Albums ändern, bleibt die URL gleich.

### Quick Fav: Ein Foto über die Albumseite zu den Favoriten hinzufügen

In Piwigo kann jeder Benutzer Fotos zu seinen Favoriten hinzufügen, um sie später schnell wiederzufinden. Standardmässig geht das nur über die Fotoseite.

Mit dem Plugin **Quick Fav** fügen Sie ein Foto mit nur einem Klick über sein Vorschaubild hinzu, auf der Albumseite oder einer anderen Übersichtsseite.

!!! warning "Warnung:"
    Dieses Plugin ist derzeit nur mit dem Erscheinungsbild Bootstrap Darkroom kompatibel. Ausserdem steht es nur Kunden von [Piwigo Cloud](https://de.piwigo.org/piwigo-bekommen) zur Verfügung (das soll bald behoben werden).

Sobald dieses Plugin aktiviert ist, erscheint ein Herz, wenn Sie mit der Maus über ein Foto fahren. Ein Klick auf das Herz fügt das Foto zu den Favoriten des Benutzers hinzu.

![Quick fav 2.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-106deb84.jpg)

Fahren Sie mit der Maus über einen Favoriten, erscheint das Herz ausgefüllt. Klicken Sie erneut darauf, um das Foto aus Ihren Favoriten zu entfernen.

![Favori.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-22b2178f.jpg)

**Ein ganzes Album mit Quick Fav zu den Favoriten hinzufügen**

Mit dem Plugin **Quick Fav** können Sie auch ein ganzes Album zu Ihren Favoriten hinzufügen.

Auf einer Seite, die Alben auflistet, erscheint dasselbe Symbol wie in einer Fotoliste. Damit fügen Sie den Inhalt eines Albums mit einem Klick zu Ihren Favoriten hinzu.

![Album fav.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-7951755d.jpg)

### Thumbnail Tooltip: Den Tooltip auf dem Vorschaubild eines Fotos anpassen

Wenn Sie auf einer Albumseite mit der Maus über ein Foto fahren, werden einige Informationen zum Foto in einem Tooltip angezeigt (Titel, Anzahl der Aufrufe …).

Den Inhalt dieses Tooltips können Sie mit dem Plugin **Thumbnail Tooltip** anpassen.

!!! warning "Warnung"
    Das Erscheinungsbild Modus zeigt auf der Albumseite keinen Tooltip an. Deshalb ist das Plugin Thumbnail Tooltip nicht mit Modus kompatibel.

Sobald das Plugin aktiviert ist, legen Sie in seiner Konfiguration fest, was im Tooltip angezeigt wird und in welcher Reihenfolge.

![TT.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-6af3607c.jpg)

![TT example.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-531023f7.jpg)

### RV Thumb Scroller: Endloses Scrollen auf der Albumseite

Mit dem Plugin **RV Thumb Scroller** können Sie die Seitenlinks auf der Albumseite abschalten.

Ist es aktiviert, werden die Vorschaubilder der Fotos beim Scrollen nach und nach geladen, ganz gleich, wie viele Fotos das Album enthält.
