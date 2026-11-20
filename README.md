# QSL-Auswertung

Statische, browserbasierte Auswertung der festen QSO-Daten in `qsos.json`. Die Datendatei enthält die 11.414 QSOs aus der gelieferten Auswertung mit den für die QSL-Planung benötigten Angaben.

## Berechnung

QSOs werden nach sendender Station und gearbeitetem Rufzeichen gruppiert. Der Kartenbedarf jeder Kombination wird aufgerundet:

`Karten = aufgerundet(QSOs / QSOs je Karte)`

In der Seite ist zwischen 2, 3 und 4 QSOs pro Karte umschaltbar. Filter, Summen, Tabelle und CSV-Export verwenden die ausgewählte Zahl.

## GitHub Pages

Unter **Settings → Pages** als Build- und Deploymentquelle **GitHub Actions** auswählen. Der Workflow veröffentlicht die Dateien im Repository-Root. Danach ist die Seite unter `https://bitkauz.github.io/QSL-Auswertung/` erreichbar.

Die Auswertung läuft im Browser und braucht weder Datenbank noch Backend.