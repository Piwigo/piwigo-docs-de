---
title: Benutzer erstellen und verwalten - Piwigo-Dokumentation
description: Wie erstellen und bearbeiten Sie Benutzer in Piwigo? Welche Einstellungen und Optionen gibt es? In diesem Artikel erklären wir alles.
---

# Benutzer erstellen und verwalten

## Benutzer anzeigen und verwalten

Um Benutzer im Administrationsbereich von Piwigo zu erstellen, zu bearbeiten oder zu löschen, klicken Sie im linken Menü auf Benutzer > Verwaltung.

![users.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-b8726ada.png)

Der erste Tab listet die Benutzer Ihrer Piwigo-Galerie auf. Hier können Sie verschiedene Aktionen ausführen:

- Einen Benutzer erstellen
- Einen Benutzer suchen
- Einen Benutzer bearbeiten
- Mehrere Benutzer auf einmal bearbeiten
- Den Gastbenutzer (anonym) bearbeiten

!!! info "Seit Piwigo 15 können Sie die Benutzerliste nach Name oder Erstellungsdatum sortieren, indem Sie auf die Spaltenüberschrift klicken."

## Wie erstelle ich einen neuen Benutzer im Administrationsbereich?

Um im Administrationsbereich von Piwigo einen neuen Benutzer zu erstellen, klicken Sie in der Benutzerliste auf „Benutzer hinzufügen“: Es öffnet sich ein Pop-up-Fenster.

![image.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-84899d98.png)

In diesem Fenster legen Sie folgende Angaben für den Benutzer fest:

- Benutzername (für die Anmeldung bei Piwigo)
- E-Mail
- Status (mehr über [Benutzerstatus](benutzerstatus.md))
- Datenschutzstufe (mehr über [Datenschutzstufen](datenschutzstufen.md))
- Gruppe(n) (mehr über [Benutzergruppen](benutzergruppen.md))
- Berechtigung, Dateien in die Galerie hochzuladen

Neue Benutzer übernehmen standardmässig die Einstellungen des Benutzers „Gast“ (siehe [weiter unten auf dieser Seite](https://app.notion.com/p/Cr-er-et-g-rer-les-utilisateurs-3e044cd69819423e8160c30f1b1d03e2?pvs=21)).

Nachdem Sie einen neuen Benutzer erstellt haben, können Sie ihn bearbeiten, um sein Profil anzupassen.

Seit Piwigo 15 wird beim Erstellen eines neuen Benutzers im Administrationsbereich automatisch ein Link an seine E-Mail-Adresse gesendet, damit er ein Passwort wählen kann.

## Wie bearbeite ich einen Benutzer?

Um einen Benutzer zu bearbeiten, klicken Sie in der Benutzerliste einfach auf das Stift-Symbol links neben dem Namen. Der ausgewählte Benutzer wird orange hervorgehoben.

![Modifier utilisateur.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-8503e72b.jpg)

Daraufhin öffnet sich das Fenster zum Bearbeiten des Benutzers.

![image.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-47138217.png)

In diesem Fenster können Sie viele Einstellungen des Benutzers ändern und bestimmte Informationen einsehen.

Die Informationen sind in 3 Bereiche aufgeteilt:

- die wichtigsten Informationen links
- der Tab „Eigenschaften“ rechts
- der Tab „Einstellungen“ rechts

Manche Plugins fügen diesem Fenster weitere Tabs hinzu.

## Benutzername und Passwort ändern

Im linken Bereich des Fensters ändern Sie den Benutzernamen und das Passwort eines Benutzers.

**Benutzername**

Der Benutzername steht oben links im Fenster.

![image.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-dffce812.png)

Klicken Sie auf das Stift-Symbol, um ihn zu ändern. Der Benutzername lässt sich dann in einem Fenster bearbeiten.

![image.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-69830722.png)

!!! warning "Der Benutzername ist gleichzeitig die Kennung, mit der sich Benutzer bei Piwigo anmelden. Ändern Sie ihn nicht, ohne die Benutzer zu informieren."

**Passwort**

Klicken Sie auf „Passwort“, um das folgende Fenster zu öffnen.

![image.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-ac1b797f.png)

In diesem Fenster können Sie:

- den Link zum Zurücksetzen des Passworts kopieren, um ihn an einen Benutzer weiterzuleiten (falls der Versand per E-Mail nicht funktioniert)
- den Link zum Zurücksetzen des Passworts erneut per E-Mail senden
- das Passwort eines Benutzers ändern

### Zugriffsrechte eines Benutzers auf Alben bearbeiten

In Piwigo können Sie festlegen, ob ein Album privat oder öffentlich ist. Ein privates Album ist in der Galerie nur für berechtigte Benutzer sichtbar.

Mehr über die Zugriffsrechte auf Alben erfahren Sie [in diesem Artikel](../alben-organisieren/zugriffsrechte-und-sichtbarkeit-von-alben.md).

Klicken Sie im Fenster zum Bearbeiten eines Benutzers auf „Zugriffsrechte“, um die Alben anzuzeigen und zu bearbeiten, die der Benutzer sehen darf.

![permissions.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-05e4f72a.png)

Es öffnet sich ein Fenster mit einer Liste der privaten Alben:

- links die Alben, die der Benutzer sehen darf
- rechts die Alben, die er nicht sehen darf.

Um zu ändern, auf welche Alben der Benutzer Zugriff hat, verschieben Sie sie mit einem Klick auf die Pfeile einfach von einer Spalte in die andere.

![Gérer les permissions.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-c0ac9326.jpg)

!!! info "Wenn der Benutzer Mitglied einer Gruppe ist, haben die individuellen Zugriffsrechte Vorrang vor den Zugriffsrechten der Gruppe. [Mehr über Benutzergruppen](benutzergruppen.md)"

### Einen Benutzer löschen

Im Fenster zum Bearbeiten eines Benutzers können Sie den Benutzer mit einem Klick auf das Papierkorb-Symbol löschen.

![delete-user.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-1f997a1a.png)

In einem Zwischenschritt bestätigen Sie Ihre Wahl.

![image.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-bc6416fc.png)

### Den Hauptbenutzer Ihres Piwigo ändern

Der „Hauptbenutzer“ von Piwigo ist standardmässig der erste Benutzer:

- derjenige, der Piwigo installiert hat, wenn Sie Ihre Galerie selbst hosten;
- derjenige, der das Konto erstellt hat, wenn Sie ein Konto bei [Piwigo Cloud](https://de.piwigo.org/piwigo-bekommen) nutzen.

Dieser Benutzer hat den Status „Webmaster“.

In der Benutzerliste ist er mit einer Krone gekennzeichnet.

![main.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-bce6eb27.png)

Sobald ein Benutzer den Status „Webmaster“ hat, kann er als Hauptbenutzer festgelegt werden. Klicken Sie dazu im Fenster zum Bearbeiten des Benutzers auf das Kronen-Symbol. Wenn Sie bestätigen, ersetzt er den bisherigen Hauptbenutzer (in einem Piwigo-Konto kann es nur einen Hauptbenutzer geben).

![main2.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-035e918b.png)

### Eigenschaften eines Benutzers bearbeiten

Im Tab „Eigenschaften“ ändern Sie die Eigenschaften, die beim Erstellen des Benutzers festgelegt wurden.

![properties.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-c727020f.png)

**E-Mail-Adresse** 

In diesem Fenster können Sie die E-Mail-Adresse eines Benutzers ändern. Vergessen Sie nicht, auf „Aktualisieren“ zu klicken, um die Änderungen zu speichern.

**Status**

Sie können den Status eines Benutzers auch nach seiner Erstellung ändern, zum Beispiel in Administrator, Generisch, Webmaster…

Mehr über die Rollen und die Rechte der einzelnen Status erfahren Sie [in diesem Artikel](benutzerstatus.md).

Dabei gibt es einige Einschränkungen:

- Der angemeldete Administrator kann seinen eigenen Status nicht ändern
- Wenn Sie den Status des ersten Piwigo-Benutzers (Hauptbenutzer) ändern möchten, müssen Sie zuerst einen neuen Hauptbenutzer festlegen (siehe unten).

**Datenschutzstufe**

Standardmässig werden in Piwigo keine Datenschutzstufen verwendet. Sie können diese Einstellung also ignorieren, ausser Sie haben einen ganz besonderen Bedarf.

[Mehr über Datenschutzstufen](datenschutzstufen.md)

**Gruppe**

Im Fenster zum Bearbeiten eines Benutzers können Sie den Benutzer einer oder mehreren bestehenden Gruppen zuordnen.

[Mehr über Benutzergruppen](benutzergruppen.md)

**Download erlauben**

Aktivieren Sie dieses Kästchen, wenn ein Benutzer die Originalversion eines Fotos aus Ihrer Galerie herunterladen darf.

Wenn Sie diese Option deaktivieren, kann der Benutzer die Fotos in der Galerie ansehen, das Download-Symbol wird aber ausgeblendet.

### Einstellungen eines Benutzers bearbeiten

Die Einstellungen verändern das Aussehen der Piwigo-Galerie je nach Benutzer.

Im Administrationsbereich ändern Sie diese Einstellungen im Fenster zum Bearbeiten des Benutzers im Tab „Einstellungen“.

![preferences.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-af0c4e19.png)

Benutzer können sie auch selbst ändern, wenn sie in der Galerie angemeldet sind, indem sie auf das Menü „Anpassen“ klicken.

!!! info "Info:"
    Dass Benutzer ihre Einstellungen in der Galerie selbst bearbeiten, lässt sich in den Optionen von Piwigo abschalten (indem Sie die Option „Eigene Benutzer-Anpassungen erlauben“ deaktivieren). In diesem Fall dient das Menü „Anpassen“ nur noch dazu, die eigene E-Mail-Adresse und/oder das Passwort zu ändern.

Um die Standardeinstellungen für neue Benutzer zu ändern, bearbeiten Sie das Profil „Gast“ (siehe weiter unten).

Ausserdem können Sie die Einstellungen mehrerer Benutzer auf einmal im Auswahlmodus bearbeiten (siehe Kapitel [Mehrere Benutzer auf einmal bearbeiten](benutzer-erstellen-und-verwalten.md)).

Hier einige Details zu den Einstellungen.

**Fotos pro Seite**

Die Anzahl der Fotos, die auf einer Seite der Galerie angezeigt werden (zum Beispiel auf der Seite eines Albums). Standardmässig ist diese Zahl auf 15 eingestellt. Bei mehr als 15 Fotos werden also Links zu weiteren Seiten angezeigt. Sie können diese Zahl erhöhen oder verringern.

**Anzeigeschema**

In den meisten Fällen verwenden Piwigo-Galerien nur ein Erscheinungsbild. Diese Einstellung müssen Sie also nicht ändern. Sie ist nur nützlich, wenn Sie mehrere Erscheinungsbilder in Ihrer Galerie installiert haben und je nach Benutzer unterschiedliche Erscheinungsbilder anzeigen möchten.

[Mehr über Erscheinungsbilder](../erscheinungsbilder/index.md)

**Sprache**

Jede Galerie hat eine Standardsprache, Sie können aber mehrere Sprachen installieren.

Mit dieser Einstellung wählen Sie also, in welcher der in der Galerie aktivierten Sprachen die Oberfläche von Piwigo für einen bestimmten Benutzer angezeigt wird.

[Mehr über Sprachen](../ihre-galerie-anpassen/verfuegbare-sprachen-der-galerie-verwalten.md)

**Wie viele Tage sollen Bilder als neu markiert werden?**

Der Zeitraum, aus dem Fotos angezeigt werden, wenn der Benutzer in Ihrer Galerie auf das Menü „Neueste Fotos“ klickt. Dieser Zeitraum ist standardmässig auf 7 Tage eingestellt und kann geändert werden.

**Albenbaum komplett ausklappen**

Standardmässig ist diese Option deaktiviert. Das Menü „Alben“ in der Galerie listet dann nur die Hauptalben auf (keine Unteralben).

![Tous les albums.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-c79788c4.jpg)

Wenn Sie diese Option aktivieren, zeigt das Menü die gesamte Baumstruktur.

![Albums étendus.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-70e5457c.jpg)

**Anzahl der Kommentare anzeigen**

Mit dieser Option wird auf den Übersichtsseiten der Galerie unter dem Vorschaubild die Anzahl der Kommentare jedes Fotos angezeigt.

!!! info "Diese Option funktioniert mit einigen Erscheinungsbildern (Elegant, Bootstrap Darkroom), aber nicht mit dem Erscheinungsbild Modus."

![Nombre de commentaires.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-4d3944cc.jpg)

**Anzahl der Bildaufrufe anzeigen**

Mit dieser Option wird auf den Übersichtsseiten der Galerie unter dem Vorschaubild die Anzahl der Aufrufe jedes Fotos angezeigt.

!!! info "Diese Option funktioniert mit einigen Erscheinungsbildern (Elegant, Bootstrap Darkroom), aber nicht mit dem Erscheinungsbild Modus."

![Nombre de visites.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-2d39be8e.jpg)

## Wie sehe ich den Verlauf eines Benutzers?

Das Fenster zum Bearbeiten eines Benutzers zeigt das Erstellungsdatum und das Datum der letzten Anmeldung. Über die Schaltfläche „Geschichte besuchen“ gelangen Sie ausserdem zum Besuchsverlauf des Benutzers.

![history.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-02660928.png)

### Besuchsverlauf

Die Schaltfläche „Geschichte besuchen“ öffnet den Besuchsverlauf dieses Benutzers. Dort sehen Sie, welche Alben er aufgerufen hat und welche Fotos er angesehen und heruntergeladen hat.

[Mehr über den Besuchsverlauf](../piwigo-administrieren/statistiken-der-galerie-ansehen.md)

![Untitled](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-94c3e836.png)

### Aktivität der Administratoren

Um den detaillierten Verlauf aller Aktionen eines Benutzers im Administrationsbereich anzuzeigen, öffnen Sie auf der Seite „Benutzer“ den Tab „Tätigkeit“.

[Mehr über den Aktivitätsverlauf](../piwigo-administrieren/statistiken-der-galerie-ansehen.md)

!!! info "Wenn Sie Kunde von Piwigo Cloud sind, ist dieses Plugin erst ab dem Enterprise-Tarif verfügbar."

![Liste activité.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-49d3aeab.jpg)

## Einen Benutzer suchen

In der Benutzerliste können Sie eine Suche durchführen, um einen Benutzer auch bei vielen Benutzern schnell zu finden.

Mit dem Suchfeld finden Sie einen Benutzer über seinen Benutzernamen. Geben Sie ein paar Buchstaben ein: Die Liste wird automatisch aktualisiert.

![Recherche utilisateur.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-e43e94df.jpg)

Sie können auch auf die Schaltfläche „Filter“ klicken, um Suchkriterien anzuzeigen.

![image.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-7d4e82c2.png)

Sie können die Benutzerliste filtern nach:

- Status (Webmaster, Administrator, Besucher…)
- Datenschutzstufe
- Gruppe
- Registrierungsdatum (Erstellung des Benutzers)

## Mehrere Benutzer auf einmal bearbeiten

Möchten Sie Änderungen auf eine Auswahl von Benutzern anwenden?

Klicken Sie dazu in der Benutzerliste rechts auf die Schaltfläche „Auswahlmodus“.

![Mode sélection utilisateurs.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-e6522118.jpg)

Sobald der Auswahlmodus aktiv ist, können Sie die Benutzer auswählen, die Sie bearbeiten möchten: Sie erscheinen nacheinander in einer Liste rechts auf dem Bildschirm. Falls Sie sich vertan haben, können Sie einen Benutzer mit einem Klick auf das Kreuz neben seinem Namen wieder aus der Auswahl entfernen.

Oben auf dem Bildschirm helfen Ihnen die Schaltflächen Die ganze Seite / Das ganze Set / Nichts / Invertieren, schneller auszuwählen, wenn Sie viele Benutzer verwalten.

- Ein Klick auf „Die ganze Seite“ fügt alle auf dem Bildschirm sichtbaren Benutzer zu Ihrer Auswahl hinzu
- Ein Klick auf „Das ganze Set“ fügt alle Benutzer Ihrer Piwigo-Galerie zu Ihrer Auswahl hinzu
- Ein Klick auf „Nichts“ leert Ihre Auswahl
- Ein Klick auf „Invertieren“ wählt alle Benutzer aus, ausser den aktuell ausgewählten.

![Choisir action utilisateurs.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-27a15512.jpg)

Wenn Ihre Auswahl fertig ist, klicken Sie auf die gewünschte Aktion:

- Markierte Benutzer löschen
- Gruppenzuordnung / Gruppenzuordnung aufheben
- Download erlauben
- Datenschutzstufe
- Einstellungen bearbeiten (Anzahl der Fotos pro Seite, Anzeigeschema, Sprache, Zeitraum für neue Fotos, Albenbaum komplett ausklappen, Anzahl der Bildaufrufe anzeigen)

## Einstellungen für „Gast“ bearbeiten

Auf der Seite zur Benutzerverwaltung können Sie den Gastbenutzer bearbeiten.

Der Benutzer „Gast“ entspricht dem Profil anonymer Besucher, die die Galerie ansehen, ohne bei Piwigo angemeldet zu sein. Aber das ist nicht alles: Die Einstellungen dieses Benutzers sind auch die Standardeinstellungen für alle neuen Benutzer.

Um das Gastprofil zu ändern, klicken Sie auf „Gastbenutzer bearbeiten“.

![Modifier utilisateur invité.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-867edb0e.jpg)

Es öffnet sich ein Fenster, das dem Fenster zum Bearbeiten eines Benutzers ähnelt.

![image.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-abd5d211.png)

## Besuchern der Galerie die Kontoerstellung erlauben oder verbieten

Je nachdem, wie Sie Ihre Piwigo-Galerie nutzen, können Sie zulassen oder ablehnen, dass Benutzer selbst ein Konto erstellen.

Zum Beispiel:

- Unternehmen und Organisationen, die mit Piwigo eine private Fotothek verwalten, möchten nicht, dass Personen von ausserhalb ein Konto erstellen können: Benutzer werden immer von einem Administrator angelegt.
- Manche Organisationen (zum Beispiel Tourismusbüros) erlauben berechtigten Personen (Journalisten, Partnern, Schulen…), ein Konto in ihrer Fotothek zu erstellen, um auf lizenzfreie Bilder zuzugreifen. Die Kontoerstellung soll aber von einem Administrator freigegeben werden.
- Andere Betreiber von Fotoarchiven stellen einen Teil ihrer Inhalte öffentlich zur Verfügung, möchten aber, dass Benutzer vor dem Zugriff auf die Galerie ein Konto erstellen. So verstehen sie besser, wie ihre Inhalte genutzt werden, und erhalten Daten über die interessierten Personen.

Piwigo lässt Sie also selbst festlegen, welche Regeln in Ihrer Fotothek für die Kontoerstellung durch Besucher gelten.

Öffnen Sie dazu im Administrationsbereich das Menü Konfiguration > Optionen, Abschnitt „Zugriffsrechte“.

![Permissions tous admins.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-837c1808.jpg)

Dort gibt es die Option **Neuregistrierung von Benutzern erlauben**.

Wenn Sie diese Option aktivieren, erscheint in Ihrer Galerie ein Link „Registrieren“. Darüber kann ein Benutzer ein Formular ausfüllen, um ein Konto in Ihrer Galerie zu erstellen.

Mit der zugehörigen Option „Eine E-Mail an die Administratoren senden, wenn sich ein neuer Benutzer registriert hat“ erhalten die Administratoren jedes Mal eine E-Mail, wenn jemand ein Konto in Ihrer Galerie erstellt. So können sie prüfen, ob die Person sich registrieren darf, und ihr die gewünschten Zugriffsrechte geben, sie einer Gruppe hinzufügen usw.

Sie können wählen, ob bei einem neuen Konto alle Administratoren benachrichtigt werden oder nur die Mitglieder einer Gruppe.

## User Mass Register: Mehrere Benutzer auf einmal erstellen

Wenn Sie mehrere Benutzer auf einmal erstellen möchten, aktivieren Sie das Plugin **User Mass Register**.

Mit diesem Plugin erstellen Sie Benutzer gesammelt aus einer Liste von E-Mail-Adressen. Die Benutzer erhalten standardmässig den Status „Benutzer“.

Anschliessend können Sie diese Benutzer im Auswahlmodus gemeinsam bearbeiten (siehe Kapitel [Mehrere Benutzer auf einmal bearbeiten](benutzer-erstellen-und-verwalten.md)).

!!! info "Wenn Sie Kunde von Piwigo Cloud sind, ist dieses Plugin erst ab dem Enterprise-Tarif verfügbar."

## Add User Note: Einem Benutzer eine Notiz hinzufügen

Um einem Benutzer eine Notiz oder einen Kommentar hinzuzufügen, können Sie das Plugin **Add User Note** aktivieren.

!!! info "Wenn Sie Kunde von Piwigo Cloud sind, ist dieses Plugin erst ab dem Team-Tarif verfügbar."

Dieses Plugin fügt dem Fenster zum Bearbeiten eines Benutzers einen Tab „Notizen“ hinzu.

![image.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-6a142b84.png)

Wenn für einen Benutzer eine Notiz eingegeben wurde, erscheint in der Liste ein Symbol neben seinem Namen. Wenn Sie mit der Maus über dieses Symbol fahren, können Sie die Notiz lesen.

![image.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-e1ff79d6.png)

## User Custom Fields: Benutzern eigene Felder hinzufügen

Sie können eigene Felder für Benutzer anlegen.

!!! info "Wenn Sie Kunde von Piwigo Cloud sind, ist dieses Plugin erst ab dem Team-Tarif verfügbar."

Aktivieren Sie dazu das Plugin User Custom Fields.

Der Vorteil dieses Plugins: Sie können von Personen, die sich in Ihrer Galerie registrieren, zusätzliche Informationen abfragen (sofern Sie die Registrierung aktiviert haben). Die zusätzlichen Felder können Pflichtfelder sein oder nicht.

Im folgenden Beispiel haben wir dem Registrierungsformular der Galerie das Feld „Stadt“ hinzugefügt.

![User Custom Fields.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-cc40ba03.jpg)

Wenn dieses Plugin aktiviert ist, erscheint im Fenster zum Bearbeiten eines Benutzers ein Tab „Eigene Felder“.

Mit einem Klick darauf können Sie den Inhalt der eigenen Felder ansehen und bearbeiten.

## Crypto Captcha: Das Erstellen gefälschter Benutzer verhindern

Um zu verhindern, dass Bots gefälschte Benutzer in Ihrer Galerie anlegen, können Sie das Plugin **Crypto Captcha** installieren.

Mit diesem Plugin müssen Benutzer vor dem Erstellen eines Kontos ein Captcha ausfüllen. Dieses Captcha lässt sich auch dem Formular zum Verfassen von Kommentaren hinzufügen.

Für die Einrichtung Ihres Captchas stehen mehrere Optionen zur Verfügung.

![Test Captcha.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-ac638942.jpg)
