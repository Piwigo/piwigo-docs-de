---
title: Benutzerstatus - Piwigo-Dokumentation
description: Administrator, Benutzer, Webmaster… Welche Benutzerstatus gibt es in Piwigo und wofür sind sie da?
---

# Benutzerstatus

Um die Benutzerverwaltung in Piwigo zu verstehen, sollten Sie zuerst wissen, wie die **Status** funktionieren.

In Piwigo gibt es 5 Status mit unterschiedlichen Rechten. Ein Benutzer hat immer genau einen dieser 5 Status.

Hier ist die Liste der Status.

## 1- Administrator

Ein Administrator hat Zugriff auf alle Daten in Piwigo und vor allem auf den Administrationsbereich:

- Alben hinzufügen, bearbeiten und löschen,
- Fotos hinzufügen, bearbeiten und löschen,
- Benutzer hinzufügen, bearbeiten und löschen,
- Schlagworte verwalten,
- Statistik und Verlauf der Aktionen in der Galerie ansehen,
- Kommentare verwalten.

Keinen Zugriff hat er dagegen auf die Konfiguration des Erscheinungsbilds der Galerie und auf das Hinzufügen von Plugins.

In den meisten Organisationen sind die Administratoren die Verantwortlichen der Fotothek: Dokumentare, Kommunikationsverantwortliche, Fotografen…

!!! info "Info:"
    Ein Administrator hat im Administrationsbereich Zugriff auf alle Alben und alle Fotos. Sobald er in der Web-Galerie angemeldet ist, gelten jedoch die Zugriffsrechte: Er sieht nur öffentliche Alben oder private Alben, auf die er Zugriff hat.

## 2- Benutzer

Ein Benutzer kann sich in Ihrer Piwigo-Galerie anmelden, aber nicht im Administrationsbereich. Wenn Sie einen Benutzer erstellen oder sich ein Benutzer selbst registriert, hat er standardmässig den Status „Benutzer“.

Ein Benutzer kann die Dateien Ihrer Fotothek ansehen und herunterladen, für die er berechtigt ist. Er kann aber keine Fotos zu Piwigo hinzufügen (ausser mit dem Plugin [Community](mitwirkende-community-plugin.md)).

In einer Organisation hat meist die Mehrheit der Benutzer diesen Status: Es sind die Personen, die sich in der Fotothek anmelden, um die benötigten Dateien zu suchen und herunterzuladen.

## 3- Webmaster

Standardmässig hat der erste Benutzer, der beim Erstellen eines Piwigo-Kontos oder bei der Installation von Piwigo angelegt wird (Hauptbenutzer), den Status „Webmaster“.

Webmaster haben dieselben Rechte wie Administratoren und noch weitere: Plugins aktivieren oder deaktivieren, das Erscheinungsbild wechseln, auf die Konfigurationsoptionen der Galerie zugreifen…

## 4- Generisch

Dieser Status ist nützlich, wenn sich mehrere Personen dasselbe Benutzerkonto teilen.

Generische Profile haben wie Benutzer Zugriff auf Ihre Galerie, aber nicht auf den Administrationsbereich. Dazu kommen einige Besonderheiten (sie können zum Beispiel weder das Passwort noch die Anzeigesprache ändern).

## 5- Gast (deaktiviert)

Benutzer mit diesem Status können sich nicht bei Piwigo anmelden.  

Dieser Status ist nützlich, um das Konto eines Benutzers zu deaktivieren, ohne seinen Verlauf zu löschen.

!!! warning "Nicht zu verwechseln mit dem „Gastkonto“ oder „Gast“, dem allgemeinen Namen für das Profil anonymer Besucher (die nicht in der Galerie angemeldet sind): siehe unten"


## Sonderfall: der Benutzer „Gast“

Der Benutzer „Gast“ ist in Piwigo ein „Phantom“-Benutzer. Er steht für alle Personen, die Ihre Galerie besuchen, ohne angemeldet zu sein.

Im Administrationsbereich legen Sie fest, welche Zugriffsrechte und Einstellungen für diese Besucher gelten. Sie werden standardmässig auch auf alle danach erstellten Benutzer angewendet: Es sind also die „Standardeinstellungen“ von Piwigo.

Wie Sie das Konto „Gast“ bearbeiten, erfahren Sie [in diesem Artikel](benutzer-erstellen-und-verwalten.md).

## Status „Mitwirkender“ (Community-Plugin)

In unseren [Tarifen](https://de.piwigo.com/preise) ist vom Status „Mitwirkender“ die Rede.

Dieser Status ist im engeren Sinn kein Benutzertyp: Gemeint sind Benutzer ohne Administratorrechte, die Dateien in Piwigo importieren dürfen, wenn das Community-Plugin aktiviert ist.

Mehr dazu erfahren Sie in diesem Artikel: [Mitwirkende (Community-Plugin)](mitwirkende-community-plugin.md)
