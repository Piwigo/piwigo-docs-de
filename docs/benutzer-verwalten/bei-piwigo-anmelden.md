---
title: "Bei Piwigo anmelden - Piwigo-Dokumentation"
description: "Wie melden Sie sich bei Ihrem Piwigo-Konto an? Welche Möglichkeiten gibt es, ein Konto zu erstellen und sich anzumelden? In diesem Artikel wird alles erklärt."
---

# Bei Piwigo anmelden

## Wie melde ich mich bei Piwigo an?

Um sich bei Ihrem Piwigo-Konto anzumelden, rufen Sie die URL (Webadresse) Ihrer Galerie auf. 

Wenn Sie Modus verwenden, das Standard-Erscheinungsbild von Piwigo, finden Sie oben rechts auf dem Bildschirm den Link „Anmeldung“. Dieser Link öffnet das Fenster, in dem Sie sich bei Piwigo anmelden können.

![Anmeldebildschirm](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-546099ea.jpg)

Wenn Sie das Erscheinungsbild Bootstrap Darkroom verwenden, öffnet die Anmeldeschaltfläche keine neue Seite, sondern ein modales Fenster.

![Anmeldung Bootstrap Darkroom](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-263eca8d.jpg)

!!! tip "Je nach Erscheinungsbild und Anpassung Ihrer Galerie kann der Anmeldebildschirm anders aussehen als auf den Bildern oben."

Die URL Ihrer Piwigo-Anmeldeseite lautet [`mygallery.com`](http://mygallery.com)/identification.php, wobei `mygallery.com` für die Stamm-URL Ihrer Galerie steht. 

Wenn Ihre Galerie bei Piwigo Cloud gehostet wird und Sie den Domainnamen Ihrer Galerie nicht angepasst haben, sieht Ihre Anmelde-URL so aus: `mygallery`.piwigo.com/identification.php. Dabei steht `mygallery` für den Benutzernamen, den Sie beim Erstellen Ihres Kontos gewählt haben.

Um sich bei Piwigo anzumelden, können Sie im Feld „Benutzername“ Ihren Benutzernamen ODER Ihre E-Mail-Adresse eingeben.

Ausserdem müssen Sie Ihr Passwort eingeben.

Nach der Anmeldung werden Sie zu Ihrer Galerie weitergeleitet.

## Wie zeige ich ein Anmeldeformular auf der Startseite an?

Wenn die Startseite direkt ein Anmeldeformular anzeigen soll, ist das mit dem Plugin **PWG Stuffs** möglich.

[Mehr erfahren](../ihre-galerie-anpassen/plugins-zur-galerie-anpassung/pwg-stuffs-bloecke-in-ihrer-galerie-hinzufuegen.md)

## Wie gelange ich in den Administrationsbereich von Piwigo?

Wenn Sie in Ihrer Piwigo-Galerie als Administrator angemeldet sind, klicken Sie in Ihrer Galerie einfach auf das Menü „Administration“, um in den Administrationsbereich zu wechseln.

Im Erscheinungsbild Modus befindet sich das Menü „Administration“ standardmässig oben rechts auf dem Bildschirm.

![Administration Modus](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-5b6e4744.jpg)

Im Erscheinungsbild Bootstrap Darkroom erreichen Sie das Menü für den Zugang zum Administrationsbereich, indem Sie oben rechts auf Ihren Benutzernamen klicken.

![Administration Bootstrap Darkroom](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-f4e53a6c.jpg)

## Wie stelle ich mein Piwigo-Passwort wieder her?

Ein verlorenes Passwort lässt sich nicht wiederherstellen, egal ob Sie Kunde von Piwigo Cloud sind oder eine selbst gehostete Piwigo-Galerie verwenden. Deshalb müssen Sie Ihr Passwort zurücksetzen.

Um Ihr Passwort zurückzusetzen, öffnen Sie das Anmeldefenster von Piwigo und klicken Sie auf „Passwort vergessen?“.

Nachdem Sie Ihren Benutzernamen oder Ihre E-Mail-Adresse eingegeben haben, erhalten Sie per E-Mail einen Link, mit dem Sie Ihr Passwort zurücksetzen können.

Sie können auch einen Administrator bitten, Ihnen eine E-Mail mit einem Link zum Zurücksetzen des Passworts zu senden oder ein neues Passwort für Sie festzulegen und es Ihnen zu schicken.

## Wie finde ich meinen Piwigo-Benutzernamen oder meine Anmelde-E-Mail-Adresse wieder?

Sie haben Ihren Benutzernamen und/oder die E-Mail-Adresse vergessen, mit der Sie sich bei Piwigo anmelden?

Kein Grund zur Panik: Es gibt mehrere Möglichkeiten, Ihr Konto wiederzufinden.

### Einen Administrator fragen

Wenn Sie in einem Team arbeiten, wenden Sie sich an den Hauptadministrator Ihrer Piwigo-Galerie: Er kann Ihr Konto wiederfinden.

Sie können auch in Ihrem Posteingang nach der E-Mail suchen, die beim Erstellen Ihres Kontos verschickt wurde.

### Die Zugangsdaten aus der E-Mail bei der Kontoerstellung wiederfinden

Wenn Sie der einzige Benutzer Ihrer Piwigo-Galerie oder der Hauptadministrator (der Webmaster) sind, sollten Sie Ihre Zugangsdaten per E-Mail erhalten haben.

- Wenn Ihre Piwigo-Galerie bei [Piwigo Cloud](https://de.piwigo.org/piwigo-bekommen) gehostet wird: Sie haben beim Erstellen Ihres Piwigo-Kontos eine E-Mail erhalten.
- Wenn Sie eine selbst gehostete Piwigo-Galerie verwenden: Falls Sie bei der ersten Installation von Piwigo das Installationsformular ausgefüllt haben, haben Sie möglicherweise die Option „Verbindungseinstellungen per E-Mail senden“ gewählt.

### Sie können sich wirklich nicht bei Piwigo anmelden?

Wenn Sie ein Konto bei Piwigo Cloud haben, wenden Sie sich an den Support: Wir finden einen Weg, es wiederherzustellen.

Wenn Sie eine selbst gehostete Piwigo-Galerie verwenden, können wir Ihnen leider nicht helfen. Wenn Sie jedoch Zugriff auf die Datenbank von Piwigo haben, finden Sie Ihren Benutzernamen in der Tabelle der Benutzer.

## Wie erstelle ich ein neues Konto in einer Piwigo-Galerie?

Es gibt zwei Möglichkeiten, einen neuen Benutzer in Piwigo anzulegen.

### Fall 1: Ein Administrator erstellt die Benutzerkonten

In manchen Fällen ist die Option „Neuregistrierung von Benutzern erlauben“ deaktiviert (diese Option finden Sie im Menü „Konfiguration > Optionen“, Reiter „Allgemein“, Abschnitt „Zugriffsrechte“).

In diesem Fall können Besucher der Galerie kein eigenes Konto erstellen: Nur ein Administrator kann neue Benutzer anlegen. 

Wie Sie im Administrationsbereich einen Benutzer erstellen, erfahren Sie [in diesem Artikel](benutzer-erstellen-und-verwalten.md).

### Fall 2: Die Besucher der Galerie können ein eigenes Konto erstellen

Wenn die Option „Neuregistrierung von Benutzern erlauben“ aktiviert ist, kann jeder Besucher der Galerie ein eigenes Konto erstellen.

!!! info "Mehr darüber, wie Sie die Kontoerstellung für Besucher der Galerie erlauben oder verbieten, erfahren Sie [in diesem Artikel](benutzer-erstellen-und-verwalten.md)."


Um ein neues Konto in einer Piwigo-Galerie zu erstellen, klicken Sie auf „Anmeldung“.

Über die Schaltfläche „Registrieren“ können Sie ein neues Konto erstellen.

Für ein neues Konto geben Sie einen Benutzernamen, eine E-Mail-Adresse und ein Passwort an.

!!! info "Wenn Sie dem Formular zur Kontoerstellung eigene Felder hinzufügen möchten, aktivieren Sie das Plugin User Custom Fields. [Mehr erfahren](benutzer-erstellen-und-verwalten.md)"


!!! info "Um zu verhindern, dass Roboter gefälschte Benutzerkonten anlegen, können Sie die Kontoerstellung mit einem Captcha-Feld absichern. Aktivieren Sie dazu das Plugin **Crypto Captcha**. [Mehr erfahren](benutzer-erstellen-und-verwalten.md)"


Benutzerkonten, die Benutzer selbst in der Galerie erstellen, sind keine Administratoren, sondern einfache Benutzer. Mehr über den Benutzerstatus erfahren Sie [in diesem Artikel](benutzerstatus.md).

## Wie aktiviere ich die Zwei-Faktor-Authentifizierung (2FA) in Piwigo?

Seit Version 16 von Piwigo können Sie die Zwei-Faktor-Authentifizierung (2FA) für Benutzer aktivieren. Diese starke Authentifizierungsmethode wird heute immer häufiger eingesetzt. Wenn die Zwei-Faktor-Authentifizierung aktiviert ist, müssen Benutzer zwei Schritte durchlaufen, um auf Piwigo zuzugreifen:

- Schritt 1: normale Anmeldung (Benutzername + Passwort)
- Schritt 2: Bestätigung ihrer Identität, entweder per E-Mail oder mit einer App, die einen Einmalcode (TOTP) erzeugt

Um die Zwei-Faktor-Authentifizierung einzurichten, installieren und aktivieren Sie das Plugin **Two Factor Authentication**.

Die Dokumentation zu diesem Plugin finden Sie hier:

[Zwei-Faktor-Authentifizierung: 2FA in Piwigo aktivieren](bei-piwigo-anmelden/zwei-faktor-authentifizierung-in-piwigo-aktivieren.md)

## Wie aktiviere ich Single Sign-On (SSO) in Piwigo?

Wenn Sie in einer Organisation arbeiten, verwenden Sie vielleicht bereits ein System zur Verwaltung von Benutzern und Passwörtern. Deshalb möchten Sie, dass sich Benutzer automatisch bei Piwigo anmelden können.

Dafür gibt es zwei Möglichkeiten: das Plugin **LDAP Login** und das Plugin **Microsoft 365 Connect**.

### LDAP Login: ein LDAP-Verzeichnis verwenden

Mit diesem Plugin können Sie Piwigo mit einem LDAP-Verzeichnis verbinden.

!!! info "Wenn Sie Kunde von Piwigo Cloud sind, ist dieses Plugin erst ab dem VIP-Tarif verfügbar."

### Microsoft 365 Connect: Piwigo mit einem Azure Active Directory verbinden

Mit diesem Plugin können Sie Piwigo mit einem Azure Active Directory verbinden.

!!! info "Wenn Sie Kunde von Piwigo Cloud sind, ist dieses Plugin erst ab dem VIP-Tarif verfügbar."

So können sich Benutzer mit ihrem Microsoft-365-Konto bei Piwigo anmelden.

- Die E-Mail-Adresse des Piwigo-Benutzers muss mit der E-Mail-Adresse des Microsoft-365-Kontos übereinstimmen.
- Zuerst müssen Sie Ihre Piwigo-App im Azure-Portal registrieren (die Anleitung finden Sie auf der Konfigurationsseite des Plugins).

## Password Policy: Sicherheitsregeln für Passwörter festlegen

Mit dem Plugin **Password Policy** können Sie Sicherheitsregeln für Passwörter festlegen: Stärkebewertung, Regeln zur Erneuerung, Umgang mit fehlgeschlagenen Anmeldeversuchen…

!!! info "Wenn Sie Kunde von Piwigo Cloud sind, ist dieses Plugin erst ab dem VIP-Tarif verfügbar."

Nachdem Sie das Plugin Password Policy in Ihrer Piwigo-Galerie aktiviert haben, öffnen Sie seine Konfiguration.

Im Reiter **Konfiguration** des Plugins legen Sie die Sicherheitsregeln fest.

![Password Policy](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-69207d70.jpg)

Auf dieser Seite können Sie:

- die verstärkte Passwortsicherheit aktivieren
- die Mindestpunktzahl festlegen, die ein Passwort erreichen muss, um akzeptiert zu werden

Eine Punktzahl unter 100 gilt als schwach. Eine Punktzahl zwischen 100 und 500 ist durchschnittlich. Eine Punktzahl über 500 ist ausgezeichnet. Die Punktzahl hängt von verschiedenen Kriterien ab (Länge, Art der verwendeten Zeichen).

- ein Passwort testen und seine Punktzahl anzeigen
    
!!! info "Zum Beispiel erhält das Passwort `piwigo12` eine schwache Punktzahl (48), das Passwort `Xhj89^h5M%` dagegen eine durchschnittliche Punktzahl (286)."
    
- festlegen, ob die Regel zur verstärkten Passwortsicherheit auch für Administratoren gilt
- die Regel zur Passworterneuerung aktivieren (in diesem Fall kann der Administrator Benutzer zwingen, ihr Passwort zu erneuern)
- den Umgang mit fehlgeschlagenen Anmeldeversuchen aktivieren: Nach einer einstellbaren Anzahl von Versuchen wird der Zugang zur Galerie gesperrt. Die angezeigte Meldung lässt sich anpassen.
    
    ![Informationsmeldung](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-25072184.jpg)
    

Im Reiter „Verwaltung“ können Sie Anfragen zur Passworterneuerung bearbeiten und gesperrte Konten entsperren.

![Benutzerverwaltung Password Policy](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-c5454ae0.jpg)
