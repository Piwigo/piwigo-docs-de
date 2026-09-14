---
title: "Zwei-Faktor-Authentifizierung: 2FA in Piwigo aktivieren"
description: "Wie melden Sie sich bei Ihrem Piwigo-Konto an? Welche Möglichkeiten gibt es, ein Konto zu erstellen und sich anzumelden? In diesem Artikel erklären wir alles."
---

# Zwei-Faktor-Authentifizierung: 2FA in Piwigo aktivieren

Inhaltsverzeichnis:

Seit Piwigo-Version 16 können Benutzer die Zwei-Faktor-Authentifizierung (*2FA*) aktivieren. Das ist eine starke Authentifizierungsmethode, die heute immer häufiger eingesetzt wird. Wenn 2FA aktiviert ist, müssen Benutzer zwei Schritte durchlaufen, um auf Piwigo zuzugreifen:

- Schritt 1: normale Anmeldung (Benutzername + Passwort)
- Schritt 2: Bestätigung der Identität, entweder mit einem Code per E-Mail oder mit einer Authentifizierungs-App, die einen Einmalcode (TOTP) erzeugt

Um die Zwei-Faktor-Authentifizierung zu nutzen, müssen Sie das Plugin **Two Factor Authentication** installieren und aktivieren.

## Das Plugin **Two Factor Authentication** konfigurieren

Öffnen Sie die Einstellungen des Plugins, um die Zwei-Faktor-Authentifizierung zu konfigurieren.

![image.png](https://ressources.piwigo.com/i?/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-29507eb1-sm.png)

Es stehen mehrere Optionen zur Verfügung:

- **Maximale Anzahl fehlgeschlagener Versuche vor der Sperrung:** Wenn ein Benutzer mehrmals erfolglos versucht, sich anzumelden, wird sein Konto gesperrt. Legen Sie hier die maximale Anzahl der Versuche fest.
- **Dauer der Sperrung (in Sekunden):** der Zeitraum, in dem das Konto gesperrt bleibt, sobald die Grenze der fehlgeschlagenen Versuche erreicht ist.

Für die Zwei-Faktor-Authentifizierung gibt es zwei Methoden:

- **2FA per App:** Benutzer verwenden eine Authentifizierungs-App, die einen Einmalcode (TOTP) erzeugt
- **2FA per E-Mail:** Benutzer erhalten einen Einmalcode per E-Mail

Sie können auch beide Methoden aktivieren: Die Benutzer wählen dann die Methode, die ihnen lieber ist.

## Zwei-Faktor-Authentifizierung durch die Benutzer aktivieren

Auch wenn 2FA über das Plugin aktiviert ist, ist sie für die Piwigo-Benutzer standardmässig **nicht** eingeschaltet.

Jeder Benutzer muss 2FA in seinem eigenen Profil aktivieren.

Dazu öffnen die Benutzer ihre Piwigo-Galerie und rufen dann die Seite „Profil“ auf.

![image.png](https://ressources.piwigo.com/i?/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-9310ab1e-la.png)

Klicken Sie auf den Pfeil neben „Zwei-Faktor-Authentifizierung“, um die verfügbaren Optionen anzuzeigen. Anschliessend können Sie die gewünschte Authentifizierungsmethode wählen.

Hinweis: Wenn in den Einstellungen des Plugins nur eine Methode aktiviert wurde, wird hier auch nur diese angezeigt.

![image.png](https://ressources.piwigo.com/i?/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-f5e7bfae-me.png)

## Zwei-Faktor-Authentifizierung mit einer Authentifizierungs-App nutzen

Wenn Sie diese Methode wählen, benötigen Sie eine Authentifizierungs-App wie 1Password, Authy, Microsoft Authenticator, TOTP oder eine andere App, die Einmalcodes für die Anmeldung erzeugen kann.

Installieren Sie zuerst die App Ihrer Wahl auf Ihrem Telefon, falls Sie das noch nicht getan haben. Diese Dokumentation zeigt den Ablauf am Beispiel der kostenlosen App TOTP (für iOS und Android erhältlich).

Öffnen Sie Ihr Profil und wählen Sie „Mit einer Authentifizierungs-App einrichten“. Es erscheint eine Anleitung.

![Capture d’écran 2025-11-17 à 17.18.35.png](https://ressources.piwigo.com/i?/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-5eb07cca-me.png)

Öffnen Sie die Authentifizierungs-App auf Ihrem Telefon und fügen Sie Ihr Piwigo-Konto hinzu, indem Sie den QR-Code auf Ihrem Bildschirm scannen.

![IMG_4248.jpg](https://ressources.piwigo.com/i?/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-241841b6-la.jpg)

Sobald das Konto hinzugefügt ist, erzeugt die App einen Einmalcode.

![IMG_4249.jpg](https://ressources.piwigo.com/picture?/1863/category/172-two_factor_authentication_enable_2fa_on_piwigo)

Geben Sie diesen Code in das dafür vorgesehene Feld in Ihrem Piwigo-Profil ein.

Danach erscheint eine Bestätigungsmeldung.

![Capture d’écran 2025-11-17 à 17.28.03.png](https://ressources.piwigo.com/_datas/c/v/7/cv7jpz6hf8/i/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-1c48becb-sm.png)

Kopieren Sie Ihre Wiederherstellungscodes und bewahren Sie sie an einem sicheren Ort auf, den Sie sich merken können (eine Notiz, ein Dokument, eine E-Mail usw.).


!!! warning "**Achtung**"

    Sobald die Zwei-Faktor-Authentifizierung aktiviert ist, können sich Drittanbieter-Anwendungen, die auf Ihr Piwigo-Konto zugreifen (Piwigo-Mobile-Apps, Lightroom-Plugin, Piwigo Remote Sync), nicht mehr mit Ihrem üblichen Benutzernamen und Passwort anmelden. [Lesen Sie das letzte Kapitel dieser Seite, um das zu beheben.](#drittanbieter-anwendungen-verbinden-wenn-2fa-aktiviert-ist)

## Zwei-Faktor-Authentifizierung per E-Mail nutzen

!!! warning "**Achtung**"

    Diese Methode ist weniger sicher. E-Mails können im Spam landen oder gar nicht erst verschickt werden, wenn Ihr Server nicht richtig konfiguriert ist. Wenn Sie diese Methode aktivieren, stellen Sie sicher, dass die E-Mails Ihrer Piwigo-Installation ihr Ziel erreichen.

Sobald 2FA per E-Mail in den Einstellungen des Plugins aktiviert ist, öffnen Sie Ihr Profil und wählen „Per E-Mail einrichten“. Prüfen Sie, ob die mit Ihrem Konto verknüpfte E-Mail-Adresse stimmt, geben Sie sie im Feld „E-Mail-Adresse bestätigen“ erneut ein und klicken Sie auf **„E-Mail senden“**.

![Capture d’écran 2025-11-17 à 17.49.36.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-f744751a.png)

Sehen Sie in Ihrem Posteingang nach und geben Sie den Code, sobald Sie ihn erhalten haben, in das entsprechende Feld ein.

![Capture d’écran 2025-11-17 à 17.51.08.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/05/25/20260525140116-9e94e80d.png)


!!! warning "**Achtung**"

    Sobald die Zwei-Faktor-Authentifizierung aktiviert ist, können sich Drittanbieter-Anwendungen, die auf Ihr Piwigo-Konto zugreifen (Piwigo-Mobile-Apps, Lightroom-Plugin, Piwigo Remote Sync), nicht mehr mit Ihrem üblichen Benutzernamen und Passwort anmelden. [Lesen Sie das letzte Kapitel dieser Seite, um das zu beheben.](#eine-drittanbieter-anwendung-mit-ihrem-api-schlussel-verbinden)

## Drittanbieter-Anwendungen verbinden, wenn 2FA aktiviert ist

Wenn 2FA aktiv ist, können sich Drittanbieter-Anwendungen nicht mehr nur mit Ihrem Benutzernamen und Passwort anmelden.

Bis diese Anwendungen eine Anmeldung per API-Schlüssel oder eine eigene 2FA-Unterstützung anbieten, stellt Piwigo eine Übergangslösung bereit. Damit funktionieren die Apps ohne Update weiter.

**Wenn ein Benutzer 2FA aktiviert und weiterhin die Piwigo-Mobile-App, Piwigo Remote Sync oder das Lightroom-Export-Plugin nutzen möchte, muss er die folgende Anleitung befolgen.**

### Einen API-Schlüssel in Ihrem Profil erstellen

Öffnen Sie Ihre Piwigo-Galerie und rufen Sie die Seite „Profil“ auf.

![image.png](https://ressources.piwigo.com/i?/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-9310ab1e-la.png)

Klicken Sie auf den Pfeil, um den Bereich „API-Schlüssel“ aufzuklappen.

Erstellen Sie einen neuen API-Schlüssel und benennen Sie ihn nach der Anwendung, die Sie verbinden möchten, zum Beispiel *„Piwigo mobile iOS“*.

Wählen Sie, wie lange dieser Schlüssel gültig sein soll. Nach Ablauf müssen Sie einen neuen Schlüssel erzeugen und den Vorgang wiederholen.

![Capture d’écran 2025-11-17 à 17.54.07.png](https://ressources.piwigo.com/i?/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-4c54c8e2-sm.png)

Klicken Sie auf **„Schlüssel generieren“**. Piwigo zeigt eine **ID** und ein **Geheimnis** (Secret) an, die Sie **unbedingt kopieren und sicher aufbewahren müssen** (eine Notiz, ein Dokument, eine E-Mail usw.).

![Capture d’écran 2025-11-17 à 17.55.23.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-fb3ad674.png)

### Eine Drittanbieter-Anwendung mit Ihrem API-Schlüssel verbinden

Öffnen Sie die Drittanbieter-Anwendung, die Sie nutzen möchten (zum Beispiel die Piwigo-Mobile-App).

Geben Sie statt Ihres Benutzernamens die **ID** des API-Schlüssels ein (sie beginnt mit „pkid-…“) und statt Ihres Passworts das **Geheimnis** des API-Schlüssels.

Sie sind dann angemeldet und werden als der Benutzer erkannt, zu dem dieser Schlüssel gehört.

!!! note "**Hinweis**"
    API-Schlüssel haben ein Ablaufdatum. Erneuern Sie sie regelmässig. Piwigo benachrichtigt Sie per E-Mail, wenn einer Ihrer Schlüssel bald abläuft.
