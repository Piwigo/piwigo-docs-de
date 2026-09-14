---
title: Was ist ein Erscheinungsbild? Piwigo-Dokumentation
description: Wofür werden Erscheinungsbilder in Piwigo verwendet? Wie installiere und passe ich sie an?
---

# Einführung in Erscheinungsbilder

## Was ist ein Erscheinungsbild in Piwigo?

Wie Sie wahrscheinlich schon wissen, ist Piwigo in zwei Oberflächen aufgeteilt:

- den Administrationsbereich, auf den nur Administratoren Zugriff haben;
- die Galerie, die normalen Benutzern und, wenn Ihre Galerie öffentlich ist, sogar allen Besuchern offenstehen kann.

Ihre Piwigo-Galerie ist eine Website, die Sie anpassen können: Farben, Schriften, Seitenaufbau…

Um Ihre Galerie anzupassen, müssen Sie aber zuerst ein Erscheinungsbild wählen, auch „Template“ genannt: Es ist die Vorlage Ihrer Galerie.

Verschiedene Beispiele für Anpassungen mit unterschiedlichen Erscheinungsbildern finden Sie auf unserer [Demo-Seite](https://piwigo.com/demo).

In einem Blogartikel stellen wir ausserdem [8 Beispiele für die grafische Anpassung von Piwigo](https://piwigo.com/blog/2022/02/03/8-examples-customized-piwigo-galleries/) vor.

## Standard-Erscheinungsbilder

Piwigo wird immer mit zwei standardmässig aktivierten Erscheinungsbildern installiert:

- Modus in der schwarz-weissen Variante: Dieses Erscheinungsbild verwendet Ihre Galerie, wenn Sie sie auf einem Computer aufrufen;
    
    ![Page accueil Modus.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-041139c5.jpg)
    
- Smart Pocket: Dieses Erscheinungsbild wird nur auf einem Smartphone oder Tablet angezeigt.
    
    ![Screenshot_20240723_122220_Chrome.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-2ec1e5de.jpg)
    

Sie können aber natürlich:

- die Farben des Erscheinungsbilds Modus ändern
- ein anderes Erscheinungsbild für Ihre Galerie verwenden
- das mobile Erscheinungsbild Smart Pocket deaktivieren (in diesem Fall verwendet Ihre Galerie auf einem mobilen Bildschirm dasselbe Erscheinungsbild wie auf einem Computer. Mit den Erscheinungsbildern Modus und Bootstrap Darkroom ist das kein Problem, denn sie sind *responsiv*, passen sich also an alle Bildschirmgrössen an).

## Kunden von Piwigo Cloud und selbst gehostete Galerien: Unterschiede beim Hinzufügen eines Erscheinungsbilds

Sie möchten ein neues Erscheinungsbild hinzufügen? Vorab sollten Sie wissen, dass das Vorgehen etwas anders ist, je nachdem, ob Sie ein Konto bei [Piwigo Cloud](https://de.piwigo.org/piwigo-bekommen) haben oder eine selbst gehostete Piwigo-Galerie nutzen.

- Ich nutze eine selbst gehostete Galerie
    
    Wenn Sie eine selbst gehostete Galerie nutzen, können Sie selbst ein neues Erscheinungsbild im Administrationsbereich hinzufügen: im Menü Konfiguration > Erscheinungsbilder, Registerkarte „Ein neues Erscheinungsbild hinzufügen“.
    
    Sie können ein Erscheinungsbild auch auf [piwigo.org](https://de.piwigo.org/) herunterladen und per FTP zu Ihrer Piwigo-Galerie hinzufügen.
    
    Denken Sie ausserdem daran, Ihre installierten Erscheinungsbilder zu aktualisieren, wenn ein Update verfügbar ist.
    
- Ich habe ein Piwigo-Konto, das bei Piwigo Cloud gehostet wird
    
    Wenn Sie ein Konto bei Piwigo Cloud erstellt haben, wird Ihre Piwigo-Galerie auf unseren Servern gehostet.
    
    Ihr Konto wurde mit einer Liste vorinstallierter Erscheinungsbilder eingerichtet. Sie können kein neues installieren. Um Updates der Erscheinungsbilder müssen Sie sich nicht kümmern.
    

## Erscheinungsbilder in Piwigo verwalten

Um Ihr Erscheinungsbild in Piwigo anzusehen, zu bearbeiten und einzurichten, öffnen Sie den Administrationsbereich und klicken Sie im Menü links auf Konfiguration > Erscheinungsbilder.

Oben auf der Seite sehen Sie unter „Aktive Erscheinungsbilder“ die Erscheinungsbilder, die in Ihrer Galerie aktiviert sind.

Weiter unten sehen Sie unter „Inaktive Erscheinungsbilder“ die Erscheinungsbilder, die installiert, aber nicht aktiviert sind.

![Tous les thèmes.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-f34d0747.jpg)

Ein aktiviertes Erscheinungsbild kann in Piwigo angezeigt werden.

Wenn Sie es als „Standard“ festlegen, wird es allen neuen Benutzern standardmässig angezeigt.

Sie können aber für jeden Benutzer einzeln festlegen, welches Erscheinungsbild er sieht: Deshalb lassen sich mehrere Erscheinungsbilder gleichzeitig aktivieren.

!!! info "Info:"
    In den allermeisten Fällen wird nur ein Erscheinungsbild aktiviert, das für alle Benutzer gleich ist (abgesehen vom Erscheinungsbild Smart Pocket, das, wenn es aktiviert ist, automatisch beim Aufrufen der Galerie auf einem mobilen Gerät angezeigt wird).

## Das Standard-Erscheinungsbild ändern

Das Standard-Erscheinungsbild Ihrer Galerie zu ändern, ist ganz einfach.

Wählen Sie auf der Seite im Menü Konfiguration > Erscheinungsbilder das Erscheinungsbild aus, das Ihre Galerie anzeigen soll, und klicken Sie auf die Schaltfläche „Aktivieren“.

![Activation thème BD.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-e54c19d8.jpg)

Nach der Aktivierung ist dieses Erscheinungsbild in Ihrer Galerie verfügbar, wird aber noch nicht standardmässig angezeigt: Dazu müssen Sie auf „Als Standard einstellen“ klicken.

![Activer thème BD.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-1dcfd849.jpg)

Öffnen Sie Ihre Galerie: Das neue Erscheinungsbild wird verwendet.

## Ihr Erscheinungsbild einrichten

Die Wahl eines Erscheinungsbilds ist nur der erste Schritt, um Ihre Galerie anzupassen. Die meisten Erscheinungsbilder bieten nämlich Konfigurationsoptionen, mit denen Sie:

- die Farben Ihrer Galerie ändern
- einige Anzeigeoptionen ändern
- Elemente zur Anpassung hinzufügen (Logo, Banner usw.)
- optionale Komponenten aktivieren

Die neuesten Erscheinungsbilder, [Modus](modus-erscheinungsbild.md) und [Bootstrap Darkroom](bootstrap-darkroom-erscheinungsbild.md), bieten viele Farbstile und Konfigurationsoptionen. Andere, ältere Erscheinungsbilder lassen sich nicht anpassen.

Wir empfehlen Ihnen, sich die Optionen der wichtigsten Erscheinungsbilder anzusehen, bevor Sie sich entscheiden. 

## Die wichtigsten Erscheinungsbilder im Überblick

### Modus

Modus ist das Erscheinungsbild, das in Piwigo standardmässig aktiviert ist. Es ist modern, responsiv und garantiert die Kompatibilität mit den meisten Plugins. Sein Navigationsmenü ist horizontal.

![Page accueil Modus.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-041139c5.jpg)

Es bietet 18 verschiedene Farbschemas, die Sie in seinen Konfigurationsoptionen auswählen können.

![Liste thèmes Modus.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-80c0803e.jpg)

Ausserdem können Sie damit:

- Grösse und Format der Vorschaubilder Ihrer Alben anpassen (standardmässig quadratische Vorschaubilder mit 250 x 250 Pixeln)
- ein Banner in Ihrer Galerie hinzufügen

[Dokumentation zum Erscheinungsbild Modus lesen](modus-erscheinungsbild.md)

### Bootstrap Darkroom

Nach Modus ist es derzeit das zweitbeliebteste Erscheinungsbild.

Bootstrap Darkroom ist ein modernes, responsives und sehr anpassbares Erscheinungsbild. Es basiert auf dem Framework Bootstrap 4, einem sehr beliebten Open-Source-Projekt zur Gestaltung von Weboberflächen. Sein Navigationsmenü ist horizontal.

![Page d'accueil BD.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-e6a71abd.jpg)

Bootstrap Darkroom bietet über 30 sehr unterschiedliche Farbstile.

![Couleurs BD.gif](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-41cb4d0e.gif)

Neben diesen Farbstilen bietet Bootstrap Darkroom viele Konfigurationsoptionen:

- Logo hinzufügen
- Banner hinzufügen (Bild, Text)
- zahlreiche Anzeigeoptionen ändern
- eigenen CSS-Code hinzufügen
- Symbole zum Teilen in sozialen Netzwerken hinzufügen
- …

[Dokumentation zum Erscheinungsbild Bootstrap Darkroom lesen](bootstrap-darkroom-erscheinungsbild.md)

### Elegant

Elegant war viele Jahre lang sehr beliebt und wird immer noch häufig verwendet. Es hat ein senkrechtes Navigationsmenü am linken Bildschirmrand. Die Alben werden statt als Vorschaubilder als grosse Blöcke angezeigt, sodass Sie zu jedem Album auf Wunsch einen Beschreibungstext anzeigen können.

![Thème Elegant.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-57c3ebf0.jpg)

Die Farben lassen sich nicht direkt in der Konfiguration von Elegant ändern: Kunden von [Piwigo Cloud](https://de.piwigo.org/piwigo-bekommen) müssen sich an den Support wenden, um eine Änderung oder Zugriff auf das Stylesheet von Piwigo zu erhalten.

Elegant bietet einige Konfigurationsoptionen:

- Seitenleiste mit dem Menü ein- oder ausblenden
- Seitenleiste mit der Fotobeschreibung ein- oder ausblenden
- Kommentarbereich ein- oder ausblenden

## Wie teste ich ein Erscheinungsbild, ohne dass es alle sehen?

Wie wir gesehen haben, können in Piwigo mehrere Erscheinungsbilder aktiviert sein, aber allen Benutzern wird nur das Standard-Erscheinungsbild angezeigt.

Wenn Sie ein Erscheinungsbild testen möchten, ohne es für alle zugänglich zu machen, ist das also ganz einfach.

Aktivieren Sie es einfach im Administrationsbereich im Menü Konfiguration > Erscheinungsbilder.

Öffnen Sie dann Ihre Galerie und das Menü „Anpassen“. In diesem Menü bearbeiten Sie Ihre persönlichen Einstellungen. Dort können Sie das Erscheinungsbild wechseln: Diese Änderung ist nur für Sie sichtbar.

![Choix de thèmes.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-c33f8f0d.jpg)

## Erscheinungsbilder einfach wechseln mit Theme Switch

Wenn Sie das Wechseln der Erscheinungsbilder in Ihrer Galerie noch einfacher machen möchten, können Sie das Plugin Theme Switch aktivieren.

Nach der Aktivierung fügt dieses Plugin Ihrer Galerie ein Pinsel-Symbol hinzu, mit dem Sie das Erscheinungsbild mit einem Klick wechseln.

!!! warning "Achtung: Dieses Symbol ist für alle Besucher sichtbar, nicht nur für Administratoren."

![Theme Switch.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-1b953541.jpg)

## Erscheinungsbilder einfach wechseln mit Admin Tools

Das Plugin Admin Tools bietet viele Möglichkeiten, Aktionen des Administrationsbereichs direkt aus Ihrer Galerie heraus aufzurufen.

Unter anderem können Sie damit einfach das Erscheinungsbild wechseln.

Wenn dieses Plugin aktiviert ist, erscheint ein zusätzliches Menü, sobald sich ein Administrator in der Piwigo-Galerie anmeldet. Mit der Schaltfläche „Optionen“ oben rechts wechseln Sie das aktive Erscheinungsbild mit einem Klick. Das ist nur für Sie sichtbar.

![Admin Tools.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-110f8230.jpg)

!!! info "Info:"
    Mit diesem Plugin können Sie ausserdem mit einem Klick die Sprache wechseln oder Ihre Galerie aus der Sicht eines beliebigen anderen Benutzers ansehen: Zum Testen ist es daher sehr nützlich.

[Mehr über das Plugin Admin Tools erfahren](../piwigo-administrieren/plugins-fuer-administratoren.md)
