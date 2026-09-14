---
title: LocalFiles Editor - Piwigo-Dokumentation
description: Wie passen Sie mit dem Plugin LocalFiles Editor die Konfigurationsoptionen von Piwigo an? In diesem Artikel erklären wir alles.
---

# Lokale Konfiguration mit LocalFiles Editor bearbeiten

## Einführung

Bei der lokalen Konfiguration bearbeiten Sie bestimmte Einstellungen Ihrer Piwigo-Galerie, die sich nicht über eine grafische Oberfläche im Administrationsbereich ändern lassen.

Diese Einstellungen sind in einer Konfigurationsdatei gespeichert: `config_default.inc.php`

Diese Datei darf **NIEMALS** bearbeitet werden. Sie können sie jedoch *mit dem Plugin* **LocalFiles Editor** *überschreiben*.

!!! tip "Tipp:"
    Wir raten dringend davon ab, die Dateien von Piwigo direkt per FTP zu bearbeiten. Die Verwendung des Plugins **LocalFiles Editor** hat viele Vorteile, wie Sie sehen werden.

## Plugin LocalFiles Editor aktivieren

Der erste Schritt zur Bearbeitung der lokalen Konfiguration ist die Aktivierung des Plugins LocalFiles Editor.

![Plugin LFE.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-2f3c60d6.jpg)

Klicken Sie nach der Aktivierung des Plugins auf „Konfiguration“.

Sie gelangen dann zum unten abgebildeten Bildschirm mit einer leeren Datei.

![LFE auto hébergement.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-4b38d1fb.jpg)

## Standardkonfiguration

Auf diesem Bildschirm haben Sie Zugriff auf die Standardkonfigurationsdatei, in der alle verfügbaren Konfigurationsoptionen aufgeführt sind. Klicken Sie dazu oben rechts auf den Link *Referenzdatei anzeigen: "config_default.inc.php"*.

Jede Zeile, die mit `$conf` beginnt, steht für eine Option.

Die Optionen sind in logische Abschnitte gruppiert (URLs, Schlagworte, verwandte Alben …).

Über jeder Option erklärt ein Kommentarabschnitt (beginnend mit `//` ) die Funktion der Option.

Nehmen wir als Beispiel die Option `'enable_formats'`: Mit dieser Option aktivieren oder deaktivieren Sie die Verwaltung mehrerer Formate in Ihrer Galerie. Standardmässig ist sie deaktiviert (`false`).

```php
// enable_formats: should Piwigo search for multiple formats?
$conf['enable_formats'] = false;
```

## Lokale Konfiguration bearbeiten

Wie gesagt, sollten Sie die mit Ihrer Piwigo-Galerie gelieferte Konfigurationsdatei nicht bearbeiten.

Mit LocalFiles Editor können Sie die Einstellungen dieser Datei überschreiben, das heisst festlegen, welche Einstellungen gegenüber der Originaldatei geändert werden sollen.

Greifen wir das vorherige Beispiel wieder auf: Angenommen, Sie möchten die Verwaltung [mehrerer Formate](../fotos-importieren-und-verwalten/mehrere-formate.md) aktivieren.

Kopieren Sie einfach den Abschnitt zur Einstellung `'enable_formats'` und fügen Sie ihn im Reiter „Lokale Konfiguration“ von LocalFiles Editor ein. Ersetzen Sie dann den Wert `false` durch `true`, wie im Beispiel unten.

!!! warning "Achtung! Die Datei muss immer mit `<?php` beginnen und mit `?>` enden."

![LFE Code.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-cf33c6f7.jpg)

Speichern Sie die Datei: Die Einstellung wird übernommen und die Verwaltung mehrerer Formate ist aktiviert.

!!! info "Info:"
    Wir empfehlen, auch die Erklärung aus den Kommentaren über der Zeile mit der Einstellung zu kopieren. So können Sie sich die Funktion jeder Einstellung leichter merken.
