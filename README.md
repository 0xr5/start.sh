# start.sh
Eine einfache Start-Datei für Minecraft Server aller Art. Ausgelegt für Server, alle Anforderungen für den eigentlichen Minecraft-Server (zu finden auf der jeweiligen Seite z.B Spigot) müssen installiert sein.
### Zusätzliche Pakete

Damit man den Server auch beim verlassen der Konsole verwenden kann, muss ein Paket installiert werden. Hierfür stellen wir erstmal sicher, dass wir die neuesten Pakete für unseren Server installiert haben. Anschließend installieren wir Screen.

```
$ sudo apt-get update -y && sudo apt-get upgrade -y
$ sudo apt-get install screen
```

### Erklärung der Parameter

```
screen -AmdS Minecraft java -Xms512M -Xmx4096M -jar server.jar
```
| Parameter  | Erklärung |
| ------------- | ------------- |
| screen -AmdS Minecraft | Erstellt ein neues Screen-Fenster mit dem Namen "Minecraft".  |
| java | Öffnet eine Java Anwendung.  |
| -Xms512M | Legt die Minimale Ram-Auslastung des Servers fest. (hier 512MB)  |
| -Xmx4069M | Legt die Maximale Ram-Auslastung des Servers fest. (hier 4GB) |
| -jar server.jar | Setzt für Java den Parameter -jar und gibt die Datei an, die geöffnet werden soll. |

### Andere Ram-Einstellungen
Je nach Hardware auf dem Server benötigt jeder Minecraft Server individuelle Einstelungen. Hat man z.B nur 2GB Ram, sollte dieser nicht alleine vom Minecraft Server belegt werden. Deshalb sollte man darauf achten, die richtigen Einstellungen für den jeweiligen Server zu finden. Hier gibt es eine Tabelle mit den beliebtesten Schritten, mit einer Empfehlung von mir. 1024M = 1GB Ram | 2048M = 2GB Ram usw.

| MB (M)  | Empfehlung |
| ------------- | ------------- |
| 64M  | Min |
| 128M  | Min  |
| 256M  | Min |
| 512M  | Min |
| 1024M  | Min & Max |
| 2048M  | Max |
| 4096M  | Max|
| 8192M  | Max|
| 16384M  | Max|
