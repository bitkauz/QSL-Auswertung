# QSL-Auswertung

Statische, browserbasierte Auswertung der festen QSO-Daten in `qsos.json`. Die Datendatei enthält die 11.414 QSOs aus der gelieferten Auswertung mit den für die QSL-Planung benötigten Angaben.

## Berechnung

QSOs werden nach sendender Station und gearbeitetem Rufzeichen gruppiert. Der Kartenbedarf je Kombination wird aufgerundet:

`Karten = aufgerundet(QSOs / QSOs je Karte)`

In der Seite kann zwischen 2, 3 und 4 QSOs pro Karte umgeschaltet werden. Filter, Summen, Tabelle und CSV-Export verwenden die gewählte Einstellung.

## GitHub Pages

GitHub Pages veröffentlicht den Repository-Root automatisch bei jedem Push auf `main`. Die Datei `.nojekyll` sorgt dafür, dass die statischen Dateien unverändert ausgeliefert werden.

Die Seite ist unter [https://bitkauz.github.io/QSL-Auswertung/](https://bitkauz.github.io/QSL-Auswertung/) erreichbar. Die Auswertung läuft vollständig im Browser und benötigt weder Datenbank noch Backend.