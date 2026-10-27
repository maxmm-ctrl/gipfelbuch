# Gipfelbuch

Persönliches Gipfel- und Tourenbuch als Web-App: topografische Karte, GPX-Auswertung, Bucketlist, Mehrtagestouren und Statistik.

**Datenschutz:** Diese Seite ist öffentlich, enthält aber keine Touren. Die Daten liegen in einem privaten Repository (`gipfelbuch.json`) und werden nur mit einem persönlichen Zugangsschlüssel geladen und gespeichert, der auf dem jeweiligen Gerät bleibt. Für Gipfelvorschläge und die Gipfelsuche gehen Koordinaten bzw. Suchbegriffe an OpenStreetMap (Overpass, Nominatim).

## Benutzung

- **Einrichten (einmal pro Gerät):** Fine-grained Token mit Zugriff nur auf das Datenrepository und der Berechtigung »Contents: Read and write« erstellen und in der App einfügen.
- **GPX importieren:** eine oder mehrere Workout-GPX wählen. Die App berechnet Datum, Dauer, Distanz, Höhenmeter und den höchsten Punkt und schlägt Gipfel und Land vor. Mehrere Dateien lassen sich als Mehrtagestour verknüpfen oder zu einer Tour zusammenführen.
- **Tour von Hand:** Formular mit Gipfelsuche und Punkt auf der Karte.
- **Bucketlist:** Ziele mit Priorität. Sobald derselbe Gipfel (und ggf. die Route) im Gipfelbuch steht, gilt das Ziel als erledigt.
- **Statistik:** Touren, Gipfel, Tage, Höhenmeter pro Jahr und Sportart, Mehrtagestouren.
- **Excel:** Export als Backup, Import aus einer Excel-Liste.
- Jede Änderung ist ein Commit im Datenrepository, der Verlauf ist dort einsehbar und wiederherstellbar.

## Kartendaten

OpenTopoMap-R und OpenHikingMap über [openmaps.fr](https://openmaps.fr) (CC-BY-SA), Daten © OpenStreetMap-Mitwirkende, SRTM · swisstopo · Esri World Imagery.
