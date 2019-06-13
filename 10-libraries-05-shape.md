# Shape Library

Library zum Bearbeiten von Shapes

## Beispiele 

...
 
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


### composeAll

Verschmelzen einer ganzen Liste von Shapes (analog zu `compose`)

- `shapes` —  Liste der Shapes die verschmolzen werden sollen
- `method` —  Art der Verschmelzung (`Union`, `Intersection`, `Difference`, `Xor`)

## Links

- Verschmelzen von Shapes
	- Mengenlehre
	- Boolsche Operatoren 
	- Venn-Diagramme
- SVG





