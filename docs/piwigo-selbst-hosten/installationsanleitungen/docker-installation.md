# Docker-Installation

!!! abstract "Voraussetzungen für die Docker-Installation"
     Diese Anleitung setzt voraus, dass Sie sich per SSH mit Ihrem Server verbinden können und Docker bereits installiert haben. Falls nicht, folgen Sie der [offiziellen Docker-Dokumentation](https://docs.docker.com/engine/install/)

## Schritt 1 - Container installieren

Verbinden Sie sich mit Ihrem Server und erstellen Sie einen Ordner namens `Piwigo`. Laden Sie dann die Datei `compose.yaml` aus dem Repository [Piwigo/piwigo-docker](https://github.com/Piwigo/piwigo-docker) in diesen Ordner herunter.

!!! tip "Mit curl können Sie `compose.yaml` herunterladen, ohne das Terminal zu verlassen:"
    ```
    curl -O "https://raw.githubusercontent.com/Piwigo/piwigo-docker/refs/heads/main/compose.yaml"
    ```

Erstellen Sie eine Datei namens `.env` mit folgendem Inhalt:

=== "Pflichtfelder"

    ```bash
    piwigo_port=8080
    db_user_password=
    timezone=
    ```

=== "Erklärung der Felder"

    ```bash
    piwigo_port= # der von Docker freigegebene Port
    db_user_password= # Passwort der Datenbank
    timezone= # Zeitzone des Containers
    PIWIGO_UID= # die UID des Benutzers, dem der Piwigo-Ordner gehören soll
    PIWIGO_GID= # die GID der Gruppe, der der Piwigo-Ordner gehören soll
    ```
    
=== "Standardwerte"
    ```bash
    piwigo_port=8080
    db_user_password=
    timezone=UTC
    PIWIGO_UID=1000
    PIWIGO_GID=1000
    ```

=== "Beispielkonfiguration"

    ```bash
    piwigo_port=10004
    db_user_password=Nkhcfnfk5GmpnLGIFoIDJqRFPW22C7PlyEUYVaB1lkte5Dn0wOQs3TI4wom1E4A6
    timezone=Europe/Paris
    PIWIGO_UID=1001
    PIWIGO_GID=1004
    ```

!!! tip "Tipp" 
    Mit folgendem Befehl können Sie ein gültiges Passwort erzeugen: 
    ```bash
    printf $(tr -dc '[:alnum:]' </dev/urandom | head -c64)"\n" 
    ```
    
Starten Sie Ihren Container mit `docker compose up -d`.  
Die Logs können Sie mit `docker compose logs` lesen.

## Schritt 2 - Reverse-Proxy konfigurieren

Es wird empfohlen, den Piwigo-Container hinter einem Reverse-Proxy wie NGINX zu betreiben.

!!! info
    Piwigo kann auf einer Domain, einer Subdomain und/oder einem Unterpfad gehostet werden. Unabhängig von Ihrer Wahl wird empfohlen, die Versionsnummer von Piwigo nicht in der URL zu verwenden.

Sie können die folgenden Nginx-Konfigurationsbeispiele verwenden: 

!!! Warning ""

    Wenn Sie piwigo_port in `.env` geändert haben, müssen Sie auch den Abschnitt `proxy_pass` entsprechend anpassen.  
    **Beachten Sie, dass Docker konstruktionsbedingt alle Ihre Firewall-Regeln ignoriert.**

=== "Auf einer Domain oder Subdomain hosten"

    ```nginx
    server {
      listen 80;
      server_name my_domain.tld;
      location / {
        proxy_pass http://127.0.0.1:8080/;
        proxy_set_header Host $host;
        proxy_set_header X-Real-IP $remote_addr;
        proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
        proxy_set_header X-Forwarded-Proto $scheme;
      }
    }
    ```

=== "Auf einem Unterpfad hosten"

    Wenn Sie Piwigo auf einem Unterpfad wie `my_domain.tld/gallery` hosten möchten, müssen Sie diesen an den Container weitergeben, indem Sie `proxy_set_header X-Forwarded-Prefix /gallery` hinzufügen.

    ```nginx
    server {
      listen 80;
      server_name my_domain.tld;
      location /gallery/ {
        proxy_pass http://127.0.0.1:8080/;
        proxy_set_header Host $host;
        proxy_set_header X-Real-IP $remote_addr;
        proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
        proxy_set_header X-Forwarded-Proto $scheme;
        proxy_set_header X-Forwarded-Prefix /gallery;
      }
    }
    ```

## Schritt 3 - Konfiguration

Sobald der Container gestartet und Ihr Reverse-Proxy konfiguriert ist, rufen Sie in einem Webbrowser die Webadresse auf, unter der Sie Piwigo hosten. Piwigo erkennt, dass noch nichts installiert ist, und leitet Sie zur Installationsseite weiter.

<figure markdown="span">
    ![](https://ressources.piwigo.com/i?/uploads/c/v/7/cv7jpz6hf8//2026/06/29/20260629150900-80ede7d4-me.webp)
    <figcaption>Installationsseite</figcaption>
</figure>

Tragen Sie die Verbindungsdaten der MySQL-Datenbank wie folgt ein:

- MySQL-Host: `piwigo-db:3306`
- Benutzer: `piwigodb_user`
- Passwort: das Passwort, das Sie in die Datei `.env` geschrieben haben
- Name der Datenbank: `piwigodb`
- Präfix der Datenbanktabellen: `piwigo_` 

Für das Webmaster-Konto sind folgende Angaben erforderlich:

- Ein Benutzername, den Sie selbst wählen
- Ein Passwort, das Sie zur Kontrolle zweimal eingeben
- Ihre E-Mail-Adresse, damit Besucher Sie kontaktieren können

Klicken Sie auf „Start der Installation“.

<figure markdown="span">
    ![](https://ressources.piwigo.com/i?/uploads/c/v/7/cv7jpz6hf8//2026/06/29/20260629150900-9d12dd40-la.webp)
    <figcaption>Erfolgreiche Installation</figcaption>
</figure>

Sie werden informiert, ob die Installation erfolgreich war oder fehlgeschlagen ist.

## Schritt 4 - Erste Anmeldung

Nach Abschluss der Installation können Sie Ihre Galerie aufrufen. Melden Sie sich mit Ihrem Webmaster-Konto an, dann gelangen Sie in den Administrationsbereich.

<figure markdown="span">
    ![](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8//2026/06/26/20260626155501-7cf8f4d0.webp)
    <figcaption>Piwigo ist installiert</figcaption>
</figure>
