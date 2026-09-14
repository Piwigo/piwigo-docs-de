# Manuelles Update

Dieses Verfahren funktioniert mit jeder Version ab 1.4. Bei einer älteren Version bitten Sie im Forum um Hilfe.

!!! warning "Prüfen Sie die neuen Voraussetzungen"
    Prüfen Sie unbedingt die aktuellen [Voraussetzungen](../installationsanleitungen/voraussetzungen.md) von Piwigo. Wenn insbesondere Ihre **PHP**- / **MySQL**-Konfiguration NICHT ausreicht, fahren Sie nicht fort, da die Aktualisierung sonst fehlschlägt.

## Schritt 1 - Paket vorbereiten

- [Laden Sie das Archiv der neuesten Piwigo-Version herunter](https://de.piwigo.org/piwigo-bekommen)
- Entpacken Sie auf Ihrem Computer das Verzeichnis `piwigo`.
- Löschen Sie das Standardverzeichnis `piwigo/local`.

## Schritt 2 - Datenbank vorbereiten (empfohlen)

Sichern Sie Ihre aktuellen Tabellen.

Wenn Sie eine Version ab der Reihe PhpWebGallery 1.7 verwenden, können Sie das Plugin DB Backup nutzen. Benutzer früherer Versionen müssen ihre Tabellen auf andere Weise sichern, zum Beispiel mit phpMyAdmin.

<figure markdown="span">
    ![](https://ressources.piwigo.com/i?/uploads/c/v/7/cv7jpz6hf8//2026/06/29/20260629172445-b7bbee28-me.webp)
    <figcaption>Empfohlene Optionen in PhpMyAdmin.</figcaption>
</figure>

!!! info
    Unser Rat: Deaktivieren Sie „Extended inserts“ oder verringern Sie „Maximal length of created queries“.

Prüfen Sie auf jeden Fall, ob das Backup vollständig ist und erfolgreich abgeschlossen wurde (das Ergebnis wird aufgrund von Serverbeschränkungen manchmal abgeschnitten).

## Schritt 3 - Dateien auf dem Server vorbereiten

!!! info "Wenn Sie Piwigo 2.1 oder höher verwenden, überspringen Sie diesen Schritt."

Sichern Sie nur Ihre angepassten Dateien oder alle Dateien.

- Laden Sie das Erweiterungswerkzeug `Prepare 2.1 Upgrade` herunter
- entpacken Sie das Skript `prep21up.php` und übertragen Sie es in das Stammverzeichnis Ihrer Piwigo-Installation
- öffnen Sie `prep21up.php` in Ihrem Webbrowser `http://exemple.com/photos/prep21up.php`, und Sie erhalten ein Archiv `upgrade21.zip`
Entpacken Sie auf Ihrem Computer das Verzeichnis `local` aus `upgrade21.zip` in das Verzeichnis `piwigo` (das Sie in [Schritt 1](#schritt-1-paket-vorbereiten) entpackt haben).

## Schritt 4 - Galerie vorbereiten

**Galerie sperren**

Bei Piwigo 2.3 oder älter: Konfiguration > Allgemein > Zugriff auf die Galerie sperren. Bei Piwigo 2.4+: Werkzeuge > Wartung.

Ab jetzt sollten Benutzer ohne Administratorrechte bei jeder Galerie-Version etwa folgende Meldung sehen: „Die Galerie ist aus Wartungsgründen gesperrt. Bitte besuchen Sie uns später wieder.“

<figure markdown="span">
    ![](https://ressources.piwigo.com/i?/uploads/c/v/7/cv7jpz6hf8//2026/06/29/20260629172446-132e2d1c-me.webp)
    <figcaption>Galerie sperren</figcaption>
</figure>

## Schritt 5 - Aufräumen

Löschen Sie alle Dateien Ihrer aktuellen Piwigo-Installation.

!!! Danger "mit folgenden Ausnahmen – diese Verzeichnisse NICHT löschen:"
    - Galleries
    - Upload
    - Plugins
    - Themes
    - Template-extension
    - Local
    - _data

## Schritt 6 - Hochladen per FTP

Laden Sie mit Ihrem gewohnten FTP-Client die neue Version, also den Inhalt des Verzeichnisses `piwigo` (das Sie in [Schritt 1](#schritt-1-paket-vorbereiten) entpackt und in [Schritt 3](#schritt-3-dateien-auf-dem-server-vorbereiten) aktualisiert haben), in das bisherige Piwigo-Installationsverzeichnis hoch.

Prüfen Sie, ob bei Ihrem FTP-Client keine Fehler aufgetreten sind.

## Schritt 7 - Datenbank aktualisieren

**Aktualisierung starten**

Öffnen Sie in Ihrem Webbrowser das Skript `upgrade.php` und folgen Sie der Anleitung: `http://example.com/photos/upgrade.php`

<figure markdown="span">
    ![](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8//2026/06/29/20260629172446-2bb8d9d9.webp)
    <figcaption>Startseite der Aktualisierung.</figcaption>
</figure>

Damit kein anderer Besucher die Aktualisierung durchführt, werden Sie gebeten, sich anzumelden.

---

Ihre bisherige Version wird erkannt, und Sie erhalten eine Zusammenfassung der Aktualisierungsschritte.  

Plugins, die vor der Aktualisierung aktiv waren, werden deaktiviert, da sie mit der neuen Version möglicherweise nicht funktionieren und eine eigene Aktualisierung benötigen.

<figure markdown="span">
    ![](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8//2026/06/29/20260629172446-82c85f1c.webp)
    <figcaption>Übersichtsseite der Aktualisierung.</figcaption>
</figure>

Plugins, die vor der Aktualisierung aktiv waren, werden deaktiviert, da sie mit der neuen Version möglicherweise nicht funktionieren und eine eigene Aktualisierung benötigen.

## Schritt 8 - Ergebnis der Aktualisierung prüfen

Ihre ersten Kontrollen können etwas Zeit in Anspruch nehmen, da Sie noch nicht alle Änderungen kennen.

Sie sehen eine Liste all Ihrer bisherigen Plugins. Einige davon wurden vollständig in den Kern integriert (z. B. Plugins Manager), andere werden jetzt separat verteilt (z. B. LocalFiles Editor). Jedes deaktivierte Plugin wurde aber aus gutem Grund deaktiviert.

Suchen Sie zuerst nach einer Aktualisierung; die Registerkarten der Plugin-Seite können Ihnen dabei helfen.

Lassen Sie bei den Erscheinungsbildern eine Administrationsseite in Ihrem Browser geöffnet, falls Sie einen Ihrer Tests rückgängig machen müssen.

Denken Sie daran, dass Ihre Mitglieder oder Besucher ein bestimmtes Erscheinungsbild gewählt haben können, das nicht mit Ihrer neuen Version kompatibel ist. Setzen Sie ihr Erscheinungsbild daher am besten auf der Seite zur Benutzerverwaltung im Administrationsbereich zurück.

## Schritt 9 - Galerie entsperren

Sobald Sie mit der neuen Version vertraut sind, vergessen Sie nicht, Ihre Galerie zu entsperren, damit Besucher wieder Zugriff haben.

## Schritt 10 - Aufräumen nach der Aktualisierung

**Nichts**

Nach einer Aktualisierung muss nichts gelöscht werden. Auch `upgrade.php` selbst darf nicht gelöscht werden. Denken Sie daran, dass die Meldung „Keine Aktualisierung erforderlich“ und die Anmeldung Ihre Galerie schützen.
