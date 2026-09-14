---
title: Plugins zur Kommentarverwaltung - Piwigo-Dokumentation
description: "Entdecken Sie mehrere Plugins für Piwigo, mit denen Sie bei der Kommentarverwaltung weitergehen: Kommentare abonnieren, Spam vermeiden …"
---

# Kommentarverwaltung mit Plugins anpassen

Im Artikel [Kommentare verwalten](kommentare-verwalten.md) haben wir die grundlegenden Optionen zur Kommentarverwaltung in Piwigo vorgestellt. Mit mehreren Plugins können Sie aber noch weitergehen: In diesem Artikel stellen wir diese Möglichkeiten vor.

## Optionen zur Formatierung von Kommentaren

### BBCode Bar: Eine Werkzeugleiste zum Formatieren von Kommentaren hinzufügen

Wenn Benutzer ihre Kommentare formatieren können sollen (fetter Text, kursiver Text, Aufzählungspunkte …), installieren Sie einfach das Plugin **BBCode Bar**.

Dieses Plugin zeigt eine Formatierungsleiste im Kommentarfenster an. Sie können wählen, welche Optionen aktiviert werden.

![BBCode Bar.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-ff9b017e.jpg)

### Smilies Support: Smileys in Kommentaren verwenden

Wenn Benutzer Smileys in Kommentare einfügen können sollen, installieren Sie einfach das Plugin **Smilies Support**.

Mit diesem Plugin wählen Sie einen Satz Smileys für Ihre Galerie aus. Beim Schreiben eines Kommentars kann der Benutzer einen Smiley aus der Liste auswählen.

![Smilies.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-f370aea2.jpg)

!!! note "Hinweis"
    Diese Smileys sind von der Art, wie man sie aus Diskussionsforen kennt. Sie sind nicht mit Emojis zu verwechseln, die heute viel häufiger verwendet werden. Piwigo hat keine Emoji-Tastatur.

## Subscribe to Comments: Benachrichtigungen über neue Kommentare für alle aktivieren

Wenn ein Benutzer (nicht nur ein Administrator) über neue Kommentare benachrichtigt werden soll, installieren Sie einfach das Plugin **Subscribe to Comments**.

Sobald dieses Plugin aktiviert ist, kann ein Benutzer beim Schreiben eines Kommentars wählen, ob er benachrichtigt werden möchte:

- wenn ein neuer Kommentar zu diesem Foto veröffentlicht wird (das entspricht einem Abonnement der Kommentare zu diesem Foto);
- wenn ein neuer Kommentar zu einem Foto aus demselben Album veröffentlicht wird
- wenn ein neuer Kommentar auf der Website veröffentlicht wird

![Zone de commentaires.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-0f344f4b.jpg)

Ein Benutzer kann Kommentare auch abonnieren, ohne selbst einen Kommentar zu schreiben: Dazu klickt er einfach auf „Abonnieren, ohne zu kommentieren“.

Wer Kommentare abonniert hat, erhält bei jedem neuen Kommentar eine E-Mail wie unten gezeigt. In dieser E-Mail kann man auf das Bild klicken, um das Foto anzusehen, die Kommentare zu diesem Foto abbestellen und alle Kommentar-Abonnements verwalten.

![image.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-7e1f590a.png)

## Spam in den Kommentaren vermeiden

Leider sind Kommentarfelder bei Spam-Robotern oft beliebt. Deshalb ist es manchmal nötig, vorbeugende Massnahmen gegen Spam zu treffen.

Mehrere Plugins ermöglichen es, die Eingabe von Kommentaren in Piwigo zu kontrollieren.

### Comments Blacklist: Bestimmte Wörter in Kommentaren verbieten

Um eine Liste verbotener Wörter für Kommentare festzulegen, können Sie das Plugin **Comments Blacklist** installieren.

Mit diesem Plugin geben Sie eine Liste verbotener Wörter ein. Enthält ein Kommentar eines dieser Wörter, wird seine Veröffentlichung entweder blockiert oder zur Moderation zurückgehalten (je nach Ihrer Wahl).

So können Sie Wörter verbieten, die häufig in Spam-Kommentaren vorkommen, aber auch unhöfliche, beleidigende oder unangemessene Kommentare verhindern.

### Crypto Captcha: Ein Captcha im Kommentarbereich hinzufügen

Um dem Kommentarformular ein Captcha hinzuzufügen, können Sie das Plugin **Crypto Captcha** installieren.

Mit diesem Plugin müssen Benutzer ein Captcha eingeben, bevor ein Kommentar abgeschickt wird. Dieses Captcha kann auch dem Registrierungsformular für neue Benutzer hinzugefügt werden, um das Anlegen von „Fake-Konten“ zu verhindern.

Für die Einrichtung Ihres Captchas stehen mehrere Optionen zur Verfügung.

![Captcha.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-216bec65.jpg)

### RV Akismet: Kommentare mit Akismet überwachen

Mit dem Online-Dienst [Askimet](https://akismet.com/), einer Referenz auf diesem Gebiet, können Sie sicherstellen, dass die in Ihrer Galerie eingegebenen Kommentare kein Spam sind.

Installieren Sie dazu einfach das Plugin **RV Akismet**.

Sobald das Plugin aktiviert ist, müssen Sie ein Akismet-Konto erstellen: Damit erhalten Sie einen API-Schlüssel, den Sie in der Konfiguration des Plugins eingeben müssen.

!!! info "Info:"
    Sie können ein kostenloses Akismet-Konto erstellen, einige Optionen erfordern aber ein kostenpflichtiges Abonnement. Kostenlose Konten sind nur für die private, nicht kommerzielle Nutzung gedacht.

Das Plugin bietet Ihnen zwei Optionen zur Auswahl:

- Alle Kommentare abweisen, die Akismet als Spam einstuft
- Kommentare moderieren, die Akismet als Spam einstuft (das heisst, sie vor der Veröffentlichung zur Freigabe zurückhalten).

## Comments on Albums: Kommentare auf Albumseiten erlauben

Standardmässig verwaltet Piwigo Kommentare auf den Fotoseiten.

Wenn Sie möchten, können Sie aber auch einen Kommentarbereich auf den Albumseiten aktivieren.

Aktivieren Sie dazu einfach das Plugin **Comments on Albums**.

Sobald dieses Plugin aktiviert ist, fügt es auf den Albumseiten Ihrer Galerie ein Fenster zur Eingabe von Kommentaren hinzu.

Für Kommentare auf Albumseiten gelten dieselben Regeln und Einstellungen wie für Kommentare zu Fotos.

![Commentaire album.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-ded72f82.jpg)

Sobald dieses Plugin aktiviert ist, wird ein Reiter Alben hinzugefügt:

- auf der Seite zur Kommentarverwaltung im Administrationsbereich
    
    ![Commentaire sur album.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-16c3f423.jpg)
    
- auf der Seite, die die Kommentare in der Galerie auflistet
    
    ![Commentaire utilisateur.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-b2691fa8.jpg)
