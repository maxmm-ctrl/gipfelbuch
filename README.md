# Gipfelbuch

Persönliches Gipfel- und Tourenbuch als Web-App: topografische Karte, GPX-Auswertung, Bucketlist, Mehrtagestouren und Statistik.

**Datenschutz:** Diese Seite ist öffentlich, enthält aber keine Touren. Die Daten liegen in einem privaten Repository (`gipfelbuch.json`) und werden nur mit einem persönlichen Zugangsschlüssel geladen und gespeichert, der auf dem jeweiligen Gerät bleibt. Für Gipfelvorschläge und die Gipfelsuche gehen Koordinaten bzw. Suchbegriffe an OpenStreetMap (Overpass, Nominatim).

## Benutzung

- **Einrichten (einmal pro Gerät):** Fine-grained Token mit Zugriff nur auf das Datenrepository und der Berechtigung »Contents: Read and write« erstellen und in der App einfügen.
- **GPX importieren:** eine oder mehrere Workout-GPX wählen. Die App berechnet Datum, Dauer, Distanz, Höhenmeter und den höchsten Punkt und schlägt Gipfel und Land vor. Mehrere Dateien lassen sich als Mehrtagestour verknüpfen oder zu einer Tour zusammenführen.
- **Tracks:** der Track wird vereinfacht (auf etwa 5 m genau) mitgespeichert und beim Antippen einer Tour gezeigt, alle zusammen über »Karte« → »Alle Tracks«. Gehört eine GPX zu einer Tour, die schon im Gipfelbuch steht (gleicher Tag, in der Nähe), wird nur der Track ergänzt. Einzelne Tracks lassen sich auch im Formular »Tour bearbeiten« anhängen, ersetzen oder entfernen.
- **Tour von Hand:** Formular mit Gipfelsuche und Punkt auf der Karte. Die Felder passen sich der Sportart an (z. B. Seillängen nur beim Klettern, Lawinenwarnstufe und Schnee bei Skitouren).
- **Mehrere Gipfel pro Tour:** beim GPX-Import werden Gipfel direkt am Weg automatisch erkannt, weitere lassen sich suchen und hinzufügen. Alle erscheinen auf der Karte und zählen in der Statistik.
- **Karte:** ▲ Gipfel, ● Routen ohne Gipfel, gestrichelter Ring = Bucketlist; alle drei unter »Auf der Karte« ein- und ausblendbar. Ein Tipp auf einen Punkt zeigt die Details in der Leiste und den Track der Tour in Rot, bei Mehrtagestouren alle Etappen. Stufenloser Zoom mit Mausrad, Trackpad und Fingern.
- **Kartenauswahl** (Knopf »Karte« oben rechts): OpenTopoMap, Mapy.com Outdoor, Satellit (Esri), Sentinel-2 Tagesbild mit Datum und Zeitraum, basemap.at (Karte, Laserscan-Gelände, Orthofoto), swisstopo Landeskarte, Kartverket Topo. Beschriftungen gehören automatisch zu Luftbildern; außerhalb ihres Landes zeigen die amtlichen Karten OpenTopoMap darunter. Darüber zuschaltbar: Wanderwege, Pisten & Loipen, berechnete Hangneigung, Straßen, alle Tracks.
- **Einstellungen → Karten:** Startkarte sowie die kostenlosen Schlüssel für Mapy.com und Copernicus (Sentinel-2); sie liegen im privaten Daten-Repository. Anleitung im Kartenvergleich (`karten.html`).
- **Handy:** die Liste ist ein Blatt über der Karte, das in drei Höhen einrastet (ziehen oder Griff antippen); Vollbild über den Knopf links oben.
- **Gipfel ja/nein:** Schalter »Gipfel« im Formular (standardmäßig an). Routen ohne Gipfel zählen nicht in der Gipfelstatistik, Gipfel am Weg zählen trotzdem.
- **Mehrtagestouren:** ein Tipp auf den Namen (↔) öffnet die Übersicht mit Zeitraum, Summen, Gipfeln und Etappen.
- **Bucketlist:** Ziele mit Priorität. Sobald derselbe Gipfel (und ggf. die Route) im Gipfelbuch steht, gilt das Ziel als erledigt.
- **Statistik:** Touren, Gipfel, Tage, Höhenmeter (auch als Vielfaches des Mount Everest), Gipfel über 3000 und 4000 m; persönliche Rekorde (höchster Gipfel, meiste Höhenmeter, Distanz und Zeit an einem Tag, längste Mehrtagestour, schwierigste Route), jeder mit Link zur Tour; Länder mit Gipfel (von 195) mit Flaggen, Kontinenten und Welt- bzw. Europakarte; Höhenmeter pro Jahr und Sportart, Mehrtagestouren.
- **Excel:** Export als Backup, Import aus einer Excel-Liste.
- Jede Änderung ist ein Commit im Datenrepository, der Verlauf ist dort einsehbar und wiederherstellbar.

## Kartendaten

OpenTopoMap-R und OpenHikingMap über [openmaps.fr](https://openmaps.fr) (CC-BY-SA), Daten © OpenStreetMap-Mitwirkende, SRTM · swisstopo · Esri World Imagery.

Weltkarte der Statistik (`welt.json`): Ländergrenzen von [Natural Earth](https://www.naturalearthdata.com) (gemeinfrei) über world-atlas, vorab projiziert. Flaggen: [flag-icons](https://github.com/lipis/flag-icons) (MIT).
