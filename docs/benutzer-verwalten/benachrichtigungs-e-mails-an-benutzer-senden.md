---
title: E-Mail-Benachrichtigungen - Piwigo-Dokumentation
description: Wie senden Sie Benachrichtigungs-E-Mails an die Benutzer Ihrer Piwigo-Galerie? In diesem Artikel erklären wir alles.
---

# Benachrichtigungs-E-Mails an Benutzer senden

Manchmal möchten Sie bestimmten Piwigo-Benutzern eine E-Mail senden, um sie über neue Fotos oder neu erstellte Alben zu informieren.

Dafür gibt es zwei Möglichkeiten.

## Benachrichtigungen zu einem Album

Im Administrationsbereich können Sie Benutzern oder Benutzergruppen eine E-Mail zu einem bestimmten Album senden.

So erfahren sie, dass ein neues Album erstellt oder ein Album geändert wurde.

Öffnen Sie dazu Alben > Verwaltung, bearbeiten Sie das betreffende Album und wechseln Sie zum Tab „Benachrichtigungen“.

In diesem Tab legen Sie fest, welche Benutzer oder Benutzergruppen benachrichtigt werden, und können bei Bedarf eine zusätzliche Nachricht eingeben.

![Notification sur album.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-7f0dc72d.jpg)

Die betreffenden Personen erhalten eine E-Mail mit einem Link zum Album und Ihrer Nachricht.

![Email de notification.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-fed62f4c.jpg)

!!! warning "Achtung:"
    Prüfen Sie vor dem Senden einer Benachrichtigung im Tab „Zugriffsrechte“, ob die Benutzer Zugriff auf dieses Album haben.

## Allgemeine Benachrichtigungen

Sie können auch E-Mails einrichten, die Benutzer über alle neuen Inhalte der Galerie seit ihrer letzten Anmeldung informieren.

!!! warning "Achtung: Nur Benutzer mit dem Status „Webmaster“ haben Zugriff auf diese Funktion."

Öffnen Sie dazu Benutzer > Benachrichtigungen.

### Einstellungen der E-Mails

Im ersten Tab „Einstellungen“ legen Sie die Einstellungen für die versendeten E-Mails fest:

![Paramètres email.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-7419dacb.jpg)

- E-Mail im HTML-Format senden: Wenn Sie „Ja“ wählen, wird die E-Mail mit Links, Bildern und Farben gestaltet. Wenn Sie „Nein“ wählen, wird die E-Mail als reiner Text verschickt.
- E-Mail senden als: der Name des Absenders, der in der E-Mail angezeigt wird. Standardmässig ist das der Name Ihrer Piwigo-Galerie.
- Detaillierten Inhalt hinzufügen: Wenn Sie „Ja“ wählen, enthält die E-Mail Details zu den Änderungen (Anzahl neuer Fotos, aktualisierter Alben, neuer Benutzer).
- Zusätzlicher Inhalt der E-Mail: Hier legen Sie eine eigene Nachricht fest, die den versendeten E-Mails standardmässig hinzugefügt wird.
- Die neuesten Bilder gruppiert nach Datum in die E-Mail einbinden: Wenn Sie „Ja“ wählen, enthält die E-Mail alle neu hinzugefügten Fotos, sortiert nach Datum des Hochladens.

### Festlegen, welche Benutzer benachrichtigt werden

Im Tab „Abonnements“ legen Sie fest, welche Benutzer Benachrichtigungs-E-Mails erhalten.

Um Benutzer an- oder abzumelden, verschieben Sie sie mit einem Klick auf die orangefarbenen Pfeile in die linke Spalte.

![Abonnement notifications.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-3f0dd524.jpg)

Wenn ein Benutzer angemeldet wird, erhält er eine Bestätigungs-E-Mail. Wenn er möchte, kann er sich wieder abmelden.

![Notification abonnement.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-8f0f2f3c.jpg)

### Eine Benachrichtigungs-E-Mail senden

Im Tab „Senden“ lösen Sie den Versand einer E-Mail aus.

![Envoi de mail.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-b08ba16a.jpg)

Der Bereich „Empfänger auswählen“ zeigt die Benutzer, die die Benachrichtigungen abonniert haben und betroffen sind (das heisst, seit ihrer letzten Benachrichtigung gibt es neue Inhalte in Piwigo). Sie können auswählen, welche Benutzer eine E-Mail erhalten sollen, oder die Auswahl aufheben.

Der Bereich „Zusätzlicher Inhalt der E-Mail“ zeigt die Standardnachricht aus den Einstellungen, die Sie hier anpassen können.

Klicken Sie auf „Senden“, um den Versand der E-Mail auszulösen.

![Nouvelles photos.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-db8a2c92.jpg)

## Protect Notification: Absender der Benachrichtigungs-E-Mails ändern

Manchmal landen die Benachrichtigungs-E-Mails von Piwigo im Spam-Ordner. Das liegt daran, dass sie mit der E-Mail-Adresse des Hauptadministrators (Webmasters) verschickt werden. Da der Cloud-Server von Piwigo keine E-Mails von dieser Adresse versenden darf, werden die E-Mails als unsicher eingestuft.

Um dieses Problem zu lösen, können Sie das Plugin **Protect Notif** installieren.

Sobald dieses Plugin aktiviert ist, werden alle Benachrichtigungs-E-Mails von Piwigo von einer fiktiven Adresse wie „no-reply@photolibrary.piwigo.com“ verschickt.

So werden die Benachrichtigungs-E-Mails zuverlässig zugestellt.

!!! info "Seit Februar 2024 ist Protect Notif bei allen neuen Konten auf Piwigo Cloud standardmässig aktiviert."
