# Synchronisierter Notion Lern-Timer + Windows-Begleit-App

Dieses Paket ersetzt die Dateien im bestehenden GitHub-Pages-Repository.

## Dateien hochladen

Alle Dateien direkt in die oberste Ebene des Repositorys laden:

- index.html
- widget.css
- widget.js
- companion.html
- companion.css
- companion.js
- manifest.webmanifest
- sw.js
- icon-192.png
- icon-512.png
- .nojekyll

GitHub Pages bleibt auf `main` und `/ (root)`.

## Einmalige Verbindung

1. Notion-Widget neu einbetten oder aktualisieren.
2. Im Widget `Code kopieren` anklicken.
3. `Begleit-App öffnen` anklicken.
4. Code in der Windows-Begleit-App einfügen und `Verbinden` wählen.
5. `Windows-Benachrichtigung` aktivieren und in Edge `Allow` wählen.
6. Optional `App installieren` anklicken.

Danach steuert nur das Notion-Widget die Zeiten. Die Begleit-App übernimmt Start, Pause, Fortsetzen, Reset und Zeitänderungen.

## Technische Hinweise

Die Synchronisierung läuft über einen zufälligen ntfy.sh-Topic-Code. Der Code wird erst beim Benutzer im Browser erzeugt und steht nicht im öffentlichen GitHub-Quelltext. Nachrichten werden mit `Cache: no` und `Firebase: no` versendet. Die Begleit-App muss geöffnet oder minimiert bleiben.
