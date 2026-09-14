---
title: Statistik in Piwigo - Piwigo-Dokumentation
description: Piwigo bietet Administratoren standardmässig oder über Plugins mehrere Möglichkeiten, die Nutzung ihrer Fotobibliothek zu beobachten und ihren Erfolg zu verfolgen.
---

# Die Statistik Ihrer Piwigo-Galerie ansehen

Piwigo bietet Administratoren standardmässig oder über Plugins mehrere Möglichkeiten, die Nutzung ihrer Fotobibliothek zu beobachten und zu verfolgen, wie erfolgreich sie ist.

## Dashboard

Die Startseite des Administrationsbereichs von Piwigo heisst Dashboard.

![Untitled](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-99beacea.png)

Auf dem Dashboard sehen Sie die Nutzung Ihrer Galerie auf einen Blick:

- Anzahl der Fotos
- Anzahl der Alben
- Anzahl der Schlagworte
- Anzahl der Benutzer
- Anzahl der Gruppen
- Kommentare
- Bewertungen
- Seitenzugriffe (seit Beginn)
- Installierte Plugins
- Belegter Speicher
- Nur bei Piwigo Cloud: Anzahl der verbleibenden Tage im aktuellen Zeitraum (Testphase, Abonnement …)

Jedes Symbol ist zugleich eine Verknüpfung zur Verwaltungsseite des jeweiligen Bereichs.

Ausserdem gibt Ihnen das Dashboard einen Überblick über die Aktivitätsspitzen der letzten 4 Wochen.

Eine farbige Blase stellt die Aktivität für jeden Wochentag dar. Wenn Sie mit der Maus über diese Blase fahren, sehen Sie die ausgeführten Aktionen.

![en-activity-dashboard.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-79b0b62b.png)

Seit Version 14 von Piwigo sehen Sie auf dem Dashboard auch den belegten Speicher pro Dateityp und Format.

![Untitled](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-27638894.png)

## Besuchsstatistik

Um die Besuchsstatistik Ihrer Piwigo-Galerie aufzurufen, öffnen Sie im Administrationsbereich das Menü Werkzeuge > Statistik.

Diese Seite zeigt ein Diagramm der Besuche in Ihrer Piwigo-Galerie.

![fr-historique-stats.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-6cae9134.png)

Sie können diese Statistik anzeigen:

- pro Tag für die letzten 3 Monate
- pro Stunde für die letzten 3 Tage
- pro Monat für die letzten 5 Jahre
- pro Jahr seit der Erstellung Ihrer Piwigo-Galerie

Wenn Sie mit der Maus über das Diagramm fahren, sehen Sie die Anzahl der Seitenzugriffe für jeden Zeitraum.

Wenn Sie oben rechts auf „Vergleichsmodus“ klicken, erhalten Sie eine andere Ansicht der Statistik.

- Die Ansicht Jahr zeigt eine Kurve pro Jahr, jede in einer eigenen Farbe; jede Kurve zeigt die Anzahl der Besuche pro Monat in diesem Jahr. So sehen Sie zum Beispiel, ob die Besuche in Ihrer Galerie einem saisonalen Muster folgen, das sich jedes Jahr wiederholt.
    
    ![en-history-compare-month.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-bd711ced.png)
    
- Die Ansicht Monat zeigt eine Kurve pro Monat für die letzten 3 Monate sowie einen Durchschnitt der letzten 12 Monate, jede Kurve in einer eigenen Farbe; jede Kurve zeigt die Anzahl der Besuche pro Tag. So sehen Sie zum Beispiel, wie sich die Besuche in Ihrer Galerie in den letzten Monaten entwickelt haben.
    
    ![en-history-compare-month.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-68fea989.png)
    

### Optionen für die Statistik

Die Erfassung der Besuche passen Sie im Administrationsbereich auf der Seite Konfiguration > Optionen an, im Reiter Allgemein, Abschnitt Verschiedenes.

Mit der Option „Besuche in der History speichern für“ legen Sie fest, welche Besuche in der Statistik erfasst werden:

- Besuche von Gästen (anonym)
- Besuche von registrierten Besuchern
- Besuche von Administratoren

Sie können natürlich alle diese Optionen oder nur einige davon auswählen.

Wenn die Statistik zum Beispiel die Beliebtheit Ihrer Galerie widerspiegeln soll und nicht die Arbeit der Administratoren, kann es sinnvoll sein, die Erfassung für Administratoren zu deaktivieren.

### Den Verlauf durchsuchen

Wie erfahren Sie, was Benutzer in Ihrer Galerie tun? Wer hat diese oder jene Datei heruntergeladen?

Diese Frage stellt sich immer wieder: um zu wissen, welche Fotos beliebt sind, aber zum Beispiel auch, um zu erfahren, wer urheberrechtlich geschützte Dateien heruntergeladen hat.

Das ist mit der **Suche im Verlauf** möglich.

Im Menü Werkzeuge > Statistik zeigt Ihnen der Reiter Suchen einen detaillierten Verlauf der in Ihrer Piwigo-Galerie ausgeführten Aktionen und ermöglicht eine Suche.

![Historique par utilisateur.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-923e5b0d.jpg)

Diese Seite listet die in Ihrer Galerie in einem bestimmten Zeitraum ausgeführten Aktionen in chronologischer Reihenfolge auf. Den Zeitraum wählen Sie über die Datumsfilter.

Hier werden zwei Arten von Aktionen angezeigt:

- Seitenaufrufe
- Datei-Downloads

Mit dem Filter „Aktion“ können Sie nur Besuche oder nur Downloads anzeigen.

Die Tabelle zeigt:

- Datum: Datum und Uhrzeit der Aktion
- Benutzer: Der Benutzer, der die Aktion ausgeführt hat (anonyme Benutzer werden als „Gast“ angezeigt), und seine IP-Adresse
- Objekt: Das betroffene Album oder die betroffene Datei. Aufrufe der Startseite sind mit „Stamm“ gekennzeichnet.
- Einzelheiten: Bei einfachen Besuchen wird hier das betroffene Album angezeigt, bei Downloads der Hinweis „Heruntergeladen“.

![Activités différentes.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-1c9e8597.jpg)

Sie können die Liste auf einen bestimmten Benutzer filtern, indem Sie in der Leiste über der Tabelle auf seinen Namen klicken.

Der gewählte Benutzer erscheint dann bei den zusätzlichen Filtern. Mit einem Klick auf das Kreuz neben dem Benutzer setzen Sie die Filter zurück.

![Dernière capture.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-70e4047b.jpg)

Schliesslich können Sie die Aktionen auch nach einem bestimmten Foto filtern: Klicken Sie dazu auf die 3 Punkte neben einem Vorschaubild und dann auf „Als Filter hinzufügen“.

![Ajouter comme filtre.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-31f8b368.jpg)

So sehen Sie alle Downloads eines Fotos für den gewünschten Zeitraum.

## Die Aktivität der Piwigo-Administratoren ansehen

Um den detaillierten Verlauf aller Aktionen der Benutzer im Administrationsbereich von Piwigo anzusehen, öffnen Sie einfach den Reiter Tätigkeit auf der Seite Benutzer.

!!! info "Wenn Sie Kunde von Piwigo Cloud sind, ist diese Funktion erst ab dem Team-Tarif verfügbar"

Diese Seite zeigt alle Aktivitäten der Benutzer in Ihrer Piwigo-Galerie:

- Anmelden / Abmelden
- Fotos importieren / bearbeiten / löschen (und andere Dateien)
- Alben erstellen / bearbeiten / löschen / verschieben
- Benutzer und Benutzergruppen erstellen / bearbeiten / löschen
- Schlagworte erstellen / bearbeiten / löschen

Sie können diese Liste nach Benutzer filtern.

![Activité utilisateur.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-4d5075b2.jpg)

## AStat.2: Detaillierte Statistik

Für eine erweiterte Statistik können Sie das Plugin **AStat.2** herunterladen.

Sobald dieses Plugin installiert ist, sehen Sie die Anzahl der aufgerufenen Seiten, Bilder und Alben nach zahlreichen Kriterien. Es bietet:

- Statistik nach Zeitraum
- Statistik nach IP-Adresse
- Statistik nach Album
- Statistik nach Datei

Mit verschiedenen Optionen passen Sie die Darstellung der Daten an.

Ausserdem können Sie mit diesem Plugin die Statistik „bereinigen“, damit sie vollständiger ist, wenn Benutzer, Dateien oder Alben gelöscht wurden.

Bei Bedarf können Sie damit auch Ihren Verlauf leeren.

![Statistik nach Album](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-f82a2632.jpg)

Statistik nach Album

![Statistik nach Foto](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-5919e257.jpg)

Statistik nach Foto

![Statistik nach Monat](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-e3bc16dc.jpg)

Statistik nach Monat

## Statistics: Ein externes Statistik-Tool in Piwigo einbinden

Möchten Sie die Statistik Ihrer Galerie mit einem Webanalyse-Tool verfolgen, das Sie bereits verwenden, etwa Google Analytics, Matomo, Piwik oder viele andere?

Das ist möglich: Aktivieren Sie dazu einfach das Plugin **Statistics**.

Sobald dieses Plugin aktiviert ist, können Sie Piwigo mit Ihrem externen Statistik-Tool verbinden. Dazu kopieren Sie den Tracking-Code (oder das Skript) Ihres Tools und fügen ihn in den Einstellungen des Plugins ein.

Sie können wählen, wo der Code eingefügt wird (Kopf- oder Fussbereich), und festlegen, ob Administratoren oder nicht angemeldete Benutzer von der Statistik ausgeschlossen werden.

!!! warning "Achtung:"
    Wenn Sie Statistik-Tools wie Google Analytics verwenden, müssen Sie die Einwilligung der Besucher Ihrer Galerie einholen. Wir empfehlen Ihnen, die Vorgaben der Behörden in den Ländern Ihrer Besucher zur Datenerfassung und zur Einholung der Einwilligung zu befolgen.

## No Stats for Robots

Die Statistik in Piwigo kann manchmal durch Besuche von Robotern (Suchmaschinen usw.) „verfälscht“ werden.

Um diese auszuschliessen, aktivieren Sie einfach das Plugin **No Stats for Robots**.

Dieses Plugin schliesst Besuche bekannter Roboter aus Ihrer Besuchsstatistik aus.
