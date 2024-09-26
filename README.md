
# Architecture Ref.Card 02 - React Application (serverless)

Link zur Übersicht<br/>
https://gitlab.com/bbwrl/m346-ref-card-overview

## Installation der benötigten Werkzeuge

Für das Bauen der App wird Node bzw. npm benötigt. Die Tools sind unter 
der folgenden URL zu finden. Für die meisten Benutzer:innen empfiehlt sich 
die LTS Version.<br/>
https://nodejs.org/en/download/

Node Version Manager<br/>
Für erfahren Benutzer:innen empfiehlt sich die Installation des 
Node Version Manager nvm. Dieses Tool erlaubt das Installiert und das 
Wechseln der Node Version über die Kommandozeile.<br/>
**Achtung: Node darf noch nicht auf dem Computer installiert sein.**<br/>
https://learn2torials.com/a/how-to-install-nvm


## Inbetriebnahme auf eigenem Computer

Projekt herunterladen<br/>
```git clone git@gitlab.com:bbwrl/m346-ref-card-02.git```
<br/>
```cd architecture-refcard-02```

### Projekt bauen und starten
Die Ausführung der Befehle erfolgt im Projektordner

Builden mit Node/npm<br/>
```$ npm install```

Das Projekt wird gebaut und die entsprechenden Dateien unter dem Ordner node_modules gespeichert.

Die App kann nun mit folgendem Befehl gestartet werden<br/>
```$ npm start```

Die App kann nun im Browser unter der URL http://localhost:3000 betrachtet werden.



### Inbetriebnahme mit Docker Container
Als erstes ein Dockerfile erstellen im Hauptordner

![Alt-Text](pictures/img.png)

### Git-Hub Actions YAML-Datei erstellen 
Das File muss in im Ordner .github/workflows sein welche neu erstellt werden müssen.

![Alt-Text](pictures/img_1.png)
![Alt-Text](pictures/img_2.png)

### Auf Dockerhub Access-Token erstellen

![Alt-Text](pictures/img_4.png)

### Token auf Git tun
Der Token muss dann auf git hinterlassen werden unter Secrets und der Name muss dann auch im YML file sein

![Alt-Text](pictures/img_5.png)

### File pushen auf Git
Dann ist es unter Actions ersichtlich

![Alt-Text](pictures/img_3.png)




