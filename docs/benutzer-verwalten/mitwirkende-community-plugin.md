---
title: Community-Plugin - Piwigo-Dokumentation
description: Mit dem Plugin Community verwalten Sie Mitwirkende, das heisst, Sie erlauben Benutzern ohne Administratorstatus, Dateien in Piwigo zu importieren.
---

# Mitwirkende verwalten (Community-Plugin)

## Wozu dient das Plugin Community?

Standardmässig dürfen in Piwigo nur Administratoren Inhalte in Ihre Fotosammlung hochladen.

Manchmal möchten Sie aber einigen Benutzern erlauben, Dateien zu importieren, ohne ihnen den Administratorstatus zu geben. Einige Beispiele aus einer Organisation:

- Sie arbeiten mit einem Fotografen zusammen und möchten Zeit sparen: Er soll seine neuesten Aufnahmen direkt in Piwigo hochladen, damit Sie sie dort sortieren können, statt sie per CD oder Dateiübertragung zu schicken;
- Einige Mitglieder Ihres Teams erstellen Dateien (bearbeitete Fotos, Grafiken, Broschüren usw.); sie sollen nicht jedes Mal einen Administrator bitten müssen, ihre Inhalte in Piwigo zu importieren, aber Sie möchten ihnen auch keinen Zugriff auf den Administrationsbereich geben.
- Mitarbeitende im Aussendienst müssen vor Ort aufgenommene Fotos schicken (Servicetechniker, Bauleiter, Baustellenaufsicht usw.). Wenn sie Fotos direkt zu Piwigo hinzufügen können, spart das allen Zeit (besonders, wenn sie [die mobile Piwigo-App](../mobile-apps/index.md) für iOS oder Android nutzen!).

Wenn Sie Piwigo in der Familie, im Freundeskreis oder im Verein nutzen, können Sie auch anderen Personen ermöglichen, ihre Fotos in Ihre Piwigo-Galerie zu schicken.

All diese Benutzer, die keine Administratoren sind, aber Inhalte in Piwigo importieren dürfen, nennen wir hier **Mitwirkende**.

Um diese Funktion zu aktivieren, müssen Sie das Plugin **Community** installieren.

!!! info "Wenn Sie Kunde von Piwigo Cloud sind, ist dieses Plugin erst ab dem Tarif Team verfügbar."

## Festlegen, welche Benutzer Fotos schicken dürfen und mit welchen Rechten

Sobald das Plugin Community aktiviert ist, öffnen Sie seine Einstellungen mit einem Klick auf „Einstellungen“.

![Plugin Community.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-09c97702.jpg)

Auf der ersten Registerkarte legen Sie die Zugriffsrechte und Optionen von Community fest.

Standardmässig ist bereits ein Zugriffsrecht angelegt, das alle registrierten Benutzer zu Mitwirkenden macht.

Sie können dieses Zugriffsrecht mit einem Klick auf das Bearbeiten-Symbol ändern oder mit einem Klick auf das Löschen-Symbol (das Kreuz) entfernen.

![Page Community.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-e7d5db8b.jpg)

Mit einem Klick auf „Zugriffsrecht hinzufügen“ können Sie auch ein neues Zugriffsrecht anlegen.

Nach einem Klick auf „Zugriffsrecht hinzufügen“ sehen Sie die verschiedenen verfügbaren Optionen.

![Ajout de permission.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-c2139294.jpg)

**Wer?**

Legen Sie hier fest, wer Fotos aus der Galerie heraus hinzufügen darf:

- Jeder Besucher (auch anonym)
- Jeder registrierte Benutzer
- Ein bestimmter Benutzer: Sie können diesen Benutzer dann auswählen
- Eine Gruppe: Sie können eine Gruppe „Mitwirkende“ anlegen, das ist am praktischsten. [Mehr über Benutzergruppen erfahren](benutzergruppen.md)

**Wo?**

Wählen Sie hier, in welchem Bereich der Galerie Mitwirkende Fotos hinzufügen dürfen:

- In der ganzen Galerie (in jedem Album)
- In einem bestimmten Album

!!! info "Info:"
    Beim Aktivieren des Plugins Community wird standardmässig ein neues Album „Community“ angelegt. Sie können festlegen, dass die Fotos der Mitwirkenden zuerst in diesem Album landen, damit ein Administrator sie sortieren und freigeben kann.

Wenn Sie „Einstellungen für Unteralben übernehmen“ auswählen, dürfen Benutzer Fotos im gewählten Album UND in seinen Unteralben hinzufügen.

Wenn Sie „Unteralben erstellen können“ auswählen, dürfen Benutzer beim Hochladen von Fotos ein neues Album erstellen.

**Welche Vertrauensstufe?**

Sie haben die Wahl zwischen zwei Optionen:

- Geringes Vertrauen: Hochgeladene Fotos müssen von einem Administrator freigegeben werden, bevor sie in der Galerie sichtbar sind.
- Hohes Vertrauen: Von Mitwirkenden hochgeladene Fotos sind sofort in der Galerie sichtbar.

**Weitere Optionen**

Ausserdem können Sie:

- die Anzahl der Fotos begrenzen, die Mitwirkende hinzufügen dürfen (Limit pro Benutzer)
- den Speicherplatz begrenzen, den die von Mitwirkenden hochgeladenen Fotos belegen (Limit pro Benutzer)

Standardmässig sind diese Werte unbegrenzt.

Klicken Sie auf „Hinzufügen“: Das Zugriffsrecht ist angelegt.

Wenn Sie verschiedene Arten von Mitwirkenden mit unterschiedlichen Rechten verwalten möchten, müssen Sie mehrere Zugriffsrechte anlegen.

**Automatisches Erstellen eines Albums pro Mitwirkendem**

Wenn Sie möchten, kann Piwigo für jeden Mitwirkenden bei seiner ersten Anmeldung automatisch ein neues Album erstellen.

Öffnen Sie dazu in den Einstellungen des Plugins Community die Registerkarte „Konfiguration“.

![Configuration de Community.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-654efc11.jpg)

Wenn Sie diese Option auswählen, können Sie festlegen, in welchem Album die Alben der einzelnen Mitwirkenden erstellt werden.

## Für Mitwirkende: Wie füge ich mit Community Fotos in Piwigo hinzu?

Benutzer, die Fotos zur Galerie hinzufügen dürfen, sehen im Menü „Erkunden“ einen neuen Menüpunkt „Bilder hochladen“.

![Ajout photos Community.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-ba709fad.jpg)

!!! note "Hinweis:"
    Das Menü „Bilder hochladen“ kann auf der Startseite rechts neben dem Menü „Erkunden“ angezeigt werden. Installieren Sie dazu das Plugin Upload 1 Menu. Wenn Sie Kunde von Piwigo Cloud sind, ist dieses Plugin erst ab dem Tarif Team verfügbar.


Über das Menü „Bilder hochladen“ gelangen Sie zur Seite zum Hochladen von Fotos.

![Ecran ajout photos Community.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-1c98b145.jpg)

Der Benutzer kann:

- das Album auswählen, in das die Fotos hinzugefügt werden (nur freigegebene Alben stehen zur Auswahl)
- ein neues Album erstellen (wenn er das darf)
- Fotos von seinem Computer hinzufügen (mit einem Klick auf „Fotos hinzufügen“ oder per Drag-and-drop)
- die Eigenschaften der Fotos (Titel, Autor, Beschreibung) festlegen, mit einem Klick auf „Fotoeigenschaften festlegen“

Die Schaltfläche „Übertragung starten“ schickt die Fotos an Piwigo.

Je nach Vertrauensstufe, die beim Anlegen des Zugriffsrechts gewählt wurde, werden die Fotos entweder:

- sofort in der Galerie angezeigt
- oder müssen erst von einem Administrator freigegeben werden

### Hinzugefügte Fotos als Mitwirkender ansehen und bearbeiten

Als Mitwirkender haben Sie im Hauptmenü „Erkunden“ Zugriff auf den Menüpunkt „Fotos bearbeiten“.

Auf dieser Seite sehen Sie die Fotos, die Sie hinzugefügt haben. Fotos, die noch auf ihre Freigabe warten, sind mit „Wartend“ gekennzeichnet.

![Menu Edit Photos Community.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-a5ba48be.jpg)

Auf dieser Seite können Sie hinzugefügte Fotos löschen und ihnen Schlagworte hinzufügen.

Um Fotos zu bearbeiten, klicken Sie auf die gewünschten Fotos, um sie der Auswahl hinzuzufügen, oder verwenden Sie die Schaltflächen „Alles“, „Nichts“ und „Invertieren“.

Klicken Sie dann auf die Dropdown-Liste „Aktion“, um die gewünschte Aktion auszuwählen:

- Ausgewählte Fotos löschen
- Schlagworte hinzufügen

![Choisir une action.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-a2c8d348.jpg)

## Für Administratoren: Wie gebe ich die von Mitwirkenden mit Community hinzugefügten Fotos frei?

Wenn Sie in den Einstellungen des Plugins Community die Option „Geringes Vertrauen“ gewählt haben (siehe erstes Kapitel dieser Seite), müssen die von Benutzern hinzugefügten Fotos von einem Administrator freigegeben werden, bevor sie in der Galerie erscheinen.

Es gibt mehrere Möglichkeiten, die Fotos zu sehen, die auf die Freigabe durch einen Administrator warten.

### Benachrichtigung per E-Mail

Die Administratoren erhalten jedes Mal eine E-Mail, wenn Fotos hinzugefügt werden. Diese E-Mail enthält einen Link, über den sie die Fotos direkt prüfen und freigeben können.

![Notification nouveaux ajouts.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-ab56a7a6.jpg)

### Dashboard von Piwigo

Wenn Fotos auf ihre Freigabe warten, werden die Administratoren durch ein Banner auf der Startseite des Administrationsbereichs von Piwigo (dem Dashboard) darauf hingewiesen.

### Ausstehende Fotos freigeben

Über den Link in der E-Mail oder auf der Startseite des Administrationsbereichs gelangen Sie zu den Einstellungen von Community, auf die Registerkarte „Ausstehende Fotos“.

Diese Registerkarte listet die Fotos auf, die auf ihre Freigabe warten.

![Décision photos Community.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-969920ba.jpg)

Zu jedem Foto sehen Sie seine Einstellungen. Mit einem Klick auf „Zoom“ vergrössern Sie es, mit einem Klick auf „Bearbeiten“ bearbeiten Sie es. So können Sie die Eigenschaften des Bildes (Titel, Beschreibung, Album, Schlagworte usw.) anpassen, bevor Sie es endgültig online stellen.

Ausserdem können Sie die Datenschutzstufe der Fotos über die Dropdown-Liste unter dem Text „Wer soll dieses Foto sehen können?“ anpassen (mehr über [Datenschutzstufen](datenschutzstufen.md)). Wenn Sie keine Datenschutzstufen verwenden, lassen Sie die Dropdown-Liste einfach auf „Jeder“.

Wählen Sie dann einfach die Fotos aus und klicken Sie auf „Validieren“ (Fotos veröffentlichen) oder „Abweisen“ (Hochladen der Fotos ablehnen).

## Ergänzende Plugins zum Plugin Community

Einige Plugins sind für Piwigo-Galerien nützlich, die das Plugin Community verwenden. Hier ist die Liste.

!!! info "Wenn Sie Kunde von Piwigo Cloud sind, sind diese Plugins erst ab dem Tarif Team verfügbar."

### Upload 1 Menu

Mit diesem Plugin zeigen Sie das Menü „Bilder hochladen“ auf der Startseite der Galerie neben dem Menü „Erkunden“ an.

![Upload 1 Menu.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-78529d2b.jpg)

### See My Photos

Mit diesem Plugin zeigen Sie in der Galerie ein Menü „Meine Fotos“ an. So kann jeder Benutzer die Fotos, die er zur Galerie hinzugefügt hat, über alle Alben hinweg einfach ansehen.

[Mehr erfahren](../ihre-galerie-anpassen/menue-und-navigationsleiste-anpassen.md)

### See photos by user

Mit diesem Plugin können die Besucher der Galerie Fotos einfach nach dem Benutzer filtern, der sie hinzugefügt hat.

[Mehr erfahren](../ihre-galerie-anpassen/menue-und-navigationsleiste-anpassen.md)

### Photo added by

Mit diesem Plugin zeigen Sie auf der Seite eines Fotos im Feld „Foto hinzugefügt von“ die Kennung des Benutzers an, der das Foto hinzugefügt hat.

![Photo ajoutée par.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-0785b63f.jpg)

In den Einstellungen des Plugins legen Sie fest, wo diese Information angezeigt wird (standardmässig direkt vor „Alben“).

Wenn das Plugin See photos by user aktiviert ist, können Sie den Benutzernamen anklickbar machen. Er führt dann zur Seite, die alle von diesem Benutzer hinzugefügten Fotos auflistet.
