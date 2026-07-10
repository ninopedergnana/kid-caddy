# Stableford Caddy ⛳

Mobile-first Web-App zum Zählen von Stableford-Punkten auf der Golfrunde.
Läuft komplett im Browser, ohne Server, ohne Konto – alle Daten bleiben auf deinem Handy.

## Funktionen

- **Spielansicht**: grosser Schlag-Button, Strafen nach Häufigkeit sortiert (Out of Bounds und Ball verloren zuoberst), Rückgängig, Loch streichen, Bestätigung beim Abschluss jedes Lochs
- **Stableford**: korrekte Punkteberechnung mit Course Handicap und Verteilung der Vorgabeschläge nach Stroke Index; Live-Anzeige, bis zu wie vielen Schlägen es noch Punkte gibt
- **Plätze**: 9- oder 18-Loch-Plätze mit Par und Stroke Index erfassen; bei 18-Loch-Plätzen auch nur Front 9 oder Back 9 spielbar
- **Scorecard**: laufende Runde live, Historie aller Runden mit Details
- **Regeln**: Nachschlagewerk mit Suche (Penalty Areas, OB, Bio-Zone, Cart Path, Droppen u.v.m.) – über das «i» auf den Straf-Buttons direkt erreichbar
- **Dreisprachig**: Deutsch, Englisch, Französisch (umschaltbar im Plätze-Tab)
- **Offline-fähig (PWA)**: einmal geladen, funktioniert die App auch ohne Empfang auf dem Platz
- **Export/Import**: Daten als JSON-Datei sichern und wiederherstellen

## Gratis hosten auf GitHub Pages

1. Auf [github.com](https://github.com) einloggen (oder gratis Konto erstellen).
2. Oben rechts **+** → **New repository**. Name z.B. `stableford-caddy`, **Public**, dann **Create repository**.
3. Auf der Repository-Seite: **uploading an existing file** anklicken und diese Dateien hochladen:
   `index.html`, `sw.js`, `manifest.json`, `icon-192.png`, `icon-512.png`
   Dann **Commit changes**.
4. Im Repository: **Settings** → **Pages** → unter *Branch* den Branch `main` und Ordner `/ (root)` wählen → **Save**.
5. Nach 1–2 Minuten ist die App erreichbar unter:
   `https://DEIN-BENUTZERNAME.github.io/stableford-caddy/`

## Auf dem Handy installieren

Die Seite im Handy-Browser öffnen, dann:

- **iPhone (Safari)**: Teilen-Symbol → «Zum Home-Bildschirm»
- **Android (Chrome)**: Menü (⋮) → «App installieren» bzw. «Zum Startbildschirm hinzufügen»

Danach startet die App vom Home-Bildschirm wie eine normale App und funktioniert offline.

## Wichtig: Daten sichern

Alle Plätze und Runden liegen im Speicher des Browsers (localStorage). Beim Löschen der
Browserdaten oder einem Handywechsel gehen sie verloren. Deshalb regelmässig im Tab
**Plätze → Daten sichern (Export)** eine JSON-Datei herunterladen. Mit **Import** kann sie
jederzeit wiederhergestellt werden.

## Bedienung in Kürze

1. **Plätze**: Platz anlegen (Par + Stroke Index je Loch).
2. **Spiel**: Platz wählen, Course Handicap eingeben, los.
3. Nach jedem Schlag den grossen Ball drücken; bei Strafen den passenden Button
   (der erneute Schlag nach OB zählt normal über den Ball-Button).
4. **Loch fertig** → Bestätigung → nächstes Loch. Keine Punkte mehr möglich? **Loch streichen**.
5. Nach dem letzten Loch wird die Runde automatisch in der Scorecard-Historie gespeichert.

Hinweis: Das Regel-Nachschlagewerk ist eine vereinfachte Gedächtnisstütze und ersetzt die
offiziellen Golfregeln (R&A/USGA) und lokalen Platzregeln nicht.
