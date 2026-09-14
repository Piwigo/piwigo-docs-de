# Voraussetzungen

Piwigo benötigt ein Webhosting. Wenn Sie eine Fotogalerie-Lösung suchen, bei der alles inbegriffen ist (Installation, Hosting, Backups), oder Piwigo einfach ohne Installation ausprobieren möchten, können Sie [ein kostenloses Testkonto bei
Piwigo Cloud eröffnen](https://de.piwigo.com/anmelden).

### Mindestvoraussetzungen

- Ein Webserver wie Nginx oder Apache
- MySQL 5.6+ oder MariaDB 10.1+. MySQL 5.0 funktioniert, wird aber nicht mehr gepflegt.
- PHP 8.2+. Piwigo läuft auch mit PHP 7.4+, diese Versionen haben jedoch das Ende ihres Lebenszyklus erreicht, werden nicht mehr gepflegt und können Ihre Website Sicherheitslücken aussetzen. Siehe [offiziell unterstützte PHP-Versionen.](https://www.php.net/supported-versions.php)
- Eine Grafikbibliothek: ImageMagick wird wegen seiner Leistung und Bildqualität empfohlen, aber auch GD, das oft mit PHP mitgeliefert wird, erfüllt den Zweck.
- Zum Hochladen der Dateien (netinstall oder vollständiges Paket) wird ein FTP-Programm benötigt: Das Piwigo-Team empfiehlt FileZilla, weil es wie Piwigo kostenlos und mit Windows, Mac und Linux kompatibel ist.
- Genügend Speicherplatz für Ihre Bilder: Zusätzlich zu den hochgeladenen Fotos speichert Piwigo die „mehrfachen Grössen“ in einem Cache-Verzeichnis auf Ihrem Server.

### Optionale Voraussetzungen

- `exiftool` wird für das Plugin Write Metadata und alle anderen Plugins benötigt, die mit EXIF/IPTC-Metadaten arbeiten
- `ffmpeg` wird für das Plugin VideoJS benötigt, um Vorschaubilder (Poster) für Videos zu erstellen
