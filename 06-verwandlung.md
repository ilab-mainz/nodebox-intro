# Verwandlung

*Transformation von Objekten*

## Flächen verwandeln
	
- _Affine_ Transformationen
	- verschieben: `translate`
	
	![](assets/translate.gif)
	
	- drehen: `rotate`
	
	![](assets/rotate.gif)
	
	- spiegeln: `flip`
	
	![](assets/flip.gif)
	
	- dehnen: `scale`
	
	![](assets/scale.gif)
	
	- kippen: `skew`
	
	![](assets/skew.gif)

## Eigene Transformationen

- Grafiken-Transformation durch Punkt-Transformation
- Flächen → Pfade → Punkte → X und Y →  *Transformation* →  X und Y → Punkte → Pfade → Flächen [![](assets/beispiel.png)](https://nodebox.live/nodebox-intro/b06eigene)

	![](assets/verwandlung.png)  

	- Pfade → Punkte: `toPoints` 
	
	![](assets/topoints_2.png)
	
	- Punkte → X und Y : `lookup`
	- Transformation : Mathematische Funktionen, Javascript etc.
	- X und Y → Punkte: `makePoint`
	
	![](assets/makepoint.png)
	
	- Punkte → Pfade: `connectPoints`
	
	![](assets/connectpoints.png)
	
	- Pfade → Fläche: `colorize` 
	
	![](assets/colorize_2.png)

## 2D-Transformation
	
- Warping mit Funktionen: Beispiel
- warp library: Beispiel
	
## 3D-Transformation

- Kippen mit `skew`: Beispiel
- Isometrische Geometrie simulieren: Beispiel



---

Weiter zur [07 – Chaos und Zufall](07-chaos-zufall.md) oder zur [Übersicht](readme.md)
