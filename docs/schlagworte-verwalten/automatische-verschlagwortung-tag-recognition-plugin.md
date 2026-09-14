---
title: "Tag Recognition: Fotos automatisch mit KI verschlagworten"
description: Sie haben sehr viele Fotos und möchten sie schnell und automatisch verschlagworten? Mit dem Plugin Tag Recognition ist das möglich.
---

# Tag Recognition: Fotos automatisch mit KI verschlagworten

Sie haben sehr viele Fotos und möchten sie schnell und automatisch verschlagworten? Mit dem Plugin Tag Recognition ist das möglich.

!!! info "Wenn Sie Kunde von Piwigo Cloud sind, ist dieses Plugin erst ab dem Enterprise-Paket verfügbar."

## Die API auswählen

Nachdem Sie das Plugin Tag Recognition installiert und aktiviert haben, öffnen Sie die Einstellungen des Plugins.

Wählen Sie zuerst aus, mit welcher Lösung die Schlagworte automatisch erstellt werden sollen.

Das Plugin nutzt nämlich eine Bilderkennungs-API eines Drittanbieters, die die Fotos analysiert und die Schlagworte erzeugt. Sie haben die Wahl zwischen zwei Lösungen:

- [Imagga](https://imagga.com/)
- [Microsoft Azure AI Vision](https://azure.microsoft.com/en-us/products/ai-services/ai-vision/)

Die Wahl hängt von Ihren Vorlieben und von der Anzahl der zu analysierenden Fotos ab. Beide Lösungen bieten ein kostenloses Paket und ab einer bestimmten Menge kostenpflichtige Angebote. Alle Details finden Sie auf den Websites der Anbieter.

!!! info "Da dieses Plugin eine externe API nutzt, können wir nicht garantieren, dass Ihre Daten nicht verwendet oder verkauft werden. Wir empfehlen Ihnen, die Datenschutzrichtlinien jeder externen API zu prüfen, die Sie mit diesem Plugin verwenden."

## Tag Recognition mit Imagga einrichten

Wenn Sie sich für Imagga entscheiden, gehen Sie wie folgt vor.

Erstellen Sie zuerst ein Konto auf der Website [https://imagga.com/](https://imagga.com/).

Im Dashboard Ihres Kontos finden Sie die beiden Angaben, die Sie benötigen: Ihren API-Schlüssel und Ihren geheimen Schlüssel (*API Secret*).

![Imagga.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-f988b6ea.jpg)

Kopieren Sie diese beiden Schlüssel und fügen Sie sie in der Konfiguration des Plugins Tag Recognition ein. Klicken Sie auf „Einstellungen sichern“.

![Reconnaissance des tags.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-2f92ec50.jpg)

[Dokumentation von Imagga](https://docs.imagga.com/)

## Tag Recognition mit Azure AI Vision einrichten

Wenn Sie sich für Azure AI Vision entscheiden, gehen Sie wie folgt vor.

Erstellen Sie zuerst ein Konto auf der Website [https://azure.microsoft.com/en-us/free/](https://azure.microsoft.com/en-us/free/).

Wenn Sie in Ihrem Konto angemeldet sind, öffnen Sie den Dienst Computer Vision. Wenn Sie kein Abonnement haben, wählen Sie zum Einstieg den Testzeitraum. Anschliessend erhalten Sie Ihren API-Endpunkt (*API Endpoint*) und Ihren API-Schlüssel (*API Key*), die Sie in der Konfiguration des Plugins Tag Recognition eintragen.

![Untitled](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-3c10df32.png)

[Dokumentation von Azure AI Vision](https://learn.microsoft.com/en-us/azure/ai-services/computer-vision/overview?wt.mc_id=searchAPI_azureportal_inproduct_rmskilling&sessionId=8acf0be16fd54e18a988e52fa4dc2edd)

## Mit Tag Recognition Schlagworte für ein Foto vorschlagen lassen

Sobald das Plugin richtig eingerichtet ist, können Sie damit automatisch Schlagworte erzeugen.

Wählen Sie dazu ein Foto aus, das Sie verschlagworten möchten, und bearbeiten Sie es.

Klicken Sie im Eingabefeld für die Schlagworte dieses Fotos auf das Symbol in Form eines Roboters.

![Tag robot.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-adc3fc23.jpg)

Nun können Sie festlegen, wie viele Schlagworte erzeugt werden sollen und in welcher Sprache.

![Générer des tags.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-3c189468.jpg)

Versuchen wir, für dieses Foto eines Hundes 10 Schlagworte auf Englisch zu erzeugen.

![pauline-loroy-U3aF7hgUSrk-unsplash.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-61bd9029.jpg)

Die API schlägt folgende Schlagworte vor:

![Tags suggérés.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-991aa7b8.jpg)

Klicken Sie auf die Schlagworte, die Ihnen gefallen, und dann auf „Apply tags“: Die Schlagworte werden Ihrem Foto hinzugefügt. Vergessen Sie nicht, auf „Einstellungen sichern“ zu klicken.

## Mit Tag Recognition Schlagworte gesammelt einer Auswahl zuweisen

Wenn es schnell gehen soll, können Sie Schlagworte gesammelt über die [Stapelverarbeitung](../fotos-importieren-und-verwalten/stapelverarbeitung.md) erzeugen.

In der Stapelverarbeitung steht dafür eine neue Aktion zur Verfügung: „Tag Recognition“.

Wählen Sie Ihre Fotos aus und wählen Sie die Aktion „Tag Recognition“. Legen Sie die Anzahl der zu erzeugenden Schlagworte und die Sprache fest.

![Gestion lot générer tag.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-06c13dd0.jpg)

Klicken Sie auf „Aktion anwenden“: Der Vorgang beginnt. Die Fotos werden nacheinander verarbeitet.

![Chargement des tags.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-c58d2705.jpg)

Sobald der Stapel verarbeitet ist, sind die Fotos verschlagwortet! Im Tab „Einzelmodus“ der Stapelverarbeitung können Sie prüfen, ob Ihnen die gewählten Schlagworte gefallen.

![Tags générés en masse.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-e3fc3d90.jpg)
