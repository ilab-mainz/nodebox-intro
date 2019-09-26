# Grundlagen

*Die grundlegende Konzepte hinter Nodebox.live*


## Nodebox als Fließband

![](https://media.giphy.com/media/wKfYItv9gsjXG/giphy.gif)

## Knoten

Wenn wir Knoten miteinander verbinden entsteht eine art Fließband bei der die informationen an jeden einzenen Arbeiter (also Knoten) weitergeben werden um Formen zu erzeugen und zu verändern.

### Beispiel:

1. Erstellen wir einen `rect` Knoten.

	![](assets/basics_1.png)

2. Verbinden wir einen `Colorize` Knoten mit dem `rect` Knoten. Er verändert den Output und färbt ihn ein.

  ![](assets/basics_2.png)

3. Anschließend fügen wir einen `rotate` Knoten hinzu. Er nimmt den output und rotiert ihn.

   ![](assets/basics_3.png)

Wir Können jeden einezelnen Schritt nachvolziehen indem wir mit einem Doppelklick den aktiven Knoten (Render-Knoten) wechseln:

![](assets/basics_render.gif)


## Ein- und Ausgänge


- Jeder Knoten verarbeitet ein oder mehrere Eingaben (Inputs) um eine Ausgabe (Output) zu erzeugen.

  ![](assets/grundlagen_input_output.png)
  
- Alle Eingang-Ports in Nodebox erwarten Input eines bestimmten Typs. Jeder Ausgang-Port erzeugt einen Output eines bestimmten Typs. 
- Wenn man über einem Eingangs mit der Maus verweilt sieht man welchen Datentypen der Knoten an diesem Port erwartet. 
- Wenn man über dem Ausgang mit der Maus verweilt sieht man welchen Datentyp der Output des Knotens hat.

  ![](assets/grundlagen_input_art.png)

## Datentypen

Die Datentypen an den Ports werden in der Regel durch Farben codiert:

### Zahlen

- ![#5DA5DA](https://placehold.it/15/5DA5DA?text=+) `Nummern` sind sowohl ganzzahlige werte `integer` (zb. 1 / 5 / 72 usw.)   
als auch Zahlen mit nachkomma stellen `float` (z.B 0.25 / 1.678 / 3.333 usw.)

	- `float`werden benutzt um um z.B die breite/höhe eine Objekts zu verändern.
	- `integer` werden benutzt um Mengen anzugeben also z.B. 10 Kopien im `copy` Knoten

### Points

- ![#60BD68](https://placehold.it/15/60BD68?text=+) `Points` (Punkte) sind zwei dimensionale Koordinaten die `X` und `Y` koordinaten enthalten.
	- Sie können benutzt werden um ein Ort zu bestimmen z.B die position eines Rechtecks, die Skalierung im `scale` Knoten oder den dreh und Angelpunkt eins `rotate` Knoten (also den Punkt um den rotiert werden soll)

### Shapes

- ![#E8AA00](https://placehold.it/15/E8AA00?text=+) `Shapes` (Formen) enthalten Informationen über Kurven, Linien und Punkte.

### Strings
- ![#F17CB0](https://placehold.it/15/F17CB0?text=+) `Strings` (Zeichenketten) enthalten reinen Text.
	- In der Regel der text in dem `textpath` Knoten.

### Listen

- ![#B276B2](https://placehold.it/15/B276B2?text=+) `Listen` sind Sammlungen und können deshalb mehrere `Nummern` `Points`, `Shapes` und `Colors` Enthalten.
	- Deshalb können sie auch mit Eingängen Verbunden werden die einen anderen Typ erwarten. d.H so lange die Liste aus Zahlen besteht kann sie auch mit dem ![#5DA5DA](https://placehold.it/15/5DA5DA?text=+) `Nummern` Eingang verbunden werden.

### Farben
- ![#DECF3F](https://placehold.it/15/DECF3F?text=+) `Colors` enthalten Farbwerte in der Form von red/green/blue/alpha (`rgbColor`) oder hue/saturation/brightness/alpha (`hsbColor`) werten.
	- Sie werden benutzt um Farbwerte zu definieren: z.B die Füllfarbe eines Objekts oder die Kontur einer Linie
