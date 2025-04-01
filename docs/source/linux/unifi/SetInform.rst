.. _set-inform:

Set-Inform: Adoptieren von UniFi-Geräten in den Controller
=====================================================

Um ein UniFi-Gerät in den Controller zu adoptieren, kann der `set-inform` Befehl verwendet werden. Dieser Befehl sendet eine Inform-Nachricht an das Gerät, die es dazu bringt, sich mit dem Controller zu verbinden.

Voraussetzungen
---------------

* Das UniFi-Gerät muss bereits eingeschaltet und mit dem Netzwerk verbunden sein.
* Der Controller muss installiert und konfiguriert sein.
* Der `set-inform` Befehl muss auf dem Gerät ausgeführt werden, das adoptiert werden soll.

Schritte
--------

1. **Ermitteln Sie die IP-Adresse des Geräts**
   Öffnen Sie ein Terminal oder eine Kommandozeile und geben Sie den Befehl ``ping <Geräte-IP-Adresse>`` ein, um die IP-Adresse des Geräts zu ermitteln.

2. **Verbinden Sie sich mit dem Gerät**
   Öffnen Sie ein Terminal oder eine Kommandozeile und geben Sie den Befehl ``ssh <Geräte-IP-Adresse>`` ein, um eine SSH-Verbindung zum Gerät herzustellen.

3. **Führen Sie den set-inform Befehl aus**
   Geben Sie den Befehl ``set-inform http://<Controller-IP-Adresse>:8080/inform`` ein, um die Inform-Nachricht an den Controller zu senden.

   Beispiel:
   ::
     set-inform http://192.168.1.100:8080/inform

   Ersetzen Sie ``<Controller-IP-Adresse>`` durch die IP-Adresse Ihres Controllers.

4. **Überprüfen Sie die Adoption**
   Öffnen Sie den UniFi-Controller und überprüfen Sie, ob das Gerät erfolgreich adoptiert wurde.

Hinweis
------

* Stellen Sie sicher, dass der Controller korrekt konfiguriert ist und die Inform-Nachrichten akzeptiert.
* Wenn das Gerät nicht adoptiert werden kann, überprüfen Sie die IP-Adresse des Geräts und des Controllers sowie die Netzwerkverbindung.

Fehlerbehebung
--------------

* Wenn der `set-inform` Befehl nicht erfolgreich ist, überprüfen Sie die IP-Adresse des Controllers und des Geräts sowie die Netzwerkverbindung.
* Wenn das Gerät nicht im Controller angezeigt wird, überprüfen Sie die Controller-Konfiguration und die Netzwerkverbindung.
