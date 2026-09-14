---
title: Plugins für Administratoren - Piwigo-Dokumentation
description: Zusätzlich zu den klassischen Administrationsfunktionen von Piwigo stehen über Plugins weitere Optionen zur Verfügung. Wir stellen sie in diesem Artikel vor.
---

# Plugins für Administratoren

Zusätzlich zu den Standardfunktionen der Administration von Piwigo stehen über Plugins weitere Optionen zur Verfügung.

Wir stellen sie auf dieser Seite vor.

## Admin Tools: Piwigo direkt aus der Galerie administrieren

Mit dem Plugin **Admin Tools** können Administratoren einige Verwaltungsaufgaben direkt in der Galerie erledigen (Fotos bearbeiten, Alben bearbeiten …).

Sobald das Plugin Admin Tools aktiviert ist, erscheint in Ihrer Galerie eine neue Navigationsleiste, wenn Sie als Administrator angemeldet sind.

![Plugin admin tools.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-6a2bdf6f.jpg)

Über diese Werkzeugleiste gelangen Sie aus Ihrer Galerie zu den wichtigsten Seiten des Administrationsbereichs.

Auf der Seite eines Fotos erscheinen Verknüpfungen zu folgenden Verwaltungsaktionen:

- das Foto bearbeiten
- das Foto als Vorschaubild des Albums festlegen
- zur Auswahl hinzufügen

![Admin tools barre.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-874eee94.jpg)

In einem Fenster zur Schnellbearbeitung können Sie die wichtigsten Angaben zum Foto ändern, ohne den Administrationsbereich zu öffnen.

Dieselben Funktionen stehen auf den Albumseiten zur Verfügung.

Schliesslich finden Sie rechts in der Admin-Tools-Leiste weitere Werkzeuge:

![Outils supp.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-3f7e0949.jpg)

- Ansehen als: um die Galerie aus der Sicht eines anderen Benutzers zu sehen
- Schneller Wechsel des Erscheinungsbilds
- Schneller Wechsel der Sprache
- Die übrigen Optionen sind nur für Entwickler gedacht.

## Admin Messages: Eine Nachricht im Administrationsbereich hinzufügen

!!! info "Wenn Sie Kunde von Piwigo Cloud sind, ist dieses Plugin erst ab dem Enterprise-Tarif verfügbar"

Mit dem Plugin **Admin Messages** können Benutzer Nachrichten auf der Startseite des Administrationsbereichs von Piwigo hinterlassen (um mit den anderen Administratoren zu kommunizieren).

Die Nachrichten werden unten auf dem Dashboard angezeigt.

Zu jeder Nachricht werden der Name des Administrators, das Datum und die Nachricht angezeigt.

![Messages admin.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-e0045482.jpg)

## Protect Notification: Den Absender von Benachrichtigungs-E-Mails ändern

Manchmal landen die von Piwigo versendeten Benachrichtigungs-E-Mails im Spam-Ordner. Das liegt daran, dass sie mit der E-Mail-Adresse des Hauptadministrators (Webmasters) versendet werden. Wenn Ihr Server (oder als Kunde der Server von Piwigo Cloud) nicht berechtigt ist, E-Mails von dieser Adresse zu versenden, gelten die E-Mails als unsicher.

Um dieses Problem zu lösen, können Sie das Plugin **Protect Notif** installieren.

Sobald dieses Plugin aktiviert ist, werden alle Benachrichtigungs-E-Mails von Piwigo über eine fiktive Absenderadresse wie „no-reply@[`mygallery.com`](http://mygallery.com)“ versendet (ersetzen Sie `mygallery.com` durch Ihren Domainnamen).

Dadurch werden die Benachrichtigungs-E-Mails korrekt zugestellt.

!!! info "Seit Februar 2024 ist Protect Notif auf allen neu erstellten Konten bei Piwigo Cloud standardmässig aktiviert"


## Download Limits: Die Anzahl der Downloads pro Tag begrenzen

!!! info "Wenn Sie Kunde von Piwigo Cloud sind, ist dieses Plugin erst ab dem Enterprise-Tarif verfügbar"

Mit dem Plugin **Download Limits** können Administratoren die Anzahl der Downloads pro Tag in ihrer Galerie begrenzen.

!!! warning "Achtung:"
    Die maximale Anzahl der Downloads lässt sich nicht in der Oberfläche von Piwigo einstellen, sondern in einer Konfigurationsdatei. Wenn Sie Kunde von Piwigo Cloud sind, wenden Sie sich für die Einrichtung an den Support.


## Export Data: Die Daten Ihrer Piwigo-Galerie exportieren

!!! info "Wenn Sie Kunde von Piwigo Cloud sind, ist dieses Plugin erst ab dem Team-Tarif verfügbar"


Mit dem Plugin **Export Data** können Administratoren Daten aus Piwigo in eine Tabelle exportieren.

Folgende Daten können exportiert werden:

- Alben
- Fotos
- Kommentare
- Downloads

Die Daten werden in eine .CSV-Datei exportiert.

## FCK Editor: Einen WYSIWYG-Editor zu Piwigo hinzufügen

Mit dem Plugin **FCK Editor** fügen Sie den meisten Eingabefeldern im Administrationsbereich von Piwigo einen HTML-Editor mit Formatierungsoptionen hinzu:

- „Beschreibung“-Felder von Alben und Fotos
- Eigene Seiten (verfügbar mit dem Plugin **Additional Pages**)
- Eigene Blöcke (verfügbar mit dem Plugin **PWG Stuffs**)

Unten sehen Sie, wie Sie die Beschreibung eines Fotos mit FCK Editor formatieren.

![Description avancée.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-06abbf51.jpg)

Standardmässig wird auf den meisten Seiten die Basisversion von FCK Editor angezeigt, die verfügbaren Funktionen sind also begrenzt. Sie können aber weitere Funktionen aktivieren, wie im Screenshot unten zu sehen.

![image.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-93cd3f42.png)

**Wie aktivieren Sie alle diese Funktionen?**

- Wenn Ihr Piwigo bei Piwigo Cloud gehostet wird, wenden Sie sich an den Support.
- Wenn Sie Piwigo selbst hosten, folgen Sie der Anleitung unten.
- Klicken Sie hier, um die Anleitung anzuzeigen
    
    Die Konfiguration von FCK Editor befindet sich in der Datei `plugins/FCKEditor/fckeditor.tpl`.
    
    Bearbeiten Sie diese Datei und suchen Sie nach folgendem Code:
    
    ```jsx
    CKEDITOR.config.toolbar_Basic =
    [
      ["Source"],["Bold","Italic","Underline"],
      ["JustifyLeft","JustifyCenter","JustifyRight","JustifyBlock"],
      ["Styles","Format","Font","FontSize"],
      ["Link","Unlink","ShowBlocks"]
    ];
    ```
    
    Ersetzen Sie diesen Codeabschnitt durch folgenden Code:
    
    ```jsx
    CKEDITOR.config.toolbar_Basic =
    [
        ['Source','-','Save','NewPage','Preview','-','Templates'],
        ['Cut','Copy','Paste','PasteText','PasteFromWord','-','Print', 'SpellChecker', 'Scayt'],
        ['Undo','Redo','-','Find','Replace','-','SelectAll','RemoveFormat'],
        ['Form', 'Checkbox', 'Radio', 'TextField', 'Textarea', 'Select', 'Button', 'ImageButton', 'HiddenField'],
        '/',
        ['Bold','Italic','Underline','Strike','-','Subscript','Superscript'],
        ['NumberedList','BulletedList','-','Outdent','Indent','Blockquote'],
        ['JustifyLeft','JustifyCenter','JustifyRight','JustifyBlock'],
        ['Link','Unlink','Anchor'],
        ['Image','Flash','Table','HorizontalRule','Smiley','SpecialChar','PageBreak'],
        '/',
        ['Styles','Format','Font','FontSize'],
        ['TextColor','BGColor'],
        ['Maximize', 'ShowBlocks','-','About']
    ];
    ```
    

## LocalFiles Editor: Eigenen Code hinzufügen

Mit dem Plugin **LocalFiles Editor** können Sie Dateien von Piwigo direkt im Administrationsbereich bearbeiten.

!!! warning "Diese Funktion ist nur für fortgeschrittene Benutzer gedacht!"


Für Kunden von Piwigo Cloud erlaubt dieses Plugin nur das Hinzufügen von eigenem CSS-Code.

Wer Piwigo selbst hostet, kann mit diesem Plugin weitere Dateien bearbeiten (lokale Konfiguration, Sprachdateien usw.).

[Mehr über LocalFiles Editor erfahren](../piwigo-selbst-hosten/lokale-konfiguration-bearbeiten-localfiles-editor.md)

## Rightclick: Rechtsklick auf Fotos deaktivieren

Möchten Sie verhindern, dass die Besucher Ihrer Galerie die Fotos herunterladen können?

Zunächst können Sie Downloads für Gäste (anonyme Besucher) oder für bestimmte Benutzer in der Benutzerverwaltung sperren, [wie in diesem Artikel erklärt](../benutzer-verwalten/benutzer-erstellen-und-verwalten.md). Wenn Sie Downloads deaktivieren, wird das Download-Symbol nicht mehr angezeigt.

Besucher können Fotos aber weiterhin über Rechtsklick > Bild speichern unter herunterladen.

![Clic droit.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-eb7be9d9.jpg)

Um diese Möglichkeit zu unterbinden, aktivieren Sie einfach das Plugin **Rightclick**.

Sobald dieses Plugin aktiviert ist, ist der Rechtsklick auf Bilder in Ihrer Galerie deaktiviert (ausser für Administratoren).

## Piwishack: Ein Foto in eine Webseite einbinden

Möchten Sie Ihre Fotos in andere Websites einbinden?

Mit dem Plugin **Piwishack** können Sie für jedes Foto einen HTML-Code erzeugen, mit dem Sie das Foto in eine Webseite einbinden.

Sobald das Plugin Piwishack aktiviert ist, erscheint in Ihrer Galerie oberhalb der Fotos ein neues Symbol.

![Piwishack.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-f4ea2792.jpg)

Ein Klick auf dieses Symbol öffnet ein Fenster, in dem Sie verschiedene Codes abrufen können.

Der erste Reiter erzeugt mehrere HTML-Codes, mit denen Sie das Foto in eine Webseite einbinden.

![Fenêtre Piwishack.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-51d965e9.jpg)

Folgende Optionen stehen zur Verfügung:

- Vorschaubild ohne Link anzeigen
- Vorschaubild mit Link zum Foto in Ihrer Galerie anzeigen
- Vorschaubild mit direktem Link zum Foto anzeigen
- Normale Ansicht (Foto in normaler Grösse) ohne Link anzeigen
- Normale Ansicht (Foto in normaler Grösse) mit Link zum Foto in Ihrer Galerie anzeigen

Der zweite Reiter erzeugt mit denselben Optionen mehrere Codes im BBCode-Format (vor allem in Diskussionsforen verwendet).

Schliesslich können Sie auch eigene Codes erzeugen.

## Stop Spammers: Spam bekämpfen

Das Plugin **Stop Spammers** richtet in Ihrer Galerie eine Spam-Prüfung ein. Falls es nicht aktiviert ist, denken Sie daran, es zu aktivieren.

## AntiAspi: IP-Adressen aus Ihrer Galerie aussperren

Das Plugin AntiAspi schützt Ihre Galerie vor Robotern oder böswilligen Benutzern, die Ihre Website angreifen könnten, insbesondere um ihre Inhalte „abzusaugen“.

In den Einstellungen des Plugins legen Sie Kriterien fest, bei denen die IP-Adresse eines Besuchers Ihrer Website gesperrt wird, zum Beispiel:

- IP-Adresse sperren, wenn innerhalb von 10 Sekunden 20 verschiedene Seiten aufgerufen wurden
- IP-Adresse sperren, wenn dieselbe Seite innerhalb von 30 Sekunden 15-mal aufgerufen wurde
- usw.

Diese Kriterien sind anpassbar.

![Plugin AntiAspi.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-593652db.jpg)

Im Reiter IP-Adressen in den Einstellungen des Plugins AntiAspi sehen Sie den Verlauf der gesperrten IP-Adressen und können IP-Adressen hinzufügen, die immer zugelassen sind (Whitelist).

## Cookie Consent: Ein Einwilligungsbanner hinzufügen

Mit dem Plugin **Cookie Consent** fügen Sie Ihrer Website ein Banner hinzu, das Benutzer auffordert, ihre Einwilligung zu den grundlegenden Cookies zu bestätigen, die Ihre Galerie auf ihrem Computer speichern kann.

Sie können es auch verwenden, um Benutzer aufzufordern, den Nutzungsbedingungen Ihrer Galerie zuzustimmen.

![Cookie Consent.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-2796e715.jpg)

Der Text, die Beschriftung der Schaltfläche und der Link sind anpassbar.

Die Bestätigung wird in einem Cookie gespeichert, dessen Gültigkeitsdauer Sie festlegen können.

![Cookie Consent Config.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-d056bb42.jpg)

!!! warning "Achtung:"
    Wenn Ihre Galerie Cookies von Drittanbietern verwendet, etwa von Google Analytics, reicht dieses Banner nicht aus, um die Einwilligung Ihrer Besucher einzuholen. Es dient nur der Information (der Benutzer kann die Cookies weder ablehnen noch seine Einwilligung widerrufen).


## Plugins für die Suchmaschinenoptimierung Ihrer Galerie

Wenn Ihre Galerie öffentlich ist, möchten Sie wahrscheinlich, dass ihre Seiten bei Google und anderen Suchmaschinen gefunden werden.

Die folgenden Plugins sind nützlich, wenn Sie die Sichtbarkeit Ihrer Piwigo-Galerie in den Suchergebnissen (SEO) verbessern möchten.

### Title: Das Title-Tag der Seiten Ihrer Website anpassen

Mit diesem Plugin passen Sie das Meta-Tag „Title“ für alle Seiten Ihrer Galerie an.

Die Title-Tags der wichtigsten Seiten passen Sie in den Einstellungen des Plugins an.

![Plugin Title.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-b295d299.jpg)

Ausserdem können Sie das Title-Meta-Tag jedes Fotos und jedes Albums auf der jeweiligen Bearbeitungsseite zusammen mit den übrigen Eigenschaften ändern.

![Options de titre.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-e6063dcd.jpg)

### Meta: Die Meta-Tags der Seiten Ihrer Website anpassen

Neben dem Title-Meta-Tag, das Sie mit dem Plugin **Title** anpassen, lassen sich in Piwigo mit dem Plugin **Meta** weitere Tags für die Suchmaschinenoptimierung (SEO) einrichten.

Das Plugin unterstützt folgende Meta-Tags:

- author
- description
- keywords
- robots

Im ersten Reiter der Plugin-Einstellungen können Sie einige Meta-Tags global für alle Seiten der Website festlegen.

![Plugin meta.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-14761527.jpg)

Mit dem Tag **robots** legen Sie unter anderem fest, ob Ihre Website von Suchmaschinen indexiert werden soll oder nicht:

- wenn Ihre Galerie nicht indexiert werden soll, geben Sie `noindex` ein
- wenn Ihre Galerie indexiert werden soll, geben Sie `index` ein

Das Meta-Tag **Description** empfehlen wir Ihnen für jede Seite einzeln festzulegen. Es ist eine wichtige Angabe für die Suchmaschinenoptimierung, da es in den Suchergebnissen angezeigt wird.

![Titre et description.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-cc312049.jpg)

Das Description-Meta-Tag jedes Fotos und jedes Albums können Sie auf der jeweiligen Bearbeitungsseite zusammen mit den übrigen Eigenschaften ändern.

![Edition photo meta.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-61f178c7.jpg)

Im Reiter „Custom metadata“ der Plugin-Einstellungen können Sie eigene Meta-Tags hinzufügen.

![Ajouter une meta.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-cdf64f3a.jpg)

### Meta Open Graph: Die Open-Graph-Meta-Tags für soziale Netzwerke anpassen

Mit den Open-Graph-Meta-Tags passen Sie den Inhalt der Vorschau an, die beim Teilen einer Seite in sozialen Netzwerken angezeigt wird.

Diese Daten sind in Piwigo standardmässig nicht vorhanden. Wenn Sie den Link zu Ihrer Galerie teilen, werden der Titel der Galerie und ein zufällig ausgewähltes Foto angezeigt.

Um diese Meta-Tags in Ihrer Piwigo-Galerie anzupassen, können Sie das Plugin **Meta Open Graph** installieren.

In den Einstellungen dieses Plugins passen Sie die Open-Graph-Meta-Tags für jede Seite Ihrer Galerie an.

![Open Graph.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-6ff33e11.jpg)

Wählen Sie eine Seite, zum Beispiel die Startseite, und klicken Sie auf „Edit Open Graph metadata“.

Geben Sie einen Titel und eine Beschreibung ein und wählen Sie das Foto aus, das die Seite repräsentieren soll (über die Auswahlliste oder durch Eingabe der ID des gewünschten Fotos im Feld „Metadata Open Graph link image“).

![Description plus longue.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-15c721c8.jpg)

Klicken Sie auf „Speichern“.

Wenn Sie die Seite jetzt in sozialen Netzwerken (etwa Facebook) teilen, berücksichtigt die Vorschau die eingegebenen Tags.

![Capture d’écran 2024-08-20 à 14.34.01.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-a21553df.png)

Für jedes Foto und jedes Album können Sie im Administrationsbereich auf der Bearbeitungsseite des Fotos bzw. Albums eigene Meta-Tags angeben.

![Options Open Graph.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-86be356c.jpg)

Im Reiter Konfiguration auf der Einstellungsseite des Plugins legen Sie Standardeinstellungen fest.

![Config Open Graph.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-7bae3079.jpg)

Unter anderem können Sie damit:

- ein bestimmtes Bild für die Meta-Tags Ihrer Alben und Fotos festlegen (standardmässig werden das Foto bzw. das Vorschaubild des Albums verwendet)
- ein Album festlegen, aus dem ein zufälliges Foto für das Meta-Bild gewählt wird, wenn keines angegeben ist
- die Grösse des verwendeten Fotos wählen
- die Standardsprache festlegen
- den Namen Ihrer Website angeben
- eine Facebook-App-ID eingeben
- die Art der Karte festlegen, die beim Teilen auf Twitter angezeigt wird (Twitter Card)
- Ihre Twitter-ID eingeben, falls Sie eine haben

[Mehr über die Open-Graph-Meta-Tags von Facebook erfahren](https://developers.facebook.com/docs/sharing/opengraph/using-objects?locale=fr_FR)

[Mehr über Twitter Cards erfahren](https://developer.twitter.com/en/docs/twitter-for-websites/cards/guides/getting-started)

## Plugins, um eigenen Code in Ihre Galerie einzufügen

Es gibt zwei Plugins, mit denen Sie eigenen Code in Ihre Piwigo-Galerie einfügen können.

Es lohnt sich, beide zu kennen, da sie sich gut ergänzen.

So können Sie zum Beispiel mit dem ersten Code im <head>-Tag einfügen und mit dem zweiten im Fussbereich der Website (vor dem schliessenden <body>-Tag).

### Add < head > element: Code im <head>-Tag einfügen

Mit dem Plugin **Add < head > element** fügen Sie Code (zum Beispiel ein JavaScript-Skript) in das <head>-Tag Ihrer Galerie ein. Sie können wählen, ob dieser Code in der Galerie, im Administrationsbereich oder in beiden aktiv sein soll.

### Statistics: Code im <head>-Tag oder im Fussbereich einfügen

Das Plugin Statistics ist dafür gedacht, den Tracking-Code eines externen Statistik-Tools (etwa Matomo oder Google Analytics) in Ihre Galerie einzufügen. Sie können damit aber auch Code für andere Zwecke einfügen.

Sie geben den gewünschten Code ein und wählen, ob er im Kopfbereich der Website, im Fussbereich oder in beiden eingefügt wird.

Mit der Option „Exclude administrators from statistics“ wird der eingegebene Code nicht ausgeführt, wenn ein Administrator angemeldet ist.

Mit der Option „Exclude guests from statistics“ wird der eingegebene Code nicht ausgeführt, wenn Gäste der Galerie nicht angemeldet sind.
