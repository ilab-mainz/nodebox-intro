# Shape Library

Library zum Bearbeiten von Shapes

## Beispiele 

- [shapeTest](https://nodebox.live/bitcraftlab/shapeTest)
	- `toContoursTest` — Textpfad in einzelne Kontouren zerlegen
	- `toShapeTest` — to be done
- [compoundTest](https://nodebox.live/bitcraftlab/compoundTest)
	- XOR-compound of 9 rotating rounded rectangles

## Nodes

### toShape

Erstellt eine Shape aus einem SVG-Code

- `string` —  SVG Dokument als Zeichenkette

**Achtung:**

- Der SVG-Code kann direkt aus Adobe Illustrator exportiert werden  
 (`Export As` > `Show Code`)
- Der Nodebox SVG-Parser funktioniert nur mit Pfaden  
(keine Polygone, Farben, Gruppen, Artboards, etc)
- Einzelne Konturen kann man in Nodebox mit der Funktion `toContours` extrahieren  
  (in der Curve Library enthalten)


### compoundAll

Verschmelzen einer ganzen Liste von Shapes (analog zu `compose`)

- `shapes` —  Liste der Shapes die verschmolzen werden sollen
- `method` —  Art der Verschmelzung (`Union`, `Intersection`, `Difference`, `Xor`)

### toContours

Kontouren einer Shape extrahieren

- `shape` — Form die zerlegt werden soll

### reduce

Hilfsfunktion um einen Knoten sukzessive auf alle Elemente einer Liste anzuwenden

## Links

- Verschmelzen von Shapes
	- [Boolsche Operatoren](https://en.wikipedia.org/wiki/Boolean_operations_on_polygons) (Wikipedia)
	- [Venn-Diagramme](https://de.wikipedia.org/wiki/Mengendiagramm) (Wikipedia)
- SVG
	- [SVG Artikel](https://de.wikipedia.org/wiki/Scalable_Vector_Graphics) (Wikipedia)
	- [SVG Wikibook](https://de.wikibooks.org/wiki/SVG) (deutsch)
		- [SVG Pfade](https://de.wikibooks.org/wiki/SVG/_Pfade) (sehr lesenswert)
	- [SVG Primer](https://www.w3.org/Graphics/SVG/IG/resources/svgprimer.html) (W3C) 

## Achtung

- Compound ist sehr ineffizient - zerstört und bläst Pfade auf (siehe auch [hier](https://github.com/nodebox/live/issues/40))

