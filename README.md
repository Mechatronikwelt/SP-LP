# Swimming Pixel - Launchpad MIDI over TCP/IP and MQTT

### Einführung 
Die Stadt Karlsruhe wurde 2019 von der UNESCO mit dem Titel City of Media Arts ausgezeichnet. Repräsentativ für diese Auszeichnung stehen Events, wie die Schlosslichtspiele, aber auch dauerhafte Einrichtungen, wie zum Beispiel das ZKM.
Die Hochschule Karlsruhe möchte sich ebenfalls daran beteiligen, die Stadt durch mediale Kunst einzigartig zu machen.

So soll im Rahmen der Lehrveranstaltung Informationstechnik - Labor das Projekt Swimming Pixels verwirklicht werden. Hierzu sollen die Studierenden schwimmende LED-Pixel konstruieren, die unteranderem mit Hilfe eines MIDI-Launchpads angesteuert werden können und somit den Schlossteich mit verschiedenen Lichtsequenzen erstrahlen lassen.

Dokumentation: http://hit-karlsruhe.de/hit-info/info-ws20/SP-LP/

### Aufgabenstellung 
Die Aufgabe besteht darin, eine Kommunikation zwischen einem Launchpad und den 4x4 Pixeln mit Hilfe des MQTT-Protokolls herzustellen. Aufgrund der Verbindung von dem Launchpad und den Pixeln mit einem Broker sollen die Pixel in Abhängigkeit von unterschiedlichen Pads auf dem Launchpad die entsprechenden Farben ausgeben. Außerdem kann der Benutzer auswählen, welche Lightshow er darstellen möchte. Der Swimming Pixel ESP 32 Code wurde mit Arduino IDE umgesetzt und Der Host wurde mit Node-RED umgesetzt. Als MQTT-Kommunikation-Protokoll zwischen Host und Pixel wurde Mosquitto als Broker verwendet. Eine Erklärung vom Code wird zudem im YouTube Video erklärt.

Link zum Youtube: https://www.youtube.com/watch?v=PrtQgnCuUxU

### Getting Started
Im Ordner "Swimming_Pixel_MQTT_Lightshow" befinden sich 16 .ino Codes zu jedem ESP32 des Pixels. Jeder einzelne Code hat die folgenden Funktionen:
- Verbindung mit WiFi
- Verbindung mit Mosquitto Broker 
- Abonnement vom Topic 
- Ansteuerung von RGB-Rings/Panels
- Bearbeitung der Nachrichten von Node-RED
- Lightshow Funktionen und Darstellungen
