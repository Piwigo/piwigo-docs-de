---
description: Wie installieren Sie ein Plugin in Piwigo? Wozu dient es? Alle unsere Erklärungen in diesem Artikel.
title: Plugins in Piwigo - Piwigo-Dokumentation
---

# Plugins in Piwigo: Vorstellung

Wenn Sie Piwigo bereits verwenden und diese Dokumentation schon gelesen haben, wissen Sie sicher, dass Plugins ein wesentlicher Bestandteil von Piwigo sind.

Trotzdem halten wir es für sinnvoll, das Thema in diesem Artikel noch einmal aufzugreifen.

## Was ist ein Plugin für Piwigo?

Ein Plugin ist eine Erweiterung, die Funktionen zu Piwigo hinzufügt oder die Grundfunktionen verändert.

Wenn Sie Piwigo zum ersten Mal installieren, haben Sie Zugriff auf das Kernsystem von Piwigo, also die technische und funktionale Grundlage, auf der die gesamte Software aufbaut:

- den Administrationsbereich von Piwigo
- die Galerie mit dem Standard-Erscheinungsbild Modus

Standardmässig sind bereits einige Plugins in Ihrem Piwigo installiert. Welche das sind, hängt davon ab, ob Sie Ihre Galerie selbst hosten oder ein Konto bei Piwigo cloud haben.

- Selbst gehostete Galerien
    
    Wenn Sie die neueste Version von Piwigo in Ihrer Umgebung installieren, werden die folgenden Plugins standardmässig installiert, aber nicht aktiviert:
    
    - Admin Tools (ermöglicht Administratoren, einige Verwaltungsaktionen direkt aus der Galerie auszuführen)
    - Language Switch (ermöglicht es, die Sprache der Galerie einfach zu wechseln)
    - LocalFiles Editor (ermöglicht es, lokale Konfigurationsdateien im Administrationsbereich zu bearbeiten)
    - Take A Tour of Your Piwigo (fügt eine interaktive Führung durch den Administrationsbereich von Piwigo für neue Benutzer hinzu)
- In Piwigo cloud gehostete Galerien
    
    Wenn Sie ein Konto bei Piwigo cloud erstellen, sind die folgenden Plugins standardmässig aktiviert:
    
    - Stop Spammer (ein Plugin gegen Spam, das nicht deaktiviert werden sollte)
    - VideoJS (das Plugin zur Videoverwaltung, das für Kunden von Piwigo cloud seit März 2023 standardmässig aktiviert ist).

**Sie sollten sich aber nicht auf die vorinstallierten Plugins beschränken.** 

Piwigo ist ein modulares Werkzeug, bei dem Sie selbst entscheiden, ob Sie Funktionen hinzufügen möchten: Genau dafür gibt es Plugins.

Wenn Sie WordPress kennen: Das ist genau dasselbe Prinzip. Übrigens werden Sie feststellen, dass nur sehr wenige mit WordPress erstellte Websites ganz ohne Plugins auskommen. Ebenso wäre es wirklich schade, Piwigo zu nutzen, ohne es mit den Plugins zu erweitern, die Ihren Bedürfnissen entsprechen.

## Verwaltung der Plugins: Unterschied zwischen Kunden von Piwigo cloud und selbst gehosteten Galerien

Plugins funktionieren unterschiedlich, je nachdem, ob Sie ein Konto bei Piwigo cloud haben oder eine selbst gehostete Piwigo-Galerie verwenden.

### Sie sind Kunde von Piwigo cloud

Wenn Sie ein Hosting-Paket bei Piwigo cloud gebucht haben, müssen Sie Plugins weder installieren noch aktualisieren.

Sie haben Zugriff auf eine begrenzte Liste von Plugins, die vom gewählten Abonnement abhängt. Diese sind in Ihrer Piwigo-Galerie bereits installiert, und Sie können sie nach Belieben aktivieren oder deaktivieren.

**Liste der Plugins**

Ihre Plugins finden Sie im Administrationsbereich Ihrer Piwigo-Galerie im Menü Plugins.

Auf der Registerkarte Liste sehen Sie die Plugins, die in Ihrer Piwigo-Galerie bereits aktiviert sind, und können unter allen Plugins suchen.

![Liste des plugins.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-97a78cd9.jpg)

Um ein neues Plugin zu aktivieren, klicken Sie einfach auf den Aktivierungsschalter: Das Plugin wird sofort aktiviert. Anschliessend haben Sie Zugriff auf seine Konfiguration.

**Plugins nach Tarif**

Die zweite Registerkarte listet die Plugins auf, die in den einzelnen Tarifen verfügbar sind. Sie können nur Plugins aktivieren, die in Ihrem Tarif enthalten sind.

![Plugins par prix.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-0ab1b3f6.jpg)

Auf dieser Seite sind die Plugins nach Tarif sortiert. An den Symbolen rechts erkennen Sie jederzeit, in welchen Tarifen ein Plugin verfügbar ist.

Wenn Sie ein bestimmtes Plugin suchen, drücken Sie die Tastenkombination Strg+F, um auf der Seite nach dem Namen des Plugins oder nach einer bestimmten Funktion zu suchen.

**Beispiel**: Beim Plugin User Custom Fields ist das erste Symbol ausgegraut, da es erst ab dem Tarif Team verfügbar ist.

![image.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-f455e07d.png)

### Sie verwenden eine selbst gehostete Piwigo-Galerie

Wenn Sie eine Piwigo-Galerie verwenden, die auf Ihrer eigenen Hosting-Plattform und nicht bei Piwigo cloud installiert ist, sieht es etwas anders aus.

Um ein neues Plugin zu verwenden, müssen Sie es zuerst auf Ihrem Server installieren und dann aktivieren.

**Liste der installierten Plugins**

Die in Ihrer Piwigo-Galerie installierten Plugins finden Sie im Administrationsbereich von Piwigo im Menü Plugins.

Auf der Registerkarte Liste sehen Sie die Plugins, die in Ihrer Piwigo-Galerie bereits aktiviert sind, und können unter den installierten, aber deaktivierten Plugins suchen.

![Plugins auto hébergement.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-44e31d6d.jpg)

**Plugins aktualisieren**

Anders als Kunden von Piwigo cloud müssen Sie Ihre Plugins selbst aktualisieren, wenn eine neue Version verfügbar ist. Dafür steht Ihnen die Registerkarte „Auf Aktualisierungen überprüfen“ zur Verfügung. Dort sehen Sie, ob Aktualisierungen verfügbar sind, und können sie installieren.

![Plugins mise à jour.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-efa434ef.jpg)

Wenn für ein Plugin eine Aktualisierung verfügbar ist, können Sie sie sofort installieren, indem Sie auf „Installieren“ klicken. Sie können auch die Plugin-Datei herunterladen oder die Aktualisierung ignorieren.

**Ein Plugin installieren**

Wenn Sie ein Plugin installieren möchten, öffnen Sie die dritte Registerkarte „Ein neues Plugin hinzufügen“.

Auf dieser Seite können Sie alle auf piwigo.org veröffentlichten Plugins durchsuchen, die Sie auch auf [der Seite Extensions der Website](https://de.piwigo.org/ext/) finden.

Sie können per Stichwort nach einem Plugin suchen oder die Plugins filtern (nach Datum, Autor, Schlagwort, Bewertung ...).

![Ajouter un plugin.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-163c6615.jpg)

In dieser Liste finden Sie auch Plugins, die bei Piwigo cloud nicht verfügbar sind. Es handelt sich um Plugins aus der Community, die das Entwicklerteam von Piwigo nicht immer getestet oder freigegeben hat: Deshalb können wir weder garantieren, dass sie korrekt funktionieren, noch dass sie kompatibel sind!

!!! info "Info:"
    Die Plugins, die wir in dieser Dokumentation vorstellen, sind die bei Piwigo Cloud verfügbaren Plugins, die unser Team getestet und freigegeben hat. Das bedeutet aber natürlich nicht, dass die anderen verfügbaren Plugins nicht interessant sind.

Um ein neues Plugin zu installieren, klicken Sie auf Hinzufügen.

![Bouton ajouter plugin.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-7ee02561.jpg)

Sie können ein Plugin direkt nach der Installation aktivieren, indem Sie im Banner auf den Link „Jetzt aktivieren“ klicken.

![Activation plugin special.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-908e71ca.jpg)

Andernfalls finden Sie das Plugin nun auf der Registerkarte Liste in der Kategorie „Deaktiviert“. Klicken Sie einfach auf den Aktivierungsschalter, um es zu aktivieren.

![Plugins désactivés.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-f846d4d2.jpg)

## Konfiguration der Plugins

Meistens haben Plugins eine eigene Konfigurationsseite. Sie erreichen sie über die Liste der in Ihrer Piwigo-Galerie aktivierten Plugins, indem Sie auf die Schaltfläche Konfiguration klicken, sofern diese orange ist.

![Exemple plugin activé.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-7d6d22ae.jpg)

Manchmal enthält diese Konfigurationsseite nur wenige Einstellungen, und Sie werden sie nur sehr selten aufrufen müssen.

In manchen Fällen bietet die Konfiguration eines Plugins jedoch Zugriff auf eine ganze Reihe wichtiger Funktionen dieses Plugins. Dann ist es entscheidend, die Konfigurationsseite aufzurufen. Deshalb zeigen wir in dieser Dokumentation jedes Mal, wenn wir ein Plugin vorstellen, eine Vorschau der Einstellungsseite.

Andererseits bieten manche Plugins keine Einstellungsseite: In diesem Fall ist die Schaltfläche Konfiguration ausgegraut.

Das ist der Fall, wenn das Plugin keine Benutzeroberfläche benötigt, um zu funktionieren, und keine Einstellungen bietet.

Das Plugin **Stop Spammers** zum Beispiel arbeitet selbstständig im Hintergrund und braucht deshalb keine Konfigurationsseite.

![Stop spammers.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-95090bc0.jpg)

Das ist auch der Fall, wenn das Plugin eine Funktion hinzufügt, die über einen anderen Bildschirm in Piwigo erreichbar ist.

Das Plugin **Rotate Image** zum Beispiel fügt auf der Bearbeitungsseite eines Fotos eine Funktion zum Drehen des Bildes hinzu und benötigt deshalb keine Einstellungsseite.

![Rotate Image.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-5d1afa3a.jpg)
## Plugins für alle Bedürfnisse

In der gesamten Dokumentation stellen wir Plugins immer dann vor, wenn es sinnvoll ist.

In den folgenden Artikeln finden Sie eine Auswahl an Plugins für Ihre Bedürfnisse.

- [Ihre Galerie mit Plugins anpassen](../ihre-galerie-anpassen/plugins-zur-galerie-anpassung.md)
- [Die Albumseite mit Plugins anpassen](../ihre-piwigo-galerie-erkunden/alben-in-ihrer-galerie.md)
- [Die Fotoseite mit Plugins anpassen](../ihre-piwigo-galerie-erkunden/die-fotoseite-in-ihrer-galerie.md)
- [Die Verwaltung von Schlagworten mit Plugins anpassen](../ihre-piwigo-galerie-erkunden/schlagworte-in-ihrer-galerie.md)
- [Die Verwaltung von Kommentaren mit Plugins anpassen](../kommentare-und-bewertungen/plugins-zur-kommentarverwaltung.md)
- [Plugins für Administratoren](../piwigo-administrieren/plugins-fuer-administratoren.md)
- [Sammlungen mit dem Plugin User Collections erstellen](../ihre-piwigo-galerie-erkunden/sammlungen-user-collections-plugin.md)
- [Intelligente Alben mit dem Plugin SmartAlbums erstellen](../alben-organisieren/intelligente-alben-smart-albums-plugin.md)
- [Mitwirkende mit dem Plugin Community verwalten](../benutzer-verwalten/mitwirkende-community-plugin.md)
