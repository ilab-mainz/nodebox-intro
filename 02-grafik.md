# Grafik

## Grundformen

- Dreieck, Quadrat, Kreis:
	- Dreieck, oder allgemein Vieleck: `polygon`
	- Quadrat, oder allgemein Rechteck: `rect`
	- Kreis, oder allgemein Ellipse: `ellipse`
	- Stern: `star`


## Flächen anordnen

- Layout
	- Einpassen in einen Bereich: `fit`
	- Einpassen in Objekte: `fitto`
	- Ausrichten: `align`
	- Stapeln: `stack`
- Gruppen
	- `group`und `ungroup`
	- Gruppe filtern: `deletePaths`
	- Gruppen werden als ein Objekt behandelt
	- Beispiel `fit` mit Liste vs Gruppe
	- Nötig um mehrere Geometrien zu verschmelzen
- Überlappen
	- Anordnung bei `combine` 
	- Neu sortiern mit `shapeSort`

## Flächen verbinden

- Jeder Pfad ist bereits eine Fläche / Flächenumriss
- Pfade verbinden / einfärben mit `colorize`
- Boolsche Flächen-Operationen:`compound`
	- Zwei Flächen verschmelzen
	- Flächen ausschneiden
	- Mehrere Flächen verschmelzen
- Morphen zwischen Flächen

	


	