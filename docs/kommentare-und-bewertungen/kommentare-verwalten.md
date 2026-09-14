---
title: Kommentare verwalten - Piwigo-Dokumentation
description: Mit Piwigo können Sie den Benutzern Ihrer Galerie erlauben, die Inhalte Ihrer Fotobibliothek zu kommentieren.
---

# Kommentare verwalten

Mit Piwigo können Sie den Benutzern Ihrer Galerie erlauben, die Inhalte Ihrer Fotobibliothek zu kommentieren.

## Kommentare in Ihrer Galerie aktivieren oder deaktivieren

Um Kommentare in Ihrer Galerie zu aktivieren oder zu deaktivieren, öffnen Sie im Administrationsbereich das Menü Konfiguration > Optionen und dann den Reiter Kommentare.

Um Kommentare zu aktivieren, wählen Sie die Option „Kommentare aktivieren“ und speichern Sie die Einstellungen. Nehmen Sie sich aber zuerst die Zeit, die verfügbaren Optionen anzusehen (siehe nächstes Kapitel)!

## Optionen zur Kommentarverwaltung

Sobald die Option „Kommentare aktivieren“ ausgewählt ist, erscheinen mehrere Unteroptionen: Sehen Sie sich diese aufmerksam an!

![Configuration commentaires.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-c8c4a805.jpg)

Einige Erläuterungen zu diesen Optionen:

- **Kommentare für alle erlauben**: Wenn Sie diese Option wählen, können auch anonyme Besucher (die nicht in Ihrer Galerie angemeldet sind) einen Kommentar hinterlassen;
- **Freigabe der Kommentare durch den Administrator erforderlich**: Wenn Sie diese Option wählen, werden Kommentare nicht sofort veröffentlicht. Ein Administrator muss sie zuerst freigeben, bevor sie in Ihrer Galerie sichtbar werden.
- **Administratoren bei folgenden Kommentar-Änderungen benachrichtigen**: Wenn Sie die Freigabe durch den Administrator gewählt haben, empfehlen wir, die Benachrichtigung der Administratoren zu aktivieren, wenn ein Kommentar **auf Freigabe wartet**. Sie können Administratoren auch nur informieren, wenn ein Kommentar veröffentlicht wird, ohne dass sie ihn freigeben müssen. Wählen Sie dazu die Benachrichtigung, wenn ein Kommentar **hinzugefügt** wurde.

### Einige Tipps gegen Spam in den Kommentaren

Standardmässig ist eine Prüfung eingerichtet, um Missbrauch zu verhindern: Versucht ein Benutzer, innerhalb sehr kurzer Zeit von derselben IP-Adresse aus mehrere Kommentare zu einem Foto zu veröffentlichen, blockiert das System den zweiten Kommentar.

Damit sind aber nicht alle Probleme gelöst.

Wenn Ihre Galerie öffentlich ist und Sie Kommentare von anonymen Benutzern zulassen, gehen Sie ein Risiko ein: Ihre Kommentare könnten von Spam-Bots zugemüllt werden.

Um das zu vermeiden, empfehlen wir einige bewährte Vorgehensweisen:

- Wählen Sie die Option „Benutzer erlauben, einen Link Ihrer Webseite einzufügen“ nicht aus: Wenn jeder auf einer Website kommentieren kann, ist diese Option bei Spammern sehr beliebt;
- Verlangen Sie von Benutzern Angaben, bevor sie einen Kommentar hinterlassen können (E-Mail-Adresse, Benutzername)
- Fügen Sie bei Bedarf eine Spam-Kontrolle für Kommentare hinzu (mehr dazu auf der Seite [Plugins zur Kommentarverwaltung](plugins-zur-kommentarverwaltung.md))

## Darstellung der Kommentare in der Galerie

In Ihrer Galerie werden Kommentare auf der Fotoseite unterhalb des Fotos angezeigt (bei den meisten Erscheinungsbildern).

Wenn Kommentare nur für angemeldete Benutzer erlaubt sind, sehen anonyme Besucher die Anzahl der Kommentare und können die veröffentlichten Kommentare lesen. Das Formular zum Verfassen eines Kommentars wird ihnen aber nicht angezeigt.

### Darstellung der Kommentare mit dem Erscheinungsbild Modus

In Galerien mit dem Erscheinungsbild Modus wird das Eingabeformular für neue Kommentare bei jedem Foto links angezeigt, die Liste der bereits veröffentlichten Kommentare rechts.

![Espace commentaires.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-b84b8dea.jpg)

### Darstellung der Kommentare mit dem Erscheinungsbild Bootstrap Darkroom

In Galerien mit dem Erscheinungsbild Bootstrap Darkroom werden die veröffentlichten Kommentare rechts unter jedem Foto angezeigt.

![Espace commentaires BD.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-22f4823c.jpg)

Mit der Schaltfläche „Einen Kommentar hinterlassen“ öffnen Sie einen neuen Reiter zur Eingabe eines Kommentars.

![Ajouter commentaire BD.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-41ea19aa.jpg)

### Kommentarseite in Ihrer Galerie

In Ihrer Galerie sehen Sie alle Kommentare auf der Seite im Menü Erkunden > Kommentare.

Diese Seite zeigt alle in Ihrer Galerie veröffentlichten Kommentare mit dem zugehörigen Foto, dem Datum usw.

Sie können die Kommentare nach Foto oder nach Datum sortieren und sie mit der Suchfunktion filtern (nach Album, nach Autor, nach einem bestimmten Wort …).

![Voir commentaires.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-89e11245.jpg)

!!! note "Hinweis"
    Auf dieser Seite können Administratoren Kommentare freigeben, bearbeiten und löschen.

## Kommentare verwalten, bearbeiten und löschen

### Wartende Kommentare nach einer E-Mail freigeben

Wenn ein neuer Kommentar auf Freigabe wartet und die Administratoren benachrichtigt werden (siehe Kapitel „Optionen zur Kommentarverwaltung“), erhalten sie eine E-Mail wie unten gezeigt, mit dem Vermerk „Dieser Kommentar erfordert Überprüfung“.

![Validation commentaire.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-6c7cbb66.jpg)

Der Link „Diesen Kommentar bearbeiten“ führt Sie direkt zum Kommentar in der Galerie. Dort stehen Ihnen 3 Optionen zur Verfügung: Validieren, Löschen (entspricht dem Ablehnen des Kommentars) und Bearbeiten.

![Valider commentaire.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-e813e195.jpg)

### Wartende Kommentare im Administrationsbereich freigeben

Im Administrationsbereich von Piwigo verwalten Sie Kommentare über das Menü Werkzeuge > Kommentare.

Auf dieser Seite sehen Sie alle in Ihrer Galerie veröffentlichten Kommentare, wenn Sie auf „Alles“ klicken. Wenn Sie die Freigabe durch den Administrator aktiviert haben, erkennen Sie die wartenden Kommentare an der roten Markierung „Freizugebende Kommentare“.

![Liste commentaires.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-a609a283.jpg)

Um nur die wartenden Kommentare zu sehen, klicken Sie auf die Schaltfläche „Freizugebende Kommentare“.

Um einen Kommentar freizugeben oder abzuweisen, wählen Sie ihn einfach aus und klicken Sie auf „Freigeben“ oder „Abweisen“.

![Commentaire en attente.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-de9d13a7.jpg)

Ein abgewiesener Kommentar erscheint nicht mehr in der Liste.

Hinweis: Wartet ein Kommentar auf Freigabe, wird auf dem Dashboard der Administratoren ein Banner angezeigt. Über eine Schaltfläche gelangen sie direkt zur Verwaltungsseite der wartenden Kommentare.

![Attente validation.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-734bc3b2.jpg)

### Einen Kommentar bearbeiten oder löschen

Administratoren können die Kommentare der Benutzer in der Galerie löschen oder bearbeiten.

Wenn ein Administrator die Kommentare zu einem Foto in der Galerie ansieht, stehen ihm für jeden Kommentar zwei Aktionen zur Verfügung: „Bearbeiten“ und „Löschen“. Wartet der Kommentar auf Freigabe, ist zusätzlich die Aktion „Validieren“ verfügbar.

![Modifier ou supprimer.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-65f2ade6.jpg)

!!! info "Info:"
    Wenn Sie die Optionen gewählt haben, mit denen Benutzer ihre eigenen Kommentare entfernen / editieren dürfen, stehen ihnen diese Aktionen für ihre eigenen Kommentare ebenfalls zur Verfügung (ausser für anonyme, nicht angemeldete Benutzer).

Selbstverständlich sind diese Aktionen auch auf der Kommentarseite der Galerie verfügbar.

Werden Administratoren nach jedem neuen Kommentar per E-Mail benachrichtigt (ohne Freigabe), enthält die E-Mail einen Link, über den sie den Kommentar lesen und bei Bedarf bearbeiten oder löschen können.
