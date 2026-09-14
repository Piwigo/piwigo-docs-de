---
title: Smart Albums - Piwigo-Dokumentation
description: Mit dem Plugin SmartAlbums für Piwigo erstellen Sie intelligente Alben in Ihrer Medienbibliothek, die sich automatisch mit Fotos füllen.
---

# SmartAlbums

Sie können „intelligente“ Alben erstellen, die sich automatisch mit Fotos füllen, die bestimmte Kriterien erfüllen.

Dazu müssen Sie das Plugin **SmartAlbums** installieren.

!!! info "Wenn Sie Kunde von Piwigo Cloud sind, ist dieses Plugin erst ab dem Enterprise-Tarif verfügbar."

Nachdem Sie das Plugin aktiviert haben, öffnen Sie seine Konfigurationsseite.

## Ein SmartAlbum erstellen

Der erste Tab listet die SmartAlbums auf. Hier können Sie auch ein neues erstellen. Ein SmartAlbum können Sie auf der obersten Ebene Ihrer Galerie oder in einem übergeordneten Album anlegen.

![SmartAlbums.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-4c6e0d44.jpg)

Nachdem Sie das SmartAlbum erstellt haben, legen Sie die Kriterien für seinen Inhalt fest.

Wählen Sie dazu einen Filter aus den verfügbaren Kriterien: Schlagworte, Datum, Album, Name, Abmessungen, Autor, Anzahl der Aufrufe usw.

Als Beispiel erstellen wir ein Album mit allen Fotos, die das Schlagwort „Hund“ haben. Ein Klick auf die Schaltfläche „Count“ zeigt Ihnen, wie viele Fotos betroffen sind.

![SmartAlbum chien.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-009a18c7.jpg)

Sie können mehrere Filter kombinieren und wählen:

- ob die Fotos alle Filter erfüllen müssen, um in das SmartAlbum aufgenommen zu werden,
- oder ob sie mindestens einen Filter erfüllen müssen.

Wenn Sie Ihre Filter festgelegt haben, klicken Sie auf „Speichern“, um Ihr SmartAlbum zu sichern.

## SmartAlbums verwalten

Die so erstellten Alben erscheinen wie alle anderen Alben in der Albenliste. Die Filter können Sie ändern, indem Sie das Album bearbeiten und den Tab „SmartAlbum“ öffnen.

![Modifier album chien.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-80922515.jpg)

Kehren wir zur Konfiguration des Plugins SmartAlbums zurück.

Die erstellten SmartAlbums sehen Sie in der Liste.

![SmartAlbum éclair.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-713522c7.jpg)

Sie können die Fotos in den SmartAlbums jederzeit neu generieren, entweder für alle Alben gleichzeitig oder für einzelne Alben. Durch das Neugenerieren aktualisieren Sie den Inhalt eines SmartAlbums.

## Konfiguration von SmartAlbums

Im Tab „Konfiguration“ können Sie einige Einstellungen vornehmen.

![SmartAlbum configuration.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-6cde2b5a.jpg)

- **Aktualisierungshäufigkeit der SmartAlbums**: SmartAlbums werden nicht in Echtzeit aktualisiert. Neu importierte Fotos landen nicht sofort in einem SmartAlbum, es sei denn, Sie erzwingen die Aktualisierung mit der Funktion zum Neugenerieren. Standardmässig werden SmartAlbums alle 3 Tage aktualisiert. Sie können diese Einstellung aber anpassen.
- **Alben nach dem Import einer Datei aktualisieren**: Wählen Sie diese Option, wenn SmartAlbums nach jedem neuen Upload automatisch neu generiert werden sollen. Aber Vorsicht: Das kann Ihre Galerie verlangsamen, besonders bei vielen Inhalten.
- **SmartAlbums von der Verwaltung der Zugriffsrechte ausnehmen**: In diesem Fall gelten SmartAlbums für alle als privat. Ein Benutzer sieht ihren Inhalt nur, wenn er in einem anderen Album verfügbar ist, auf das er Zugriff hat.
