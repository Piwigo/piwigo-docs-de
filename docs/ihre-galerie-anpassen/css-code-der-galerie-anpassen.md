---
title: CSS-Code der Galerie anpassen - Piwigo-Dokumentation
description: Wenn Sie HTML- und CSS-Kenntnisse haben, können Sie das Design Ihres Piwigo-Erscheinungsbilds anpassen.
---

# CSS-Code der Galerie anpassen

Wenn Sie sich mit HTML und CSS auskennen, können Sie das Design Ihres Erscheinungsbilds verändern.

## CSS mit dem Erscheinungsbild Bootstrap Darkroom hinzufügen

Wenn Ihre Galerie das Erscheinungsbild Bootstrap Darkroom verwendet, können Sie in dessen Einstellungen im Feld „Custom CSS“ eigenen CSS-Code hinzufügen.

![CSS Bootstrap Darkroom](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-f6d07700.jpg)

[Mehr über Bootstrap Darkroom erfahren](../erscheinungsbilder/bootstrap-darkroom-erscheinungsbild.md)

## CSS mit LocalFiles Editor hinzufügen

Mit dem Plugin **LocalFiles Editor** bearbeiten Sie Piwigo-Dateien direkt im Administrationsbereich.

!!! warning "Diese Funktion ist nur für erfahrene Benutzer gedacht!"

Für Kunden von Piwigo Cloud erlaubt dieses Plugin nur das Hinzufügen von eigenem CSS-Code.

Wenn Sie Ihre Piwigo-Galerie selbst hosten, können Sie mit diesem Plugin weitere Dateien bearbeiten (lokale Konfiguration, Sprachdateien, persönliches Plugin). [Mehr erfahren](../piwigo-selbst-hosten/lokale-konfiguration-bearbeiten-localfiles-editor.md)

Öffnen Sie nach der Aktivierung des Plugins seine Einstellungen.

Dort finden Sie ein Fenster, in dem Sie die CSS-Dateien der in Ihrer Galerie installierten Erscheinungsbilder laden können. Um das Erscheinungsbild zu wechseln, wählen Sie es im Dropdown-Menü aus und klicken auf „Bearbeiten“.

![CSS mit LocalFiles Editor](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-b0540a3f.jpg)

Wenn Sie eigenen CSS-Code auf diese Weise hinzufügen, stellen Sie sicher, dass er nicht durch den Code von Piwigo „überschrieben“ wird. Das ist daher der beste Weg, selbst wenn Sie (per FTP) Zugriff auf die Piwigo-Dateien haben.

!!! warning "Achtung:"

    Wenn Sie Ihre Piwigo-Galerie selbst hosten, bearbeiten Sie die Installationsdateien nicht direkt! Sonst werden Ihre Änderungen beim nächsten Update überschrieben.
