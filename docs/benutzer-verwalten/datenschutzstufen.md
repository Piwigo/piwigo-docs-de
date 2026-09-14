---
title: Datenschutzstufen - Piwigo-Dokumentation
description: Mit Datenschutzstufen legen Sie die Rechte der Benutzer Ihrer Piwigo-Galerie noch genauer fest. In diesem Artikel erklären wir alles.
---

# Datenschutzstufen

## Datenschutzstufen: Wozu dienen sie?

Um festzulegen, welche Benutzer in Piwigo auf welche Inhalte zugreifen dürfen, sind Zugriffsrechte auf Alben die gängigste und praktischste Lösung.

Zur Erinnerung: Ein Album kann privat oder öffentlich sein, und Benutzer und Benutzergruppen haben entweder Zugriff auf ein privates Album oder nicht. [Mehr über die Sichtbarkeit von Alben](../alben-organisieren/zugriffsrechte-und-sichtbarkeit-von-alben.md)

Ein in Ihrer Galerie angemeldeter Benutzer sieht also nur die Alben, auf die er Zugriff hat.

In manchen Fällen müssen Sie die Rechte aber noch feiner steuern, Datei für Datei und unabhängig von den Alben. Genau dafür gibt es die „Datenschutzstufen“.

!!! warning "Achtung!"
    Dies ist eine fortgeschrittene Funktion von Piwigo, die wir Einsteigern nicht empfehlen.


## Datenschutzstufen: Wie funktionieren sie?

In Piwigo kann jede Datei einer Datenschutzstufe zugeordnet werden.

Wenn Sie ein Foto bearbeiten, legen Sie seine Datenschutzstufe im Feld „Wer soll dieses Foto sehen können?“ fest (Standard: Jeder).

![Niveau de confidentialité.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-abb3ba46.jpg)

Wenn Sie die Liste aufklappen, können Sie die Datenschutzstufe für dieses Foto auswählen.

![Niveaux de confidentialité.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-e8767701.jpg)

Wenn Sie Datenschutzstufen verwenden, muss auch jeder Benutzer einer Datenschutzstufe zugeordnet werden:

- Administratoren (Achtung: Das hat nichts mit dem Status „Administrator“ zu tun)
- Familie
- Freunde
- Kontakte
- Keine (Standard)

Die Benutzer mit der höchsten Stufe (Administratoren) haben Zugriff auf alles.

Die Benutzer der Stufe „Familie“ haben nur Zugriff auf Fotos mit den Datenschutzstufen „Familie“, „Freunde“ und „Kontakte“.

Die Benutzer der Stufe „Freunde“ haben nur Zugriff auf die Stufen „Freunde“ und „Kontakte“.

Die Benutzer der Stufe „Kontakte“ sehen nur Dateien mit der Stufe „Kontakte“.

Und Benutzer mit der Stufe „Keine“ haben nur Zugriff auf Dateien, die für „Jeder“ freigegeben sind.

Dieses Modell der Rechteverwaltung funktioniert „kaskadenartig“. Es ist nicht ganz leicht zu verstehen und relativ „starr“. Deshalb empfehlen wir es Einsteigern eher nicht.

!!! info "Info:"
    Wenn Ihnen die Bezeichnungen Administratoren, Familie, Freunde und Kontakte nicht gefallen: Sie lassen sich anpassen, bei einem Konto auf Piwigo Cloud über den Support, bei einem selbst gehosteten Piwigo direkt in der Datenbank. Eine weitere Datenschutzstufe hinzuzufügen ist jedoch nicht möglich.
