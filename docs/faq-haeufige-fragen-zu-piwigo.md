---
title: FAQ - Häufige Fragen zu Piwigo
description: Auf dieser Seite haben wir die Antworten auf die Fragen zusammengefasst, die uns zur Nutzung von Piwigo am häufigsten gestellt werden. Wenn Sie ein Problem haben, schauen Sie zuerst hier nach!
---

# FAQ - Die häufigsten Fragen zu Piwigo

**Auf dieser Seite haben wir die Antworten auf die Fragen zusammengefasst, die uns zur Nutzung von Piwigo am häufigsten gestellt werden. Wenn Sie ein Problem haben, schauen Sie zuerst hier nach!**

Klicken Sie auf den Pfeil, um die Antwort auf eine Frage anzuzeigen.

---

- Hilfe, ich sehe meine Fotos / meine Alben nicht!
    
    Sie haben ein Album erstellt und sehen es nicht in Ihrer Galerie?
    
    Keine Panik! Wahrscheinlich liegt es an den Zugriffsrechten. 
    
    Wenn Ihr Album privat ist und Sie sich selbst keine Rechte dafür gegeben haben, ist es logisch, dass Sie es nicht in Ihrer Galerie sehen. 
    
    Um das zu prüfen, öffnen Sie den Administrationsbereich und dann Alben > Verwaltung. Suchen Sie Ihr Album und bearbeiten Sie es. Öffnen Sie den Tab „Zugriffsrechte“. Wenn Ihr Album privat ist, stellen Sie sicher, dass Sie die Berechtigung haben, es anzusehen. 
    
    [Mehr über die Zugriffsrechte von Alben erfahren](alben-organisieren/zugriffsrechte-und-sichtbarkeit-von-alben.md)
    
    Wenn Sie die Berechtigung haben, dieses Album anzusehen, stellen Sie sicher, dass es nicht leer ist (also Fotos enthält). Leere Alben sind in der Galerie nicht sichtbar.
    
    Wenn Sie ein Album sehen, ein anderer Benutzer aber nicht, obwohl er Zugriffsrechte für dieses Album hat: Stellen Sie sicher, dass das Album nicht gesperrt ist!
    
- Die E-Mails von meinem Piwigo kommen nicht an (oder landen im Spam-Ordner)
    
    Die Benachrichtigungs-E-Mails von Piwigo werden mit der E-Mail-Adresse des Hauptadministrators (Webmaster) versendet, also des ersten Benutzers, der erstellt wurde. 
    
    Manchmal darf der Server, auf dem Ihr Piwigo läuft, keine E-Mails mit dieser Adresse versenden. Die E-Mails landen dann im Spam oder kommen gar nicht an.
    
    Für dieses Problem gibt es mehrere Lösungen:
    
    - Die E-Mail-Adresse des Webmasters ändern: Damit die E-Mails ihr Ziel erreichen, muss Ihre Piwigo-Galerie berechtigt sein, E-Mails mit der Adresse des Webmasters Ihrer Website zu versenden. Mit einer Adresse von Gmail, Yahoo usw. funktioniert der Versand aus Piwigo möglicherweise nicht. Idealerweise hat die E-Mail-Adresse des Webmasters denselben Domainnamen wie Ihre Galerie. Lautet die Adresse Ihrer Galerie zum Beispiel photos.mysite.com, sollte die E-Mail-Adresse des Webmasters idealerweise etwa *@mysite.com sein.
    - Das Plugin Protect Notification installieren: Das Plugin Protect Notification ersetzt den Absender der E-Mails durch eine Adresse wie no-reply@mysite.com (wobei mysite.com durch den Domainnamen Ihrer Galerie ersetzt wird). In der Regel löst die Installation dieses Plugins die E-Mail-Probleme. Seit Februar 2024 ist Protect Notification bei neuen Piwigo-Konten standardmässig aktiviert.
    - ⚠️ Diese Lösungen beheben keine Probleme beim Empfang von E-Mails, die über das Plugin Contact Form gesendet werden, da diese mit der im Formular eingegebenen E-Mail-Adresse versendet werden. Wie Sie Probleme mit dem Plugin Contact Form lösen, erfahren Sie [auf dieser Seite](ihre-galerie-anpassen/seiten-zur-galerie-hinzufuegen.md).
- Wie lösche ich mein Piwigo-Cloud-Konto?
    
    Wenden Sie sich an den Support unter support@piwigo.com.
    
- Wie verknüpfe ich meine Piwigo-Cloud-Galerie mit einem eigenen Domainnamen?
    
    Standardmässig haben alle Piwigo-Cloud-Konten eine Webadresse der Form *.piwigo.com. Sie können Ihren eigenen Domainnamen oder eine einfache Subdomain hinzufügen. 
    
    Da Piwigo cloud keine Domainnamen verkauft, müssen Sie ihn bei einem Domain-Anbieter wie OVH kaufen. 
    Schicken Sie uns eine E-Mail an support@piwigo.com und teilen Sie uns Ihren Domainnamen (oder Ihre Subdomain) mit. 
    Wir richten die Server von Piwigo cloud ein und erklären Ihnen, wie Sie Ihren Domainnamen konfigurieren. 
    Sobald die DNS-Konfiguration übernommen wurde, fügen wir mit HTTPS eine zusätzliche Sicherheitsebene hinzu.
    
- Wie benenne ich mein Piwigo-Cloud-Konto um?
    
    Wenden Sie sich an den Support unter support@piwigo.com.
    
- Wie ändere ich den Titel meiner Piwigo-Galerie?
    
    Um den Titel Ihrer Galerie zu ändern, öffnen Sie im Administrationsbereich von Piwigo das Menü Konfiguration > Optionen. Im ersten Tab können Sie den Namen Ihrer Galerie im ersten Feld „Galerie-Titel“ ändern. 
    
- Wie mache ich meine Galerie in Suchmaschinen sichtbar?
    
    Sobald Ihre Galerie erstellt ist, sollte sie in Suchmaschinen sichtbar sein. Wenn Ihr Domainname jedoch neu ist oder Sie wenig Besucher haben, kann das eine Weile dauern. 
    
    Mit diesen Tipps machen Sie Suchmaschinen auf Ihre Piwigo-Galerie aufmerksam:
    
    - Setzen Sie Links zu Ihrer Galerie auf Websites, die bereits Besucher haben
    - Teilen Sie Ihre Galerie in den sozialen Medien
    - Fügen Sie Ihre Galerie zur [Google Search Console](https://search.google.com/search-console/welcome) (für Google) oder zu den [Bing Webmaster Tools](https://www.bing.com/webmasters/about) (für Bing) hinzu.
- Wie sorge ich dafür, dass meine Galerie NICHT in Suchmaschinen sichtbar ist?
    
    Wenn Ihre Galerie nicht in Suchmaschinen sichtbar sein soll, können Sie im Stammverzeichnis Ihrer Website eine Datei robots.txt anlegen (wenn Sie eine selbst gehostete Galerie nutzen) und folgende Zeilen einfügen:
    
    ```html
    User-agent: *
    Disallow: /
    ```
    
    Sie können die Sichtbarkeit Ihrer Galerie in Suchmaschinen auch mit dem Plugin Meta steuern. Mit diesem Plugin legen Sie die Metadaten Ihrer Website für Suchmaschinen fest, sowohl für die gesamte Website als auch für einzelne Seiten.
    
    Um die Indexierung Ihrer Piwigo-Galerie in Suchmaschinen mit dem Plugin Meta vollständig zu deaktivieren, öffnen Sie die Einstellungen des Plugins und wählen Sie im ersten Tab die Metadaten „robots“ aus. Bearbeiten Sie die Metadaten, geben Sie den Wert `noindex` ein und klicken Sie dann auf „Metadaten einfügen“.
    
    [Mehr über Plugins zur Indexierung Ihrer Galerie erfahren](piwigo-administrieren/plugins-fuer-administratoren.md)
    
- Wie lege ich den Titel und die Beschreibung meiner Galerie in Suchmaschinen fest?
    
    Um anzupassen, wie die Seiten Ihrer Galerie in Suchmaschinen angezeigt werden, installieren Sie die Plugins Title und Meta.
    
    Mit dem Plugin Title ändern Sie den Titel, der für jede Seite in Suchmaschinen angezeigt wird. 
    
    Mit dem Plugin Meta ändern Sie die Beschreibung, die für jede Seite in Suchmaschinen angezeigt wird.
    
    ![Titre et description.jpg](https://ressources.piwigo.com/uploads/c/v/7/cv7jpz6hf8/2026/07/03/20260703190344-cc312049.jpg)
    
    [Mehr über Plugins zur Indexierung Ihrer Galerie erfahren](piwigo-administrieren/plugins-fuer-administratoren.md)
    
- Wie ändere ich das Aussehen meiner Galerie, wenn sie in sozialen Medien geteilt wird?
    
    Um das Aussehen (Titel, Beschreibung, Bild...) der Seiten Ihrer Galerie beim Teilen in sozialen Medien anzupassen, können Sie das Plugin **Meta Open Graph** installieren. [Mehr erfahren](piwigo-administrieren/plugins-fuer-administratoren.md)
    
- Wie ändere ich die Fusszeile meiner Galerie?
    
    Standardmässig zeigt Ihre Galerie unten auf der Seite einen Text mit einem Link zu Piwigo cloud oder piwigo.org an (je nachdem, ob Ihre Galerie bei Piwigo cloud oder auf Ihrem eigenen Hosting liegt). 
    
    Wenn Sie die Fusszeile Ihrer Galerie anpassen möchten, können Sie das Plugin **Perso Footer** installieren ([mehr erfahren](ihre-galerie-anpassen/plugins-zur-galerie-anpassung.md)).
    
    Wenn Sie die Fusszeile vollständig ausblenden möchten (und damit keine Werbung für Piwigo mehr machen 😢), können Sie mit dem Plugin LocalFiles Editor folgenden Code in die CSS-Datei der Website einfügen ([mehr über LocalFiles Editor erfahren](piwigo-selbst-hosten/lokale-konfiguration-bearbeiten-localfiles-editor.md)). Das wäre allerdings schade.
    
    ```css
    #copyright{display: none;}
    ```
    
    Zusätzlich zur Standard-Fusszeile können Sie auch eine eigene Fusszeile erstellen, indem Sie mit dem Plugin [PWG Stuffs](ihre-galerie-anpassen/plugins-zur-galerie-anpassung/pwg-stuffs-bloecke-in-ihrer-galerie-hinzufuegen.md) einen eigenen Block anlegen. 
    
- Wie füge ich meiner Piwigo-Website ein eigenes Banner / Foto hinzu?
    
    Es gibt mehrere Möglichkeiten, Ihr Piwigo mit einem Hintergrundbild auf der Startseite oder einem Banner auf den Seiten Ihrer Website anzupassen. 
    
    Wie das geht, erfahren Sie in diesem Artikel:
    
    [Eigenes Banner](ihre-galerie-anpassen/eigenes-banner-zur-galerie-hinzufuegen.md)
    
- Wie erhalte ich bei Piwigo cloud eine Rechnung?
    
    Sie benötigen eine Rechnung für Ihr Abonnement bei Piwigo cloud?
    
    - Wenn Sie vor der Zahlung eine Rechnung benötigen: Fragen Sie den Support. Achtung: Wenn Sie eine Rechnung anfordern, müssen Sie sie auch bezahlen.
    - Wenn Sie nach der Zahlung eine Rechnung benötigen: Kein Problem, sie steht automatisch in Ihrem Piwigo-Administrationsbereich zur Verfügung, im Menü Mein Konto > Verwaltung, im Tab für die Abrechnung.
