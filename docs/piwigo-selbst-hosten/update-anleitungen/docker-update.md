

!!! info "Diese Anleitung betrifft nur Benutzer des offiziellen Docker-Images."
    Diese Anleitung gilt nur für das offizielle Piwigo-Image. Wenn Sie einen Container von LinuxServer verwenden, nutzen Sie bitte stattdessen deren Dokumentation.    
     Wenn Sie zum offiziellen Image wechseln möchten, können Sie [dieser Anleitung folgen](https://github.com/Piwigo/piwigo-docker/wiki/Migration-Guide-from-the-LinuxServer).

## Schritt 1 - Nach Updates suchen

Die Versionsnummern des Containers entsprechen immer der Piwigo-Version. Ab 16.3.0 folgt ihnen zusätzlich ein Buchstabe, damit auch containerspezifische Updates möglich sind.

=== "Container-Version 16.3 und höher"

    Sie sollten bereits in der Update-Oberfläche sehen können, ob ein Update verfügbar ist:
    
    <figure markdown="span">
      ![](https://ressources.piwigo.com/i?/uploads/c/v/7/cv7jpz6hf8//2026/06/29/20260629172514-64cac366-la.webp)
      <figcaption>Beispiel einer Update-Liste</figcaption>
    </figure>
    
=== "Container-Version 16.2 und niedriger"

    Öffnen Sie die Tag-Liste auf [dockerhub](https://hub.docker.com/r/piwigo/piwigo/tags) oder auf [GitHub](https://github.com/Piwigo/piwigo-docker/pkgs/container/piwigo) und suchen Sie den gewünschten Tag.

## Schritt 2 - Ein Backup erstellen

Damit das Update ohne Risiko abläuft, sollten Sie sowohl von der Datenbank als auch von den Dateien Ihrer Piwigo-Instanz ein Backup erstellen.
Wechseln Sie in den Ordner, in dem sich Ihre `compose.yaml` befindet.

### Backup Ihrer Datenbank

Mit dem folgenden Befehl können Sie ein Backup Ihrer Datenbank erstellen (ersetzen Sie `piwigo-db-1` durch den Namen Ihres Datenbank-Containers):

```bash
docker exec -it piwigo-db-1 mariadb-dump -u piwigodb_user -p "piwigodb" | tee db_dump.sql 
```

### Backup Ihrer Galerie und Konfigurationsdateien

Um alle in Ihr Piwigo hochgeladenen Bilder/Fotos und Ihre aktuelle Konfiguration zu sichern, kopieren Sie die folgenden Ordner aus dem Ordner `./piwigo-data/piwigo/`: `galleries`, `upload` und `local`.

!!! Warning "Je nach Anzahl Ihrer Fotos können `galleries` und `upload` sehr viel Speicherplatz belegen" 

### Backup Ihrer Dateien `compose.yaml` und `.env`

Benennen Sie Ihre `compose.yaml` um und erstellen Sie eine Kopie Ihrer `.env` (zum Beispiel, indem Sie `.bak` am Ende anhängen).

???+ tip "Mit den folgenden Befehlen können Sie ein Backup mit Zeitstempel erstellen"

    ```bash
    mv compose.yaml "compose.yaml_$(date '+%F-%H-%M-%S').bak" 
    cp .env "env$(date '+%F-%H-%M-%S').bak"
    ```

## Schritt 3 - Die neue Compose-Datei herunterladen und `.env` aktualisieren

- Laden Sie die Version der `compose.yaml` herunter, die dem in [Schritt 1](#schritt-1-nach-updates-suchen) gewählten Tag entspricht.

!!! tip ""

    Mit dem folgenden Befehl können Sie sie abrufen. Ersetzen Sie einfach `<TAG>` durch den gewählten Tag (z. B. `16.4a`).

    ```bash
    PWG_DOCKER_VERSION="<TAG>"; curl -O "https://raw.githubusercontent.com/Piwigo/piwigo-docker/refs/tags/v$PWG_DOCKER_VERSION/compose.yaml" 
    ```
    
- Lesen Sie die Seite im [Github Wiki](https://github.com/Piwigo/piwigo-docker/wiki/Environment-file-updates) und passen Sie Ihre `.env`-Datei entsprechend an.

??? example "Beispiel für ein Update von Version 15.6 auf Version 16.3c"

    `.env` vor dem Update:

    ```
    piwigo_port=8080
    db_user_password=4JKQplDWaePjjwqiuAmcWWrwY3oqxWtxRs2XCEObf1wRdD2boDa6VA804kzQm2kj
    ```
    
    Wir fügen das Feld timezone hinzu, da es mit `15.7.0` eingeführt wurde, sowie die Felder UID/GID, die mit `16.3.0c` eingeführt wurden.

    ```
    piwigo_port=8080
    db_user_password=4JKQplDWaePjjwqiuAmcWWrwY3oqxWtxRs2XCEObf1wRdD2boDa6VA804kzQm2kj
    timezone=Europe/Paris
    PIWIGO_UID=1004
    PIWIGO_GID=1001
    ```

## Schritt 4 - Den Container aktualisieren und neu starten

Laden Sie das Image mit `docker compose pull` herunter und starten Sie Ihre Container mit `docker compose up  -d` neu.  
Mit `docker compose logs` können Sie in den Logs prüfen, ob alles einwandfrei funktioniert.
