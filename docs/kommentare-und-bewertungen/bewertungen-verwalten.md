---
title: Bewertungen verwalten
description: In diesem Artikel erfahren Sie, wie Sie Besuchern Ihrer Piwigo-Galerie erlauben, Ihre Fotos zu bewerten.
---

# Bewertungen verwalten

Mit Piwigo können Sie Besuchern Ihrer Galerie erlauben, Fotos und andere Dateien zu bewerten, indem sie ihnen eine bestimmte Anzahl Sterne vergeben. So können Sie ein Abstimmungssystem einrichten, zum Beispiel für Fotowettbewerbe.

## Bewertungen aktivieren oder deaktivieren

Um Bewertungen zu aktivieren oder zu deaktivieren, öffnen Sie im Administrationsbereich das Menü Konfiguration > Optionen.

Aktivieren oder deaktivieren Sie im Abschnitt „Zugriffsrechte“ die Option „**Bewertungen von Fotos erlauben**“.

Wenn Sie dieses Kästchen aktivieren, erscheint eine weitere Option: „Bewertungen durch Gäste erlauben“. Aktivieren Sie diese Option, wenn alle Besucher (auch anonyme) eine Datei bewerten dürfen. Deaktivieren Sie sie, wenn diese Funktion nur angemeldeten Benutzern Ihrer Galerie vorbehalten sein soll.

## Bewertungen in Ihrer Galerie anzeigen

Wenn Bewertungen in Ihrer Galerie aktiviert sind, erscheinen neben einem Foto zwei neue Angaben:

- Bewertung: Hier werden die Punktzahl des Fotos (also die nach Anzahl der Bewertungen gewichtete Durchschnittsbewertung) und die Anzahl der Stimmen angezeigt.
- Foto bewerten: Hier können Besucher das Foto bewerten, indem sie auf die gewünschte Anzahl Sterne klicken (1 Stern = 0, 6 Sterne = 5). Ein Benutzer kann seine Bewertung jederzeit ändern.

![Score et note.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-91833265.jpg)

Wenn Bewertungen aktiviert sind, wird Ihrer Galerie der Bereich „Am besten bewertet“ hinzugefügt.

Dort sehen Sie alle bewerteten Fotos, sortiert nach Punktzahl (von der höchsten zur niedrigsten).

![Mieux notées.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-3f36fdac.jpg)

!!! info "Warum eine gewichtete Punktzahl statt einer Durchschnittsbewertung?"
    
    Bei der Durchschnittsbewertung würde ein Foto mit einer einzigen Bewertung von 5/5 besser abschneiden als ein Foto mit 500 Bewertungen und einem Durchschnitt von 4,8/5. Für einen Wettbewerb ist das nicht sinnvoll.


## Bewertungen im Administrationsbereich verwalten

Um Bewertungen im Administrationsbereich zu verwalten, öffnen Sie das Menü Fotos > Bewertungen.

Diese Seite enthält zwei Tabs: „Fotos“ und „Benutzer“.

### Bewertungen nach Foto

Der Tab „Fotos“ zeigt die Liste der bewerteten Fotos und zu jedem Foto alle Informationen zu seinen Bewertungen (Anzahl der Bewertungen, Punktzahl, Durchschnittsbewertung, Summe der Bewertungen, Benutzer, die abgestimmt haben, Datum der Stimmen…).

Sie können diese Liste nach verschiedenen Kriterien sortieren. Ausserdem können Sie die Bewertungen nach Benutzertyp filtern (angemeldete Benutzer oder anonyme Gäste). Schliesslich können Sie die Liste auch nach Album filtern.

Mit einem Klick auf den Papierkorb rechts in jeder Zeile löschen Sie alle Bewertungen eines Fotos und setzen seine Punktzahl zurück.

Um ein Foto zu bearbeiten, klicken Sie auf sein Vorschaubild: Sie werden dann zur Bearbeitungsseite des Fotos weitergeleitet.

![Toutes les notes.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-ae35fb19.jpg)

### Bewertungen nach Benutzer

Der Tab „Benutzer“ zeigt die Liste der Benutzer, die Fotos bewertet haben, und zu jedem Benutzer alle Informationen zu seinen Bewertungen (Datum der letzten Bewertung, Anzahl der Bewertungen, Durchschnittsbewertung, Verteilung der Stimmen auf die einzelnen Bewertungsstufen…).

Sie können die Liste so filtern, dass nur Benutzer angezeigt werden, die mehr als eine bestimmte Anzahl Bewertungen abgegeben haben.

Mit einem Klick auf den Papierkorb rechts in der Zeile löschen Sie alle Bewertungen eines Benutzers.

![Tous les noteurs.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-edd593fe.jpg)

## Alle Bewertungen zurücksetzen

Mit dem Plugin Delete Hit/Rate können Sie alle Bewertungen zurücksetzen:

- eines bestimmten Fotos, direkt in der Fotobearbeitung
- aller Fotos eines Albums, direkt in der Albumbearbeitung

Ausserdem können Sie damit alle Bewertungen der Galerie auf der Seite Werkzeuge > Wartung zurücksetzen.
