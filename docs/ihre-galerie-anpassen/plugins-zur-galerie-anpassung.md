---
title: Plugins zur Anpassung Ihrer Galerie - Piwigo-Dokumentation
description: In diesem Artikel finden Sie einige Plugins, mit denen Sie das Aussehen und die Funktionen Ihrer Piwigo-Galerie anpassen können.
---

# Ihre Galerie mit Plugins anpassen

Auf dieser Seite finden Sie einige Plugins, mit denen Sie das Aussehen und die Funktionen Ihrer Galerie anpassen können.

Weitere Plugins zur Anpassung Ihrer Galerie finden Sie in den folgenden Artikeln:

[Die Albumseite in Ihrer Galerie](../ihre-piwigo-galerie-erkunden/alben-in-ihrer-galerie.md)

[Die Fotoseite in Ihrer Galerie](../ihre-piwigo-galerie-erkunden/die-fotoseite-in-ihrer-galerie.md)

[Schlagworte in Ihrer Galerie](../ihre-piwigo-galerie-erkunden/schlagworte-in-ihrer-galerie.md)

## PWG Stuffs: anpassbare Blöcke zu Ihrer Galerie hinzufügen

Das Plugin **PWG Stuffs** bietet verschiedene Möglichkeiten, anpassbare Blöcke zu Ihrer Galerie hinzuzufügen.

Diese Blöcke ergänzen die bestehenden Seiten. Damit ist es ein sehr umfassendes Plugin zur Anpassung Ihrer Galerie. Unter anderem können Sie damit die Anzeige je nach Benutzer anpassen.

Es wird zum Beispiel verwendet, um:

- eine Schlagwortwolke auf der Startseite hinzuzufügen
- einen Anmeldebereich auf der Startseite hinzuzufügen
- usw.

Klicken Sie unten, um die vollständige Dokumentation zu PWG Stuffs zu lesen.

[PWG Stuffs: Blöcke in Ihrer Galerie hinzufügen](../ihre-galerie-anpassen/plugins-zur-galerie-anpassung/pwg-stuffs-bloecke-in-ihrer-galerie-hinzufuegen.md)

## Fotorama: eine andere Diashow für Ihre Galerie

Mit dem Plugin **Fotorama** können Sie die Diashow, die Ihre Piwigo-Galerie standardmässig verwendet, durch eine andere ersetzen.

In den Einstellungen des Plugins gibt es verschiedene Anpassungsmöglichkeiten.

![Vollbild-Diashow mit Fotorama](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-14cf1f90.jpg)

Vollbild-Diashow mit Fotorama

## Extended Description: viele Möglichkeiten zur Anpassung Ihrer Galerie

Das Plugin Extended Description bietet viele Möglichkeiten. Unter anderem können Sie damit die Titel und Beschreibungen von Alben und Fotos in mehrere Sprachen übersetzen, [wie in diesem Artikel erklärt.](verfuegbare-sprachen-der-galerie-verwalten.md)

Es kann aber noch viel mehr.

Sie können damit nämlich Tags verwalten, die Sie an beliebiger Stelle in Ihrer Galerie einfügen können.

Damit können Sie zum Beispiel:

- zwei verschiedene Beschreibungen für ein Album verwalten (eine kurze in der Albumliste und eine lange auf der Albumseite)
- ein Album oder ein Foto in ein beliebiges Textfeld Ihrer Galerie einfügen
- ein Karussell (oder eine Diashow) in ein beliebiges Textfeld Ihrer Galerie einfügen
- ein Album auf der Seite des übergeordneten Albums oder im Menü ausblenden
- ein Foto auf einer Albumseite ausblenden
- ein Album auf eine beliebige URL weiterleiten
- ein Element auf ein Foto, ein Album oder eine Suchseite weiterleiten
- einen Anmeldelink zur Galerie an beliebiger Stelle einfügen.

Sobald Sie Extended Description installiert haben, erscheint neben den Eingabefeldern ein Symbol in Form eines Fragezeichens: Klicken Sie darauf, um alle Optionen des Plugins anzuzeigen.

Wir haben sie unten alle aufgelistet.

- **Die vollständige Dokumentation des Plugins Extended Descriptions ansehen**
    
    **Mehrsprachige Beschreibungen**
    
    Mehrsprachige Beschreibungen stehen zwischen den Tags `[lang=xx]` und `[/lang]`, wobei xx der Sprachcode ist (zum Beispiel: en, fr, es...).
    
    ```html
    [lang=en]Default description[/lang]
    [lang=fr]Description en français[/lang]
    [lang=de]Deutsche Beschreibung[/lang]
    ```
    
    **Tag *default***
    
    Wenn die Beschreibung nicht in der Sprache des Benutzers vorhanden ist, wird die Standardbeschreibung verwendet.
    Wenn `[lang=default]` nicht vorhanden ist, gilt alles, was ausserhalb der Sprach-Tags steht, als Standardbeschreibung.
    
    ```html
    [lang=default]Default description[/lang]
    [lang=fr]Description en français[/lang]
    
    // OR
    
    Default description
    [lang=fr]Description en français[/lang]
    ```
    
    **Tag *all***
    
    Alles, was zwischen den Tags `[lang=all]` und `[/lang]` steht, wird unabhängig von der Sprache des Benutzers in die Beschreibung übernommen.
    Das ist besonders nützlich, um HTML- oder Javascript-Code in eine Beschreibung einzufügen.
    
    ```html
    [lang=all]<p>[/lang]
      [lang=default]Default description[/lang]
      [lang=fr]Description en français[/lang]
      [lang=de]Deutsche Beschreibung[/lang]
    [lang=all]</p>[/lang]
    ```
    
    **Erweiterte Beschreibungen**
    
    Mit den Tags für erweiterte Beschreibungen können Sie eine gekürzte Beschreibung für die Vorstellung eines Albums verwenden, eine längere Beschreibung auf der Albumseite anzeigen oder zwei verschiedene Beschreibungen auf der Albumseite haben.
    
    **<!--more-->**
    
    In der Vorstellung des Albums wird nur die gekürzte Beschreibung angezeigt. Im Album selbst besteht die Beschreibung aus der gekürzten Beschreibung und der ausführlichen Beschreibung.
    
    ```html
    shortened description <!--more--> detailed description
    ```
    
    **<!--complete-->**
    
    In der Vorstellung des Albums wird nur die gekürzte Beschreibung angezeigt. Im Album selbst besteht die Beschreibung jedoch nur aus der ausführlichen Beschreibung. Es handelt sich also um 2 verschiedene Beschreibungen.
    
    ```html
    shortened description <!--complete--> detailed description
    ```
    
    **<!--up-down-->**
    
    In der Vorstellung des Albums wird nur die obere Beschreibung angezeigt. Im Album selbst wird die obere Beschreibung über den Vorschaubildern angezeigt, die untere Beschreibung darunter (dort, wo die Beschreibung normalerweise steht).
    
    ```html
    upper description <!--up-down--> lower description
    ```
    
    **Ein Album oder ein Foto einfügen
    [photo id=xx]**
    
    Mit diesem Tag können Sie ein Foto in beliebiger Grösse einfügen.
    
    **Optionen:**
    • `id` die Nummer des Fotos
    • `album` (optional) die Nummer des übergeordneten Albums
    • `size` (optional) die Grösse des Fotos, eine von *SQ, TH, XXS, XS, S, M, L, XL, XXL*
    • `html` (optional) bei `false` liefert der Tag nur die URL des Fotos, ohne HTML
    • `link` (optional) bei `true` ist das Foto anklickbar und führt zu seiner Seite
    
    ```html
    [photo id=46]
    
    [photo id=46 album=22 size=M html=true link=true]
    ```
    
    **[random album=xx]**
    Die Optionen sind dieselben, ausser dass die Fotos zufällig aus der ganzen Galerie oder aus `album` ausgewählt werden.
    Um mehrere Fotos anzuzeigen, verwenden Sie die Option:
    • `nb_images` (optional) die Anzahl der anzuzeigenden Fotos
    
    ```html
    [random]
    
    [random album=123 size=M html=yes link=yes]
    
    [random album=123 size=M html=yes link=yes nb_images=8]
    ```
    
    **[cat=xx]**
    
    Mit diesem Tag können Sie ein Album in die Beschreibung einfügen, wobei `xx` die Nummer des Albums ist.
    
    **Ein Karussell einfügen
    [slider album=xx]**
    Damit können Sie eine Diashow einfügen.
    
    **Optionen:** (Sie müssen `album` ODER `list` angeben)
    • `album` (optional) Quellalbum
    • `nb_images` (optional) maximale Anzahl Fotos in der Diashow
    • `random` (optional) die Fotos zufällig aus dem Album auswählen
    • `list` (optional) eine Liste von Fotos, durch Kommas getrennt
    • `size` (optional) die Grösse der Fotos, eine von *SQ, TH, XXS, XS, S, M, L, XL, XXL*
    • `speed` (optional) die Geschwindigkeit der Diashow (in Sekunden)
    • `title` (optional) den Namen des Fotos anzeigen
    • `effect` (optional) Übergangseffekt (siehe [die Dokumentation von NivoSlider](http://docs.dev7studios.com/jquery-plugins/nivo-slider#jumpNav-5))
    • `arrows` (optional) Navigationspfeile anzeigen
    • `elastic` (optional) die Grösse der Diashow an jedes Foto anpassen
    • `control` (optional) die Navigationsleiste anzeigen, kann auch `thumb` sein
    • `thumbs_size` (optional) Grösse der Vorschaubilder in Pixeln, wenn `control=thumb`
    
    ```html
    [slider album=123]
    
    [slider list=46,47,52]
    
    [slider album=123 nb_images=10 random=false size=M speed=3 title=false effect=fade arrows=true elastic=false control=true thumbs_size=80]
    ```
    
    **Ein Element ausblenden**
    
    **Ein Album ausblenden**
    
    Verwenden Sie den Tag `<!--hidden-->` im Namen des Albums:
    • es wird nicht mehr auf der Seite des übergeordneten Albums angezeigt
    • es bleibt im Albummenü sichtbar
    
    **Ein Album im Menü ausblenden**
    
    Verwenden Sie den Tag `<!--mb-hidden-->` im Namen des Albums:
    • es wird nicht mehr im Albummenü angezeigt
    • es bleibt auf der Seite des übergeordneten Albums sichtbar
    
    **Ein Foto ausblenden**
    
    Verwenden Sie den Tag `<!--hidden-->` im Namen des Fotos:
    • es wird nicht mehr auf der Seite mit den Vorschaubildern angezeigt
    • im Album selbst bleibt es jedoch sichtbar
    
    **Ein Element weiterleiten**
    
    **[redirect http://piwigo.org]**
    Fügen Sie diesen Tag in die Beschreibung eines Albums ein, um es auf eine URL Ihrer Wahl weiterzuleiten.
    
    **[redirect img=xx]**
    Leitet auf ein Foto Ihrer Galerie weiter, wobei `xx` seine ID ist. Sie können nach der Nummer des Fotos auch die ID des Albums angeben: `xx.ccc`.
    
    **[redirect cat=xx]**
    Leitet auf ein Album Ihrer Galerie weiter, wobei `xx` seine ID ist.
    
    **[redirect search=xx]**
    Leitet auf eine Suchseite Ihrer Galerie weiter, wobei `xx` die ID der Suchseite ist.
    
    **Anmeldelink und Block für angemeldete Benutzer
    [login-link]**
    Mit diesem Tag können Sie an beliebiger Stelle einen Anmeldelink einfügen, der automatisch auf die aktuelle Seite zurückleitet.
    
    **Optionen:**
    • `html` (optional) bei `false` liefert der Tag nur die URL des Links, ohne HTML
    • `text` (optional) Text des Links, kann `[lang]`-Tags enthalten
    
    ```html
    [login-link]
    
    [login-link html=true text="log in[lang=en]log-in[/lang]"]
    ```
    
    **[logged]**
    Zeigt einen Textblock an, je nachdem, ob der Benutzer angemeldet ist oder nicht.
    
    ```html
    [logged=true] Welcome back [/logged]
    [logged=false] Please log in [/logged]
    ```
    

## Perso Footer: die Fusszeile Ihrer Galerie anpassen

Standardmässig zeigt die Fusszeile Ihrer Galerie einen Vorstellungstext zu Piwigo, einen Link zum Anmelden bzw. Abmelden und einen Link, um dem Webmaster der Galerie eine E-Mail zu senden (nur für Kunden von Piwigo cloud).

![Pied de page basique.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-02bf4b28.jpg)

Mit dem Plugin **Perso Footer** können Sie dieser Fusszeile Inhalte hinzufügen.

In den Einstellungen dieses Plugins finden Sie ein Texteingabefeld, in das Sie einfachen Text oder HTML-Code einfügen können.

Wenn Sie zusätzlich das Plugin FCKEditor installieren, das den Texteingabefeldern einen visuellen Editor zum Formatieren von Text hinzufügt, können Sie ganz einfach eine eigene Fusszeile gestalten.

![Plugin PF config.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-cefaec71.jpg)

## Personal Favicon: das Symbol Ihrer Galerie im Browser anpassen

Standardmässig ist das Favicon Ihrer Piwigo-Galerie, also das Symbol, das im Browser angezeigt wird, das Symbol von Piwigo cloud.

![Untitled](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-8435a237.png)

Sie können dieses Symbol anpassen, indem Sie das Plugin **Perso Favicon** aktivieren.

Sobald dieses Plugin aktiviert ist, öffnen Sie seine Konfigurationsseite.

In Piwigo können Sie eine Datei hochladen (Endung .ico, max. 5 KB), die das Standardsymbol ersetzt.

![Plugin PF.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-7ab12eea.jpg)

## OpenStreetMap: Ihre Fotos auf einer interaktiven Karte verorten

Das Plugin OpenStreetMap basiert auf dem freien Kartenprojekt [OpenStreetMap](https://www.openstreetmap.fr/). Damit können Sie Ihre Fotos anhand ihrer GPS-Koordinaten auf einer Karte anzeigen.

Hier sehen Sie ein Beispiel für eine Galerie, die Geolokalisierung mit OpenStreetMap nutzt: [https://laseineavelo.piwigo.com/](https://laseineavelo.piwigo.com/)

Die Karte kann angezeigt werden:

- auf der Startseite von Piwigo
    
    ![Plugin OSM.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-5d071890.jpg)
    
- auf einer Albumseite
    
    ![OSM page album.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-90f3d987.jpg)
    
- auf einer Fotoseite
    
    ![Carte sur page image.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-0dd4baba.jpg)
    

Ausserdem kann das Plugin eine Seite hinzufügen, die über das Menü der Galerie erreichbar ist und eine Karte im Vollbild öffnet.

![Carte plein écran.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-034adaee.jpg)

Wenn Sie auf der Karte auf einen Punkt klicken, werden das zugehörige Foto und die verfügbaren Informationen angezeigt, etwa der Titel des Fotos oder sein Autor. Ein Klick auf das Bild öffnet die Seite des Fotos.

![Focus sur image.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-6389439b.jpg)

Wenn Sie ein Foto im Administrationsbereich bearbeiten, können Sie im Tab OpenStreetMap die geografischen Koordinaten des Fotos ansehen und bei Bedarf ändern.

![Edition photo OSM.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-b5a3a44e.jpg)

Sie können die GPS-Koordinaten mehrerer Fotos auch gleichzeitig in der Stapelverarbeitung bearbeiten.

![OSM GeoTag BM.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-b775355d.jpg)

In den Einstellungen des Plugins stehen viele Konfigurationsoptionen zur Verfügung. Sie können zum Beispiel das Aussehen der Karte und ihre Grösse ändern oder festlegen, ob die Standortbestimmung aktiviert ist…

![Untitled](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-8d4fc096.png)

![Untitled](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-f72fd449.png)

Sie können sogar einen eigenen Stil für die Farben Ihrer Karte und für die Markierungen erstellen, die die Fotos darstellen.

## Header Manager: das Banner Ihrer Galerie einfach verwalten

Es gibt mehrere Möglichkeiten, Ihrer Piwigo-Galerie ein Banner hinzuzufügen.

Die einfachste finden Sie im Administrationsbereich im Menü **Konfiguration > Optionen**, im Tab **Allgemein**, Abschnitt **Grundeinstellungen**. Dort können Sie HTML-Code für Ihr Banner eingeben.

Das Plugin **Header Manager** bietet Ihnen mehr Möglichkeiten, Ihr Banner einzurichten.

![Bannière photo.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-495987f6.jpg)

Mit diesem Plugin können Sie:

- ein oder mehrere Bilder hochladen oder eines der Fotos Ihrer Galerie auswählen
- Ihr Bild online zuschneiden, um Ihr Banner zu erstellen
- Ihr Banner anpassen:
    - nur ein Bild anzeigen
    - den Titel Ihrer Galerie über dem Bild anzeigen (als transparenter Text)
    - das Bild und einen Text Ihrer Wahl anzeigen
    - festlegen, ob das Banner auf den Fotoseiten angezeigt wird
    - zufällig zwischen mehreren Bannern wechseln
    - für jedes Album ein eigenes Banner festlegen

Mehr über das Erstellen eines Banners, mit oder ohne dieses Plugin, erfahren Sie in diesem Artikel:

[Eigenes Banner](eigenes-banner-zur-galerie-hinzufuegen.md)

## Paypal Shopping Cart: Fotos in Ihrer Galerie mit Paypal verkaufen

Möchten Sie zum Beispiel Abzüge Ihrer Fotos in Ihrer Galerie verkaufen?

Das ist mit dem Plugin **Paypal Shopping Cart** möglich.

Um dieses Plugin zu nutzen, müssen Sie zuerst ein PayPal-Konto erstellen.

**Dieses Konto muss dieselbe E-Mail-Adresse verwenden wie der Webmaster Ihrer Galerie.**

In der Konfiguration des Plugins PayPal Shopping Cart können Sie Folgendes festlegen:

- die auf Ihrer Website verwendete Währung
- die Aktivierung des PayPal-Warenkorbs für die ganze Galerie oder nur für einzelne Alben
- unterschiedliche Preise je nach Grösse der Fotos
- den Betrag der Versandkosten (pauschal)

Sobald diese Punkte eingerichtet sind, erscheint auf den Fotoseiten der betroffenen Alben eine Schaltfläche „In den Warenkorb“.

![PayPal Images.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-91f408b3.png)

Wenn ein Foto in den Warenkorb gelegt wird, öffnet sich automatisch eine PayPal-Zahlungsseite. Der Besucher kann aber zu Ihrer Galerie zurückkehren und weitere Fotos in seinen Warenkorb legen.

Sobald er mit dem Einkaufen fertig ist, kann er seine Bestellung bei PayPal abschliessen.

![Panier achats.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-ae87289b.jpg)

---
