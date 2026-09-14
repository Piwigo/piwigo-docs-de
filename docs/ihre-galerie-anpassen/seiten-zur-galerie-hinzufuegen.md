---
title: Seiten zu Ihrer Galerie hinzufügen - Piwigo-Dokumentation
description: Möchten Sie Ihrer Piwigo-Galerie eigene Seiten hinzufügen? Mit ein paar Plugins ist das möglich.
---

# Seiten zu Ihrer Galerie hinzufügen

Möchten Sie Ihrer Piwigo-Galerie eigene Seiten hinzufügen? Mit ein paar Plugins ist das möglich.

## Additional Pages: HTML-Seiten hinzufügen

Mit dem Plugin Additional Pages können Sie Ihrer Galerie neue Seiten hinzufügen und sie über das [Navigationsmenü](menue-und-navigationsleiste-anpassen.md) zugänglich machen.

Sobald dieses Plugin aktiviert ist, öffnen Sie seine Konfigurationsseite.

### Eine neue Seite hinzufügen

Im ersten Tab können Sie Ihrer Galerie eine neue Seite hinzufügen.

Sie können mit einer leeren Seite beginnen oder eine der Seitenvorlagen laden, die mit dem Plugin mitgeliefert werden.

Sie können die Eigenschaften und Optionen dieser Seite festlegen:

- Auswahl einer Seitenvorlage (standardmässig ist nur die Vorlage „Standalone Homepage“ verfügbar)
- Name der Seite
- Permalink (URL)
- ob diese Seite Ihre Startseite ersetzt oder nicht
- ob diese Seite eigenständig ist oder nicht (eine eigenständige Seite ist nicht an den Stil Ihrer Piwigo-Galerie gebunden und übernimmt daher die definierten CSS-Stile nicht).

Im Feld „Inhalt“ geben Sie den HTML-Code Ihrer Seite ein.

![Plugin AP.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-bcded356.jpg)

Wenn Sie das Plugin FCKEditor installiert haben, wird standardmässig ein HTML-Editor angezeigt, in dem Sie das Ergebnis sehen. Sie können den HTML-Code aber anzeigen, indem Sie FCKEditor unten rechts im Fenster deaktivieren.

![Plugin AP avec FCK.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-5e930604.jpg)

### Eine Startseite für Ihre Piwigo-Galerie erstellen

Das Plugin Additional Pages wird oft verwendet, um eine eigene Startseite für eine Piwigo-Galerie zu erstellen.

Die Seite, die standardmässig mit der Vorlage *Standalone Homepage* angeboten wird, ist dafür gedacht, eine Startseite zu erstellen, die ein ausgewähltes Foto aus Ihrer Galerie zeigt, wie in diesem Beispiel: [https://endangeredarts.com/](https://endangeredarts.com/) 

![Untitled](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-f3d57b74.png)

Wenn Sie dasselbe tun möchten, müssen Sie das Plugin Extended Description installieren. Damit können Sie Inhalte aus Ihrer Galerie auf der Seite anzeigen.

[Mehr über Extended Description erfahren](plugins-zur-galerie-anpassung.md)

Passen Sie anschliessend im HTML-Code, der beim Erstellen der Seite standardmässig vorhanden ist, den Inhalt des Tags (`[photo id=12345 size=L link=no]`) an Ihre Wünsche an:

- Ersetzen Sie 12345 durch die numerische ID des Fotos, das auf der Startseite angezeigt werden soll
- Ändern Sie die Grösse des angezeigten Fotos (SQ, TH, XXS, XS, S, M, L, XL oder XXL)
- Ändern Sie „link=no“ nicht

Sie können diesen Tag auch durch `[random album=xx]` ersetzen, wobei Sie xx durch die ID des gewünschten Albums ersetzen: So wird auf Ihrer Startseite automatisch ein zufälliges Foto aus dem ausgewählten Album angezeigt.

Sie können diesen Tag auch durch `[slider album=xx]` ersetzen, wobei Sie xx durch die ID des gewählten Albums ersetzen: So wird auf Ihrer Startseite eine Diashow mit Fotos aus dem ausgewählten Album angezeigt. Alle Optionen der Diashow können Sie über die Funktionen des Plugins Extended Descriptions steuern.

![Untitled](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-4ee672eb.png)

Und sobald Sie etwas Erfahrung mit HTML haben, sind die Möglichkeiten grenzenlos! Sie können zum Beispiel ein eigenes Navigationsmenü oben oder unten auf der Seite erstellen.

### Bestehende Seiten verwalten

Sobald Sie eine erste Seite erstellt haben, können Sie sie im Tab „Verwaltung“ ansehen und bearbeiten. Dort können Sie die erstellten Seiten auch neu anordnen.

### Konfiguration der zusätzlichen Seiten

Der Tab „Konfiguration“ bietet mehrere Optionen.

![Config AP.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-8c4cc10f.jpg)

**Verwaltung der Zugriffsrechte aktivieren**

Sie können die Verwaltung der Zugriffsrechte für zusätzliche Seiten aktivieren: nach Datenschutzstufe, nach Benutzertyp (Status), nach Benutzergruppe und nach Sprache. Wenn Sie eine dieser Optionen aktivieren, können Sie die Zugriffsrechte für jede Seite beim Bearbeiten festlegen.

![Niveaux confidentialité AP.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-14758bcb.jpg)

**Zusätzliche Seiten in Ihrer Galerie anzeigen**

Diese Optionen gelten für alle Ihre zusätzlichen Seiten.

Sie können festlegen:

- ob die zusätzlichen Seiten eine Schaltfläche zur Rückkehr zur Startseite enthalten
- ob die zusätzlichen Seiten über einen Menüeintrag erreichbar sind, und wie dieser Menüeintrag in den einzelnen Sprachen Ihrer Galerie heisst.

## Contact Form: ein Kontaktformular zu Ihrer Galerie hinzufügen

Mit dem Plugin Contact Form können Sie Ihrer Galerie eine Seite mit einem Kontaktformular hinzufügen.

Jedes Mal, wenn ein Besucher Ihrer Galerie dieses Formular ausfüllt, sendet Ihnen Ihre Piwigo-Galerie eine Benachrichtigung per E-Mail.

Sobald dieses Plugin aktiviert ist, öffnen Sie seine Konfigurationsseite.

### Konfiguration des Kontaktformulars

Im Tab „Konfiguration“ richten Sie Ihr Formular und seine Sichtbarkeit ein.

![Plugin CF.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-bd10c103.jpg)

Auf dieser Seite legen Sie fest:

- ob ein Link „Kontakt“ im Menü hinzugefügt wird
- ob Gäste (anonyme Besucher Ihrer Galerie) das Formular sehen dürfen
- ob der Benutzer nach dem Absenden des Formulars auf eine bestimmte URL weitergeleitet wird
- das Format der E-Mail, die nach dem Absenden des Formulars an den Administrator gesendet wird
- den Text (optional), der auf der Seite über und unter dem Formular angezeigt wird.

### Die E-Mail-Empfänger auswählen

Im Tab „E-Mails“ legen Sie fest, wer die Benachrichtigungen erhält, wenn jemand das Kontaktformular ausfüllt.

![CF emails.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-2ac5d66a.jpg)

Standardmässig erhalten alle Administratoren und Webmaster die E-Mails. Sie können einzelne Empfänger aber mit einem Klick auf das Kreuz entfernen.

Neue Empfänger fügen Sie über die Auswahlliste „Neuen Benutzer auswählen“ hinzu.

Schliesslich können Sie rechts weitere Empfänger hinzufügen, auch wenn diese keine Benutzer Ihrer Piwigo-Galerie sind.

### Das Formular in Ihrer Galerie anzeigen

Wenn Sie diese Option gewählt haben, ist das Formular über den Menüeintrag „Kontakt“ im Menüblock „Erweitert“ erreichbar ([mehr über Menüs erfahren](menue-und-navigationsleiste-anpassen.md)).

![Formulaire contacty.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-c28415ff.jpg)

Wenn Sie den Link zum Formular direkt im Hauptmenü Ihrer Galerie anzeigen möchten, ist das mit dem Plugin **Contact 1 Menu** möglich.

Dieses Plugin verschiebt den Menüeintrag „Kontakt“ direkt in die Hauptnavigationsleiste.

![Plugin C1M.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-7317d208.jpg)

### Crypto Captcha: Ihr Formular vor SPAM schützen

Leider erzeugen Formulare im Internet oft Spam, weil sie von Robotern ausgefüllt werden.

Um das zu verhindern, können Sie das Plugin **Crypto Captcha** installieren.

Mit diesem Plugin müssen Benutzer vor dem Absenden des Formulars ein Captcha eingeben. Für die Einrichtung Ihres Captchas stehen mehrere Optionen zur Verfügung.

![Plugin CC.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-5c63613e.jpg)

!!! info "Mit diesem Plugin können Sie auch ein Captcha für das Verfassen eines Kommentars oder das Erstellen eines neuen Benutzers hinzufügen."

### ⚠️ Häufige Probleme mit dem Plugin Contact Form

Wenn Ihnen jemand über das Kontaktformular eine Nachricht sendet, ist die Absenderadresse der Benachrichtigung die E-Mail-Adresse, die im Formular eingegeben wurde.

Ihre Piwigo-Website darf jedoch keine E-Mails im Namen einer Gmail-, Yahoo- oder Orange-Adresse versenden. Manche E-Mail-Anbieter blockieren diese E-Mails deshalb.

Daher kann es sein, dass über dieses Formular gesendete E-Mails nicht ankommen. Das passiert vor allem dann, wenn der Absender eine Gmail-Adresse verwendet und der Empfänger ebenfalls eine Gmail-Adresse hat.

Wenn dieses Problem auftritt, können Sie versuchen, es zu lösen, indem Sie die E-Mail-Adresse der Empfänger ändern (vermeiden Sie Gmail- oder Yahoo-Adressen).

Wenn Sie das Problem nicht lösen können, empfehlen wir Ihnen, Contact Form zu deinstallieren.
