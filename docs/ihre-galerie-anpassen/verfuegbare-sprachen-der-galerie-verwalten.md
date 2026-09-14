---
title: Sprachen und Übersetzung - Piwigo-Dokumentation
description: Mit Piwigo können Sie eine mehrsprachige Fotobibliothek erstellen, in der Besucher in der Sprache ihrer Wahl stöbern. In diesem Artikel erklären wir, wie das geht.
---

# Verfügbare Sprachen Ihrer Galerie verwalten

Die Oberfläche von Piwigo ist in über 70 Sprachen verfügbar.

Sie können mit Piwigo also eine mehrsprachige Fotobibliothek erstellen und Besuchern ermöglichen, Ihre Fotobibliothek in der Sprache ihrer Wahl zu durchsuchen.

In diesem Artikel erklären wir, wie das geht.

## Verfügbare Sprachen in Piwigo verwalten

Um die verfügbaren Sprachen Ihrer Piwigo-Galerie zu ändern, öffnen Sie im Administrationsbereich das Menü **Konfiguration > Sprachen**.

Diese Seite zeigt die in Ihrer Piwigo-Galerie aktivierten Sprachen. Hier können Sie neue Sprachen aktivieren und die Standardsprache festlegen.

![Liste langues.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-40c57bcb.jpg)

Wenn Sie Ihr Konto über die Website von Piwigo cloud erstellt haben, ist die Konfiguration wie folgt:

- Die aktivierte Sprache ist Englisch
- Die Standardsprache ist Englisch.

Um eine Sprache zu deaktivieren, klicken Sie einfach auf „Deaktivieren“.

Um eine weitere Sprache zu aktivieren, wählen Sie einfach eine Sprache in der Liste und klicken Sie auf „Aktivieren“.

Um die Standardsprache zu ändern, klicken Sie bei der gewünschten Sprache einfach auf „Standard“.

Wechseln Sie anschliessend zur Galerie.

Mit einem Klick auf „Anpassen“ können Sie die Anzeigesprache ändern: Diese Wahl gilt nur für Sie selbst (es handelt sich um eine Einstellung, die für jeden Benutzer gespeichert wird).

[Mehr über Einstellungen erfahren](../benutzer-verwalten/benutzer-erstellen-und-verwalten.md)

![Options customisation.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-6e2d7d1f.jpg)

Der Sprachwechsel wird sofort übernommen: Er betrifft alle Texte Ihrer Galerie (Menüs, Schaltflächen...). Aber Achtung: Dynamische Inhalte aus der Datenbank (Albumnamen, Fotonamen, Beschreibungen...) werden nicht übersetzt.

![Eine Piwigo-Galerie auf Spanisch.](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-f241a9d8.png)

Eine Piwigo-Galerie auf Spanisch.

## Die Sprache in Ihrer Galerie wechseln

Wenn Sie den Sprachwechsel in Ihrer Galerie einfacher und schneller machen möchten, können Sie das Plugin **Language Switch** verwenden.

Sobald dieses Plugin aktiviert ist, erscheint in Ihrer Galerie eine Flagge, die der aktuellen Sprache entspricht.

Wenn Sie auf diese Flagge klicken, können Sie mit einem Klick auf eine andere Flagge die Sprache wechseln.

![Sprachwechsel mit Language Switch und dem Erscheinungsbild Modus](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-b7adfd03.jpg)

Sprachwechsel mit Language Switch und dem Erscheinungsbild Modus

![Sprachwechsel mit Language Switch und dem Erscheinungsbild Bootstrap Darkroom](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-a348cdfc.jpg)

Sprachwechsel mit Language Switch und dem Erscheinungsbild Bootstrap Darkroom

## Exif View: die Namen der EXIF-Metadaten übersetzen

Wenn Sie die Werte der EXIF-Metadaten in die Sprache der Galerie übersetzen möchten, müssen Sie das Plugin **Exif View** installieren.

## Extended Descriptions: Namen und Beschreibungen von Fotos und Alben übersetzen

Wenn Sie die Namen und Beschreibungen von Fotos oder Alben übersetzen möchten, müssen Sie das Plugin **Extended Descriptions** installieren.

Dieses Plugin fügt Piwigo viele Funktionen hinzu, darunter die Möglichkeit, je nach Sprache des Benutzers einen anderen Titel und eine andere Beschreibung für ein Foto oder ein Album anzuzeigen.

Die Funktionsweise dieses Plugins ist auf seiner Seite „Konfiguration“ beschrieben.

Im Administrationsbereich von Piwigo müssen Sie in jedem Feld, das Sie übersetzen möchten, jeden Wert mit zwei Tags umschliessen, die die Sprache angeben, wie im folgenden Beispiel.

```html
[lang=en]Default description[/lang]
[lang=fr]Description en français[/lang]
[lang=de]Deutsche Beschreibung[/lang]
```

Mit dem Tag „default“ können Sie die Standardsprache angeben, wie im folgenden Beispiel.

Die Standardbeschreibung (oder der Standardname) wird verwendet, wenn für die Sprache des Benutzers keine Beschreibung angegeben ist.

Wenn [lang=default] nicht vorhanden ist, gilt alles, was ausserhalb der Sprach-Tags steht, als Standardbeschreibung.

```html
[lang=default]Default description[/lang]
[lang=fr]Description en français[/lang]

// OR

Default description
[lang=fr]Description en français[/lang]
```

Mit dem Tag „all“ können Sie einen Text festlegen, der unabhängig von der Sprache des Benutzers immer angezeigt wird.

Alles, was zwischen den Tags [lang=all] und [/lang] steht, wird unabhängig von der Sprache des Benutzers übernommen.

Das ist besonders nützlich, um HTML- oder Javascript-Code in eine Beschreibung einzufügen.

```html
[lang=all]<p>[/lang]
  [lang=default]Default description[/lang]
  [lang=fr]Description en français[/lang]
  [lang=de]Deutsche Beschreibung[/lang]
[lang=all]</p>[/lang]
```

Das Plugin Extended Descriptions bietet Ihnen übrigens noch weitere Funktionen, um Ihre Galerie anzupassen.

[Mehr über Extended Descriptions erfahren](plugins-zur-galerie-anpassung.md)
