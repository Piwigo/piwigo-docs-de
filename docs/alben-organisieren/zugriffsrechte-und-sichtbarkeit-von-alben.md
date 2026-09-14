---
title: Zugriffsrechte und Sichtbarkeit von Alben - Piwigo-Dokumentation
description: In diesem Kapitel sehen wir uns an, wie Sie in Piwigo die Zugriffsrechte für Alben verwalten und bearbeiten, also den Status der Alben (privat / öffentlich) und die Rechte der Benutzer auf die Alben.
---

# Zugriffsrechte und Sichtbarkeit von Alben

In diesem Kapitel sehen wir uns an, wie Sie in Piwigo die Zugriffsrechte für Alben verwalten und bearbeiten, also den Status der Alben (privat / öffentlich) und die Rechte der Benutzer auf die Alben.

Ausserdem sehen wir, wie Sie diese Eigenschaften von Alben einfach ansehen und ändern können:

- gesperrte / entsperrte Alben
- Kommentare für Alben aktivieren
- Alben, deren Fotos heruntergeladen werden dürfen oder nicht

## Wie funktionieren Zugriffsrechte für Alben?

Wenn Sie in Piwigo ein Album erstellen: Wer darf seinen Inhalt sehen? Wie ändern Sie das? Welche Regeln gelten für Unteralben?

Dabei gibt es einiges zu beachten.

### Private und öffentliche Alben

Zunächst ist wichtig: Ein Album kann in Piwigo privat oder öffentlich sein.

**Öffentliche Alben** sind für alle Besucher Ihrer Fotobibliothek sichtbar, die nicht angemeldet sind (also kein Konto haben: Das entspricht dem speziellen Benutzer „Gast“).

Sobald jemand die Website Ihrer Galerie im Internet besucht, ohne sich anzumelden, kann er die öffentlichen Alben sehen, und nur diese.

**Private Alben** hingegen sind nur für identifizierte Benutzer zugänglich, die mit ihrem Benutzernamen und Passwort angemeldet sind.

Für jedes private Album können Sie festlegen, welche Benutzer und Benutzergruppen es sehen dürfen.

!!! info "Info:"
    Ein neues Stammalbum ist in Piwigo standardmässig immer öffentlich. Wenn Sie das ändern möchten, wenden Sie sich an den Support, falls Sie Kunde von Piwigo Cloud sind. Andernfalls fügen Sie mit [LocalFiles Editor](../piwigo-selbst-hosten/lokale-konfiguration-bearbeiten-localfiles-editor.md) folgende Einstellung zu Ihrer Konfiguration hinzu: `$conf['newcat_default_status'] = 'private';`

### Zugriffsrechte für ein Album bearbeiten

Um die Zugriffsrechte für ein Album zu ändern, müssen Sie dieses Album bearbeiten:

- entweder in Ihrer Galerie, indem Sie die Seite des Albums öffnen und auf das Bearbeiten-Symbol klicken;
- oder im Administrationsbereich, indem Sie die Albenliste öffnen (Menü Alben > Verwaltung) und auf das Bearbeiten-Symbol klicken.

[Mehr über das Bearbeiten von Alben erfahren](ein-album-bearbeiten.md)

Klicken Sie in der Album-Bearbeitung auf den Tab „Zugriffsrechte“. Hier legen Sie den Status Ihres Albums fest (öffentlich oder privat).

![Permissions.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-37a2ed66.jpg)

Wenn Sie ein Album privat machen, können Sie festlegen, welche Benutzer seinen Inhalt sehen dürfen.

Sie können Zugriffsrechte vergeben:

- an eine oder mehrere Benutzergruppen
- an einen oder mehrere bestimmte Benutzer

![Accès privé.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-84a5d6f8.jpg)

Mehr über Benutzergruppen erfahren Sie [in diesem Artikel](../benutzer-verwalten/benutzergruppen.md).

!!! warning "Achtung!"
    Ein privates Album sieht in der Galerie niemand, nicht einmal Administratoren! Vergeben Sie sich deshalb unbedingt selbst die Rechte für jedes private Album, das Sie erstellen.

Mit dem Kontrollkästchen „Einstellungen für Unteralben übernehmen“ können Sie die Zugriffsrechte eines Albums in einem Schritt ändern und diese Änderungen auf alle bestehenden Unteralben übertragen.

!!! warning "Achtung: Diese Änderung gilt nicht für Unteralben, die Sie später erstellen."

### Regeln für Zugriffsrechte in der Albenhierarchie

Ein Unteralbum, das Sie in einem öffentlichen Album erstellen, ist standardmässig öffentlich.

Ein Unteralbum, das Sie in einem privaten Album erstellen, ist privat. Ausserdem ist es standardmässig für alle Administratoren zugänglich, genau wie alle übergeordneten Alben.

Wenn Sie ein Album öffentlich machen, dessen übergeordnete Alben privat sind, werden die übergeordneten Alben automatisch ebenfalls öffentlich.

Wenn Sie ein Album privat machen, dessen Unteralben öffentlich sind, werden die Unteralben automatisch ebenfalls privat.

Abgesehen vom Status (privat / öffentlich) übernehmen Unteralben die Zugriffsrechte ihrer übergeordneten Alben nicht automatisch.

Ein Beispiel: Sie haben ein privates Album, auf das die Benutzer X und Y Zugriff haben. Wenn Sie in diesem privaten Album ein Unteralbum erstellen, haben die Benutzer X und Y standardmässig keinen Zugriff darauf (nur die Administratoren).

!!! info "Info:"
    Wenn Unteralben die Zugriffsrechte ihrer übergeordneten Alben automatisch übernehmen sollen, wenden Sie sich an den Support, falls Sie Kunde von Piwigo Cloud sind. Andernfalls fügen Sie mit [LocalFiles Editor](../piwigo-selbst-hosten/lokale-konfiguration-bearbeiten-localfiles-editor.md) folgende Einstellung zu Ihrer Konfiguration hinzu: `$conf['inheritance_by_default'];`

## Zugangsart mehrerer Alben gleichzeitig verwalten (öffentlich / privat)

Um die Zugangsart Ihrer Alben (öffentlich / privat) auf einen Blick zu sehen und zu ändern, öffnen Sie im Administrationsbereich das Menü Alben > Eigenschaften.

Im ersten Tab können Sie ein Album ganz einfach von öffentlich auf privat umstellen und umgekehrt.

![Propriétés albums.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-37a751a9.jpg)

Auf dieser Seite sehen Sie alle Alben und Unteralben Ihrer Fotobibliothek, jeweils in der Spalte, die ihrem Status entspricht („Öffentlich“ und „Privat“).

!!! info "Unteralben erkennen Sie leicht, da ihr Name so angezeigt wird: Stammalbum / Unteralbum 1 / Unteralbum 2"

Um ein Album von öffentlich auf privat umzustellen, klicken Sie einfach auf das Album und dann auf den Pfeil unter der ersten Spalte: Das Album wird in die Spalte „Privat“ verschoben. Um ein privates Album öffentlich zu machen, gehen Sie umgekehrt vor!

Sie können mehrere Alben auswählen, genau wie Dateien auf Ihrem Computer:

- Mehrere aufeinanderfolgende Alben bearbeiten: Klicken Sie auf das erste gewünschte Album, halten Sie die Umschalttaste gedrückt und klicken Sie auf das letzte gewünschte Album: Alle Alben dazwischen sind ausgewählt.
- Mehrere Alben bearbeiten, die in der Liste nicht aufeinanderfolgen: Klicken Sie auf das erste gewünschte Album, halten Sie die Taste Ctrl bzw. Cmd gedrückt und klicken Sie nacheinander auf die weiteren Alben, bis alle gewünschten Alben ausgewählt sind.

### Sonderfall: Alben mit Unteralben

Wenn Sie ein Album mit Unteralben auf privat umstellen, werden auch alle seine Unteralben privat.

Wenn Sie hingegen ein Unteralbum auf öffentlich umstellen, wird sein übergeordnetes Album automatisch ebenfalls öffentlich. Denn man muss Zugriff auf ein Album haben, um auf eines seiner Unteralben zugreifen zu können.

Unten sehen Sie ein konkretes Beispiel.

![Propriétés.gif](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-9e8786bc.gif)

## Sichtbarkeit mehrerer Alben gleichzeitig verwalten (gesperrt / entsperrt)

Um mehrere Alben Ihrer Galerie zu sperren oder zu entsperren, öffnen Sie im Administrationsbereich das Menü Alben > Eigenschaften.

Der zweite Tab funktioniert genauso wie der erste (siehe vorheriger Abschnitt), nur dass Sie hier Alben sperren und entsperren.

!!! info "Info:"
    Ein gesperrtes Album ist in der Galerie nicht zugänglich, ausser für Administratoren. Meist wird der Status „gesperrt“ verwendet, wenn ein Album noch nicht bereit ist, in der Galerie veröffentlicht zu werden, weil ein Administrator daran arbeitet (Vorbereitung vor der Veröffentlichung, Wartung…). Es handelt sich also um einen vorübergehenden „Arbeitsstatus“.

Um ein einzelnes Album zu sperren oder zu entsperren, können Sie auch einfach dieses Album bearbeiten.

## Kommentare für mehrere Alben gleichzeitig verwalten

Wenn Sie Kommentare in Ihrer Galerie aktiviert haben, sehen Sie auf einen Blick, welche Alben für Kommentare offen sind und welche nicht. Öffnen Sie dazu im Administrationsbereich das Menü Alben > Eigenschaften.

Der dritte Tab funktioniert genauso wie die beiden anderen (siehe vorherige Abschnitte).

Mehr über Kommentare erfahren Sie [in diesem Artikel](../kommentare-und-bewertungen/kommentare-verwalten.md).

## Download Permissions: Download-Rechte für jedes Album verwalten

Standardmässig können Benutzer, die Fotos herunterladen dürfen, in Piwigo alle Fotos der Galerie herunterladen.

Wenn Sie die Rechte für jedes Album einzeln verwalten möchten, können Sie das Plugin **Download Permissions** installieren.

!!! info "Wenn Sie Kunde von Piwigo Cloud sind, ist dieses Plugin erst ab dem Enterprise-Tarif verfügbar."

Es fügt der Seite Alben > Eigenschaften einen neuen Tab hinzu. Dort legen Sie, genau wie in den anderen Tabs, fest, in welchen Alben Benutzer Fotos herunterladen dürfen.

![Téléchargement.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-1fd60f62.jpg)
