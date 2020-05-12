# Grundlagen

Auf diese Seite findet ihr die grundlegenden Konzepte hinter [NodeBox.live](http://nodebox.live) erklärt.

## Visuelle Programmierung

NodeBox ist ein Programm oder auch System zur visuellen Programmierung. D.h. Programme, also Abläufe, werden anhand visueller Elemente erstellt. Dies steht im Gegensatz zu text-basierter Programmierung, bei der Code, also Programmier-Text verfasst wird.

![Vergleich visuelle und code-basierte Programmierung](assets/compare.png)

Im Beispiel oben sind die zwei Rechtecke in der Mitte einmal mittels visueller Programmierung (links zu sehen) und einmal mittels code-basierter Programmierung erstellt (rechts zu lesen).

Bei der visuellen Programmierung hat man eine gute Übersicht des Ablaufs: im ersten Knoten (`rect`) oben wird die Form erzeugt und dann zum Einfärben an den zweiten Knoten (`colorize`) unten weiter gegeben. Das Programm ist zugleich Bedienoberfläche (Interface), da man hier die Werte, bspw. Größe od. Farbe, direkt ändern kann.

## Knoten: NodeBox als Fließband

![](https://media.giphy.com/media/wKfYItv9gsjXG/giphy.gif)

Wenn wir Knoten („node“ bedeutet im Engl. „Knoten“) miteinander verbinden, entsteht eine Art Fließband bei der die Informationen an jeden einzenen Arbeiter (also Knoten) weitergeben werden um Formen zu erzeugen und zu verändern.

In NodeBox, wie in vielen anderen visuellen Programmierumgebungen auch, fließen die Daten von einem „Knoten“ zum nächsten. Jeder Knoten verrichtet eine bestimmte Aufgabe (Knoten sind Funktionen) und gibt sein Ergebnis an den nächsten weiter.

### Beispiel:

1. Erstellen wir einen `rect` Knoten.

![](assets/basics_1.png)

2. Verbinden wir einen `colorize` Knoten mit dem `rect` Knoten. Dies verändert das Resultat, es ist nun eingefärbt.

![](assets/basics_2.png)

3. Anschließend fügen wir einen `rotate` Knoten hinzu, dieser dreht die Form um einen Punkt.

![](assets/basics_3.png)

Wir Können jeden einzelnen Schritt nachvollziehen, indem wir mit einem Doppelklick den aktiven Knoten (der sog. „Render-Knoten“) wechseln:

![](assets/basics_render.gif)

[Live Beispiel ansehen](https://nodebox.live/nodebox-intro/b00knoten)

### Render-Node (aktiver Knoten) und Debugging (Fehlersuche)

Der aktive Render-Knoten bestimmt was in der Ansicht ausgegeben wird. Im Beispiel oben ist das das Rechteck auf der rechten Seite. Man kann durch das aktivieren der einzelnen Knoten im Knoten-Baum (Netzwerk) Unterergebnisse direkt anschauen. So lassen sich häufig Fehler relativ schnell finden.

## Pins, die Ein- und Ausgänge

Jeder Knoten verarbeitet ein oder mehrere Eingaben (Inputs) um eine Ausgabe (Output) zu erzeugen. Diese Ein- und Ausgänge werden `pins` oder auch `ports` genannt.

  ![](assets/grundlagen_input_output.png)

Alle Eingangs-Ports erwarten Daten eines bestimmten Typus. Jeder Ausgangs-Port gibt ein Ergebnis eines bestimmten Typus zurück. Wenn man über einem Eingang mit der Maus verweilt, wird angezeigt welchen Datentypus der Knoten an diesem Port erwartet. Wenn man über dem Ausgang mit der Maus verweilt, erscheint der Datentypus des Ergebnisses des Knotens.

  ![](assets/grundlagen_input_art.png)

Da Knoten im Grunde Funktionen sind, kann man die Pins/Ports auch als Parameter der Funktion verstehen. Der `rect` Knoten von oben würde dann so aussehen:

```javascript
let rectShape = g.rect( aPoint, widthVal, heightVal, roundnessVal )
```

## Datentypen

Werte, die in NodeBox (oder anderen Umgebungen) verarbeitet und erzeugt werden, haben einen bestimmten Typus, den sog. Datentyp. Eine Zahl könnte bspw. eine `integer` oder `float` sein, ein Text wäre ein `string`, eine Form bspw. ein `shape`.

Die Datentypen, also die unterschiedlichen Arten von Daten, erweitern die bereits in [JavaScript verfügbaren Datentypen](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures).

Die Datentypen an den Ports werden in der Regel durch Farben codiert, die sowohl die Farbe der Ports als auch der „Kabel“ (Verbindungen zw. zwei Knoten) bestimmt.

### Zahlen

![#5DA5DA](https://placehold.it/15/5DA5DA?text=+) Nummern sind sowohl ganzzahlige Werte, genannt `integer` (z.B.: `1`, `5`, `72`, usw.), als auch Zahlen mit Nachkommastellen, genannt `float` (von „Fließkommazahlen; z.B.: `0.25`, `1.678`, `3.333`, usw.).

	- `float` werden benutzt um um z.B. die Breite / Höhe eine Objekts zu verändern.
	- `integer` werden benutzt um Mengen anzugeben also z.B. 10 Kopien im `copy` Knoten

### Points

![#60BD68](https://placehold.it/15/60BD68?text=+) `point`s sind zweidimensionale Punkte, die `x` und `y` Koordinaten enthalten (`y` wird nach oben positiv, `x` nach rechts). Sie können benutzt werden um ein Ort festzulegen z.B. die Position eines Rechtecks, den Ursprung einer Skalierung im `scale` Knoten oder den Dreh- und Angelpunkt eines `rotate` Knoten (also den Punkt um den rotiert werden soll).

### Shapes

![#E8AA00](https://placehold.it/15/E8AA00?text=+) `shape`s (Formen) enthalten Informationen über Kurven, Linien und Punkte. Alle visuellen Elemente od. Formen sind Shapes, also jedes Rechteck, jeder Kreis, jede Linie, …, Buchstaben, Polygone, etc.

### Strings

![#F17CB0](https://placehold.it/15/F17CB0?text=+) `string`s (Zeichenketten) enthalten unformattierten Text.

### Farben

![#DECF3F](https://placehold.it/15/DECF3F?text=+) `color`s enthalten Farbwerte in der Form von \[Rot / Grün / Blau / Alpha\] (`rgbColor`) oder \[Farbton / Sättigung / Helligkeit / Alpha\] (`hsbColor`) Werten. Sie werden benutzt um Farbwerte zu definieren: z.B die Füllfarbe eines Objekts oder auch deren Kontur (Outline).

### Listen / Arrays

![#B276B2](https://placehold.it/15/B276B2?text=+) `array`s sind Sammlungen von Daten (Listen) und können deshalb unterschiedliche Datentypen wie bspw. `number` `point`, `shape` oder `color` enthalten. Deshalb können sie auch mit Eingängen verbunden werden, die einen anderen Typ erwarten. d.h. solange die Liste aus Zahlen besteht, kann sie auch mit dem ![#5DA5DA](https://placehold.it/15/5DA5DA?text=+) `number`-Eingang verbunden werden. Manche Ports erwarten sogar, dass die Werte als Liste eingehen oder liefern Listen als Ausgabewert.

## Listenverarbeitung

> **`/!\`** TODO! Sollte auf eine eigene Seite …

---

Weiter zu [01 – Interface](01-interface.md) oder zur [Übersicht](readme.md)
