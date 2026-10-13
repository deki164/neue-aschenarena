# Aschenarena (Browser, mit Online-Relay)

Das Spiel ist `public/index.html` (Three.js). `server.js` liefert die Seite aus und leitet
Online-Nachrichten zwischen zwei Spielern weiter. Keine Abhängigkeiten, nur Node 18+.

## Lokal testen
    node server.js        # dann http://localhost:3000 in zwei Browser-Tabs öffnen

## Auf Render bereitstellen (kostenlos)
1. Diesen Ordner in ein neues GitHub-Repository hochladen (Dateien direkt im Repo-Root).
2. render.com > New > **Web Service** > das Repo wählen.
3. Runtime: Node, Build Command leer lassen (oder `npm install`), Start Command: `node server.js`, Plan: Free.
4. Nach dem Deploy die Render-Adresse (https://....onrender.com) an den Freund schicken.

## Online spielen
Beide öffnen dieselbe Render-Adresse. Einer klickt **Match hosten** und schickt den angezeigten Code,
der andere gibt ihn ein und klickt **Beitreten**. Der Host rechnet das Spiel, der Gast schickt Eingaben.
Kostenlose Render-Dienste schlafen nach Inaktivität ein: der erste Aufruf kann bis zu einer Minute dauern.
