# BITTE BEACHTEN!
**Dieses Programm wurde in Linux programmiert. Einige Änderungen müssen eventuell vorgenommen werden.

# Minecraft-Manager
Ein Discord-Bot, der Minecraft-Server steuern kann

# Abhängigkeiten
**py-cord v2.3**: Discord API
**mcrcon**: Minecraft Rcon commmunicator

# Installation
## Windows
**py-cord**

```py -3.10 -m pip install -U py-cord --pre```

**mcrcon**

```py -3.10 -m pip install mcrcon``

## Linux/Mac-OSX
**py-cord**

```python3.10 -m pip install -U py-cord --pre```


**mcrcon**

```python3.10 -m pip install mcrcon``

# Laufend

## Einen Server erstellen
Erstellen Sie einen neuen Ordner im Verzeichnis ~/servers, z.B. ~/servers/myserver

Installieren Sie in diesem Ordner die Datei server.jar und starten Sie sie, z.B. ```java -jar server.jar``` 

Erstellen Sie eine start.sh Datei z.B.

``` #!bin/bash (neue Zeile) java -Xms1024M -Xmx1024M -jar minecraft.jar --nogui```

Dann verwenden Sie den folgenden Befehl:

```chmod +x start.sh```

Stellen Sie sicher, dass es funktioniert, indem Sie verwenden: ```./start.sh```

## Hinzufügen des Servers
Starten Sie den Bot, und verwenden Sie dann den Befehl /add_server SERVERNAME PORT z.B. 56775 PASSWORD

Das Passwort und der Port werden in der server.properties Ihres Servers festgelegt. DIESE SIND NICHT FÜR DIE VERBINDUNG ZUM SERVER GEDACHT. 

Aktivieren Sie rcon auf dem Server in server.properties, indem Sie false durch true bei enable-rcon=false ersetzen 

Setzen Sie Ihr Passwort und den Port in server.properties, wo rcon.port=PORT und rcon.password=PASSWORD steht.

## Ausführen des Servers
Jetzt können Sie Ihren Server starten. Verwenden Sie den Befehl /start SERVERNAME und er sollte starten. 

Hinweis: Es dauert länger, beim ersten start
