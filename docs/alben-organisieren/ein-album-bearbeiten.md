---
title: Ein Album bearbeiten - Piwigo-Dokumentation
description: Wie bearbeite ich ein Album in Piwigo? Welche Informationen und Eigenschaften gibt es? Wie verwalte ich die Zugriffsrechte eines Albums?
---

# Ein Album bearbeiten

## Ein Album im Administrationsbereich bearbeiten

Um ein Album im Administrationsbereich von Piwigo zu bearbeiten, öffnen Sie über das Menü Alben > Verwaltung die Albenliste.

Klicken Sie in der Albenliste auf das Symbol „Album bearbeiten“. Es öffnet sich eine neue Seite: die Bearbeitungsseite des Albums.

![Modifier album.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-5ee23170.jpg)

## Ein Album in Ihrer Galerie bearbeiten

Als Administrator können Sie ein Album auch direkt in Ihrer Galerie bearbeiten.

Öffnen Sie dazu die Seite des Albums und klicken Sie auf das Symbol „Album bearbeiten“.

Je nach Erscheinungsbild sieht dieses Symbol wie ein Schraubenschlüssel oder auch wie ein Stift aus. Sie werden dann zur Bearbeitungsseite des Albums im Administrationsbereich weitergeleitet.

## Die Eigenschaften eines Albums ansehen und bearbeiten

Die Bearbeitungsseite eines Albums bietet Ihnen zahlreiche Möglichkeiten.

!!! abstract "Die folgenden Screenshots zeigen die neue Version der Album-Bearbeitung, die ab Piwigo 14 verfügbar ist"

Sehen wir uns zuerst den ersten Tab „Eigenschaften“ an.

![Edition album.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-e958fd3f.jpg)

### Informationen zum Album ansehen

Auf dieser Seite sehen Sie Informationen zu Ihrem Album.

In der Kopfzeile finden Sie den Namen des Albums, links seine Position im Baum und rechts die ID des Albums (eindeutige Kennung).

Darunter sehen Sie Informationen zum Album: Erstellungsdatum, Datum der letzten Änderung, Anzahl der Fotos und Anzahl der Unteralben.

### Die Eigenschaften des Albums bearbeiten

Im Tab „Eigenschaften“ können Sie verschiedene Angaben zu Ihrem Album ändern.

- Den Namen Ihres Albums ändern
- Die Beschreibung Ihres Albums ändern

Wenn Sie Ihrem Album eine Beschreibung hinzufügen, erscheint sie in Ihrer Galerie über den Fotos des Albums, wie im folgenden Beispiel.

![Description album.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-5dc7059e.jpg)

- Ein übergeordnetes Album für Ihr Album festlegen oder ändern

So können Sie ein Album in ein anderes Album verschieben und es damit zu einem Unteralbum machen. Umgekehrt können Sie ein Album auch auf die oberste Ebene Ihrer Galerie verschieben.

- Das Vorschaubild des Albums ändern (Album-Vorschaubild)

Wenn Sie ein Album im Administrationsbereich bearbeiten, können Sie das Vorschaubild ändern, das in Ihrer Galerie für das Album angezeigt wird. Fahren Sie dazu mit der Maus über das Bild und klicken Sie auf „Vorschaubild ändern“. Piwigo geht dann die Fotos in diesem Album durch, bis Sie das passende gefunden haben.

Wenn ein bestimmtes Foto Ihr Album repräsentieren soll, bearbeiten Sie dieses Foto im Administrationsbereich und wählen Sie im Feld „Album-Vorschaubild“ das Album aus, für das es stehen soll. [Mehr erfahren](../fotos-importieren-und-verwalten/eigenschaften-und-metadaten-von-fotos.md)

Sie können auch in Ihrer Galerie ein Foto auswählen und auf der Fotoseite auf das Symbol „Als Album-Vorschaubild festlegen“ klicken.

![image.png](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-a52d2e09.png)

### Kommentare erlauben oder sperren

Unten auf der Bearbeitungsseite des Albums können Sie Kommentare für die Fotos in diesem Album erlauben oder sperren.

Um Kommentare in Unteralben zu verwalten, klicken Sie oben rechts auf das Symbol mit den 3 Punkten.

![Commentaires sous albums.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-15baa234.jpg)

[Mehr über Kommentare erfahren](../kommentare-und-bewertungen/kommentare-verwalten.md)

### Weitere Aktionen für das Album

Über die Werkzeugleiste rechts haben Sie Zugriff auf mehrere Optionen.

![Gérer photos album.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-e301da89.jpg)

- Albumfotos verwalten: Mit diesem Symbol bearbeiten Sie die Fotos Ihres Albums gesammelt. [Mehr über die Stapelverarbeitung erfahren](../fotos-importieren-und-verwalten/stapelverarbeitung.md)
- Fotos hinzufügen: Mit diesem Symbol fügen Sie neue Dateien zu Ihrem Album hinzu
- Unteralben verwalten: Dieses Symbol führt Sie zur Albenliste, wenn Sie die Unteralben in Ihrem Album bearbeiten möchten
- Album löschen: Mit diesem Symbol löschen Sie nach Wunsch das Album samt Inhalt oder nur das Album (die enthaltenen Fotos gelten dann in Piwigo als „verwaist“).

Um Ihr Album direkt in der Galerie zu öffnen, klicken Sie schliesslich unten rechts auf die Schaltfläche „In Galerie öffnen“.

### Ein Album sperren

Unten auf der Bearbeitungsseite des Albums können Sie ein Album sperren.

!!! info "Info:"
    Ein gesperrtes Album ist in der Galerie nicht zugänglich, ausser für Administratoren. Meist wird der Status „gesperrt“ verwendet, wenn ein Album noch nicht bereit ist, in der Galerie veröffentlicht zu werden, weil ein Administrator daran arbeitet (Vorbereitung vor der Veröffentlichung, Wartung…). Es handelt sich also um einen vorübergehenden „Arbeitsstatus“.

Sie können auch eine Liste von Alben über das Menü Alben > Eigenschaften > Sperren sperren oder entsperren.

## Die Reihenfolge der Fotos in einem Album ändern

Wenn Sie ein Album bearbeiten, können Sie im zweiten Tab „Foto-Sortierreihenfolge“ festlegen, in welcher Reihenfolge die Fotos in Ihrem Album angezeigt werden.

!!! info "Info:"
    Standardmässig sortiert Piwigo Fotos so: nach Upload-Datum (von neu nach alt), DANN nach Dateiname (von A bis Z), DANN nach ID (von klein nach gross). Sie können diese Einstellung in den Konfigurationsoptionen von Piwigo ändern. [Mehr erfahren](../ihre-galerie-anpassen/anpassungsoptionen-fuer-ihre-galerie.md)

### Die Reihenfolge der Fotos manuell ändern

Im ersten Bereich „Manuelle Sortierung“ können Sie die Reihenfolge der Fotos per Drag-and-drop ganz nach Wunsch ändern. Klicken Sie auf ein Foto und halten Sie die Maustaste gedrückt: Wenn Sie die Maus bewegen, können Sie das Foto an jede beliebige Stelle ziehen. Lassen Sie die Maustaste los, sobald das Foto an der richtigen Stelle ist.

![Ordre des photos.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-31b42ab6.jpg)

### Die Reihenfolge der Fotos automatisch ändern

Im zweiten Bereich „Sortierreihenfolge“ können Sie die Sortierreihenfolge der Fotos automatisch festlegen.

![Ordre de tri.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-e2301eb2.jpg)

Sie haben 3 Möglichkeiten:

- Die Standard-Sortierreihenfolge verwenden: Diese Sortierreihenfolge gilt, solange nichts geändert wurde. In diesem Fall werden die Fotos nach Datum und Uhrzeit ihres Uploads in Piwigo angezeigt.
- Manuelle Sortierung: Wenn Sie die Reihenfolge der Fotos in Ihrem Album bereits manuell geändert haben, ist diese Option automatisch ausgewählt.
- Automatische Sortierung: Mit dieser Option können Sie aus zahlreichen Möglichkeiten eine automatische Sortierreihenfolge wählen, wie das folgende Bild zeigt.
    
    ![Liste ordres.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-2e36ecbd.jpg)
    
    Bei Bedarf können Sie mehrere Optionen kombinieren, zum Beispiel: Fotos nach Upload-Datum sortieren (von alt nach neu), DANN nach Dateiname (von A bis Z).
    

![Ordres combinés.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-fc9057f9.jpg)

Vergessen Sie nicht, auf „Einstellungen sichern“ zu klicken, um Ihre Auswahl zu speichern!

Die gewählte Sortierreihenfolge können Sie auch auf die Unteralben anwenden (falls Ihr Album welche hat). Aktivieren Sie dazu das Kontrollkästchen neben der Schaltfläche zum Speichern.

### Reset Manual Order

Sie möchten die Fotos eines Albums nach einer automatischen Sortierreihenfolge ordnen und diese dann noch anpassen? Dafür können Sie das Plugin **Reset Manual Order** aktivieren.

Dieses Plugin fügt die Option „Manuelle Sortierung mit der aktuellen automatischen Sortierung zurücksetzen“ hinzu. Damit wird eine automatische Sortierreihenfolge auf Ihr Album angewendet, die Sie anschliessend manuell ändern können.

## Zugriffsrechte für ein Album bearbeiten

Der dritte Tab der Album-Bearbeitung ist ohne Zweifel der wichtigste: Hier legen Sie fest, wer dieses Album und seinen Inhalt in Ihrer Galerie sehen darf!

![Permissions.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-37a2ed66.jpg)

Alles über die Verwaltung von Zugriffsrechten für Alben erfahren Sie im folgenden Artikel:

[Zugriffsrechte und Sichtbarkeit von Alben](zugriffsrechte-und-sichtbarkeit-von-alben.md)

## Eine Benachrichtigung zu einem Album senden

Im Tab „Benachrichtigungen“ können Sie eine E-Mail mit einem Link zum Album an einen oder mehrere Benutzer oder sogar an alle Benutzer einer Gruppe senden.

![Notif album.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-6dafd56c.jpg)

Die betreffenden Personen erhalten eine E-Mail mit einem Link zum Album und Ihrer Nachricht.

![Mail album.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-f7bfa0ea.jpg)

!!! warning "Achtung:"
    Bevor Sie eine Benachrichtigung senden, vergewissern Sie sich im Tab „Zugriffsrechte“, dass die Benutzer Zugriff auf dieses Album haben.
