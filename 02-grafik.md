# Grafik

## Grundformen

- Dreieck, Quadrat, Kreis:
	- Dreieck, oder allgemein Vieleck: `polygon`
	
	![](assets/shape_1.gif)
	
	- Quadrat, oder allgemein Rechteck: `rect`
	
	Durch die Einstellung lässt sich aus dem Rechteck auch eine Ellipse oder ein Kreis formen.
	
	![](assets/shape_2.gif)
	
	- Kreis, oder allgemein Ellipse: `ellipse`
	
	![](assets/shape_3.gif)
	
	- Stern: `star`
	
	Verändert man die Einstellungen des Knoten so lässte sich auch ein Dreieck formen.
	
	![](assets/shape_4.gif)

## Shapes

- Ein Shape hat:
	- eine Füllfarbe (`fill`) 
	- eine Umrißfarbe (`stroke`)
	- eine Strichstärke (`strokeWidth`)
	
	Es lässt sich ebenfalls die Deckkraft des Stiches und/oder Der Füllung einstellen.
	
	![](assets/fill.png)
	
- Diese Eigenschaften kann man mit dem `colorize`-Knoten ändern.

![](assets/shape_5.gif)

## Pfade

- Eine Shape ohne Füllung (mit transparenter Füllung) ist ein Pfad.
- Ein Pfad setzt sich zusammen aus:
	- Grade Strecken
	- Bezier-Kurven
	- Kreis-Segemente
	- Sprünge

## Kontouren

- Ein Pfad kann aus ein oder mehreren Konturen bestehen
	- Beispiel: `textPath`erzeugt eine Shape mit Innen und Außenkonturen. 
	- Mit `wiggleContour` kann man die Kontouren durcheinanderschütteln
	
	![](assets/contour.gif)
	
- Es gibt *Außenkontouren* und *Innen-Kontouren*
  (Beispiel: Buchstabe 'O')
- Eine Kontour kann offen sein (Pfad mit Anfang und Ende) oder Geschlossen (Outline einer Shape)

## Gruppen

- Mehrere Shapes kann man mit `group` zu einer Gruppe zusammengefassen.


## Anordnen

- Layout
	- Einpassen in einen Bereich: `fit`
	- Einpassen in Objekte: `fitTo`
	- Ausrichten: `align`
	
	![](assets/align.png)
	
	- Stapeln: `stack` [![](assets/beispiel.png)](https://nodebox.live/nodebox-intro/b02stack)
	
	![](assets/stack.gif)]
	
- Listen
	- Liste von Objekten mit `combine` erstellen  [![](assets/beispiel.png)](https://nodebox.live/nodebox-intro/b02combine)
	
	![](assets/combine.png)
	
	- Die Objekte werden in der Reihenfolge gemalt in der sie in der Liste stehen
	- Neu sortiern mit `shapeSort`
	
- Gruppieren:
	- `group`und `ungroup`
	- Gruppe filtern: `deletePaths`
	
	![](assets/deletepaths.gif)
	
	- Gruppen werden als ein Objekt behandelt
	- Beispiel `fit` mit Liste vs Gruppe

## Flächen verschmelzen

- Jeder Pfad ist bereits eine Fläche / Flächenumriss
- Pfade verbinden / einfärben mit `colorize`
- Boolsche Flächen-Operationen:`compound` [![](assets/beispiel.png)](https://nodebox.live/nodebox-intro/b02compund)
	- Zwei Flächen verschmelzen
	- Flächen ausschneiden
	- Mehrere Flächen verschmelzen
	
	![](assets/compound.gif)
	
- Morphen zwischen Flächen

	


	
