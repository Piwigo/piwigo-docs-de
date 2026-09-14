---
title: Wartung von Piwigo - Piwigo-Dokumentation
description: Für die „technischen“ Administratoren von Piwigo gibt es ein Menü Wartung, das nur Benutzern mit dem Status Webmaster zugänglich ist.
---

# Wartung Ihrer Piwigo-Galerie

Für die „technischen“ Administratoren von Piwigo steht ein Menü Wartung zur Verfügung. Es ist nur für Benutzer mit dem Status Webmaster zugänglich.

Sie finden es im Administrationsbereich unter Werkzeuge > Wartung.

## Verfügbare Wartungsaktionen in Piwigo

Der erste Reiter „Optionen“ bietet zahlreiche Aktionen zur Verwaltung Ihrer Piwigo-Galerie.

![Page de maintenance.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-e890070e.jpg)

Die im „normalen“ Gebrauch von Piwigo am häufigsten genutzte Aktion ist „Zugriff auf die Galerie sperren“ (siehe nächstes Kapitel). Damit machen Sie die Galerie unzugänglich, zum Beispiel während Sie sie neu organisieren.

Die übrigen Aktionen dienen hauptsächlich dazu, nicht mehr benötigte Daten zu löschen oder die in Piwigo angezeigten Informationen zu aktualisieren.

!!! info "Wozu sind diese Aktionen nötig?"

    Damit Seiten schneller laden, verwendet Piwigo zwischengespeicherte Daten. Statt zum Beispiel bei jedem Seitenaufruf die Anzahl Fotos in jedem Album neu zu zählen, wird diese Information in der Datenbank gespeichert. Theoretisch ist sie immer korrekt, doch gelegentlich kann ein Fehler auftreten, sodass die zwischengespeicherte Information nicht mehr stimmt. In diesem Fall kann es helfen, den Cache zu löschen und neu zu erzeugen.
    
    Ausserdem werden manche Daten mit der Zeit überflüssig. Wenn Sie sie aus der Datenbank löschen, geben Sie Speicherplatz frei.


### Aktionen für die Galerie

Hier die Aktionen im Bereich „Globale Galerie-Aktionen“.

- **Zugriff auf die Galerie sperren**

Mit dieser Aktion versetzen Sie Ihre Galerie in den „Wartungsmodus“.

Eine gesperrte Galerie ist nur für Administratoren sichtbar. Solange die Galerie gesperrt ist, wird auf allen Seiten des Administrationsbereichs von Piwigo ein Warnhinweis angezeigt.

![Galerie verrouillée.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-826b8c70.jpg)

Die Besucher der Galerie können die Website dagegen nicht mehr aufrufen. Stattdessen wird folgende Meldung angezeigt: *Die Galerie ist aus Wartungsgründen gesperrt. Bitte besuchen Sie uns später wieder.*

- **Alben-Informationen aktualisieren**

Diese Aktion kann nützlich sein, wenn in Ihrer Galerie eine Fehlermeldung erscheint. Sie prüft die in der Datenbank gespeicherten Daten zu den Alben und korrigiert sie bei Bedarf.

- **Fotoinformationen aktualisieren**

Diese Aktion kann nützlich sein, wenn in Ihrer Galerie eine Fehlermeldung erscheint.

Sie prüft die in der Datenbank gespeicherten Daten zu den Fotos und korrigiert sie bei Bedarf.

- **Datenbank reparieren und optimieren**

Diese Aktion kann nützlich sein, wenn in Ihrer Galerie eine Fehlermeldung erscheint.

Sie führt eine Wartung Ihrer Datenbank durch: Optimierung (Freigabe von leeren Bereichen, die früher Daten enthielten) und Reparatur (Prüfung und Reparatur der Tabellenstrukturen). Ausserdem wird die Datenbank dadurch etwas verkleinert.

- **Integrität erneut prüfen**

Normalerweise müssen Sie diese Aktion nicht ausführen.

Sie setzt die Fehlerzähler zurück, die bei Integritätsprüfungen erkannt wurden, einschliesslich der Ergebnisse auf der Startseite des Administrationsbereichs.

### Bereinigungsaktionen

Hier die Aktionen im Bereich „Bereinigungsaktionen“.

- **Benutzer-Zwischenspeicher leeren**

Diese Aktion kann nützlich sein, wenn ein Benutzer in der Galerie Elemente sieht, die er nicht sehen sollte (zum Beispiel, wenn Sie feststellen, dass Zugriffsrechte nicht eingehalten werden). Normalerweise müssen Sie diese Aktion nicht ausführen.

- **Nicht benutzte Schlagworte entfernen**

Mit dieser Aktion löschen Sie alle Schlagworte, die keinem Foto zugeordnet sind.

- **History-Einträge löschen**

Diese Aktion löscht den gesamten Verlauf der Besuche. Die Suche im Verlauf (erreichbar über das Menü Werkzeuge > Statistik > Suchen) zeigt danach keine Daten mehr an.

!!! danger "Alle Daten gehen unwiderruflich verloren. Die Grafiken im Reiter Statistik werden jedoch weiterhin angezeigt, ausser Sie löschen auch die History-Zusammenfassung (nächster Absatz)"


- **History-Zusammenfassung löschen**

Diese Aktion löscht die Statistikgrafiken im Menü Werkzeuge > Statistik > Statistik.

!!! warning "Wenn Sie nicht gleichzeitig auch die History-Einträge löschen (vorheriger Absatz), werden die Grafiken aus den Informationen im detaillierten Verlauf neu berechnet"


- **Sitzungen löschen**

Wenn sich Besucher in einer Galerie anmelden, wird eine Sitzung mit einer eindeutigen Kennung erzeugt. Diese wird in einer Tabelle der Datenbank und in einem Cookie gespeichert (das Cookie ist 30 Minuten gültig). Die Sitzungskennung wird für verschiedene Zwecke verwendet, insbesondere für die Statistik. Es kann daher nötig sein, Sitzungen zu löschen, die seit Langem nicht mehr verwendet wurden.

Unter anderem lässt sich so die Grösse der Datenbank verringern.

- **Nicht verwendete Benachrichtigungen löschen**

Der RSS-Benachrichtigungs-Feed wird für jeden Besucher individuell angepasst (neue Elemente, neue Kommentare usw.). Mit dieser Funktion löschen Sie diese „Anpassung“ für Besucher, die den Feed nicht nutzen.

- **Suchhistorie löschen**

Piwigo speichert die Kriterien der Suchen, die Besucher in Ihrer Galerie durchführen. Mit dieser Funktion löschen Sie diesen Verlauf.

Unter anderem lässt sich so die Grösse der Datenbank verringern.

### Cache leeren

Hier die Aktionen im Bereich „Cache leeren“.

**Cache-Grösse berechnen**

Klicken Sie auf „Aktualisieren“, um diese Berechnung neu durchzuführen.

**Kompilierte Vorlagen entfernen**

Verwenden Sie diese Funktion, um die Darstellung der Galerie neu zu erzeugen, wenn sie fehlerhaft ist. Das ist meist nach Änderungen an Vorlagen (Templates) oder nach einem Wechsel des Erscheinungsbilds der Fall.

### Mehrfache Bildgrössen entfernen

Jedes Mal, wenn ein Benutzer eine bestimmte Version eines Fotos in der Galerie anzeigen lässt, wird diese Version gespeichert. Mit der Zeit kann das Speicherplatz in Ihrer Datenbank belegen. Dieser Bereich zeigt den Platz, den diese Versionen belegen, und ermöglicht es Ihnen, sie zu löschen. Sie werden dann bei Bedarf neu erzeugt.

## Server-Umgebung: Informationen zu Ihrer Piwigo-Galerie

Der Reiter „Server-Umgebung“ zeigt Informationen zu Ihrer Piwigo-Galerie.

Für Kunden, die bei Piwigo Cloud gehostet sind, stehen nur folgende Informationen zur Verfügung:

- Aktuelle Piwigo-Version
- Liste der aktivierten Plugins

![image.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-14cd61fc.png)

Bei einem selbst gehosteten Piwigo gibt es zusätzliche Informationen:

- Installationsdatum
- Betriebssystem
- PHP-Version
- MySQL-Version
- Verwendete Grafikbibliothek und deren Version
- Grösse des Cache

Auf dieser Seite können Sie ausserdem prüfen, ob ein Piwigo-Update verfügbar ist.

![image.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-191f586d.png)

## System-Aktivitäten

Im dritten Reiter „System-Aktivitäten“ (eingeführt mit Piwigo-Version 15) sehen Sie einen detaillierten Verlauf mit Zeitstempel für alle folgenden Ereignisse:

- Änderung eines Konfigurationsparameters von Piwigo
- Installation / Aktivierung / Deaktivierung eines Plugins
- Installation / Aktivierung / Deaktivierung eines Erscheinungsbilds
- Update eines Erscheinungsbilds oder Plugins
- Update des Piwigo-Kerns
- Änderung des Standard-Erscheinungsbilds
- Wartungsaktionen

Zu jeder Aktion sehen Sie das betroffene Objekt (Kern, Plugin oder Erscheinungsbild), die Art der Aktion (Konfiguration, Update, Aktivierung …), den Benutzer, der die Aktion ausgelöst hat, Datum und Uhrzeit sowie Details (Version usw.).

![image.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-46f517ca.png)

## Delete Hit/Rate: Aufrufe (Hits) und Bewertungen von Fotos löschen

Wenn Sie die Aufrufe und Bewertungen von Fotos zurücksetzen möchten, können Sie das Plugin **Delete Hit/Rate** installieren.

- Hits: die Aufrufe der Fotos. Sie werden in der Galerie angezeigt, wenn Sie diese Option aktiviert haben. Danach richtet sich auch die Sortierung der Fotos nach Anzahl Aufrufe.
- Rates: die Bewertungen der Fotos. Sie werden angezeigt, wenn Sie auf der Seite Konfiguration > Optionen die Option „Bewertungen von Fotos erlauben“ aktiviert haben.

[Mehr über Bewertungen erfahren](../kommentare-und-bewertungen/bewertungen-verwalten.md)

Sobald das Plugin Delete Hit/Rate aktiviert ist, stehen im Bildschirm Wartung zwei neue Bereinigungsaktionen zur Verfügung:

- Alle Aufrufe der Galerie löschen (alle Besuche löschen)
- Alle Bewertungen der Galerie löschen

![Actions de purge.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-23ad9743.jpg)
