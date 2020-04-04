# Gitter & Raster

In NodeBox gibt es verschiedene Wege Ordnung zu schaffen. Prominentester Knoten ist dabei der `grid` Knoten. Aber auch mittels `stack` und anderer Knoten können interessante Layouts erzeugt werden.

Da viele der Knoten mit Listen von Elementen arbeiten, oder Listen generieren, ist es wichtig sich zuvor nochmals die [Dokumentation zu diesen](00-grundlagen.md) `XXX -- bessere Doku??? -- XXX` durch zu lesen.

## In Reih' und Glied

Viele Raster lassen sich als verschachtelte Sequenzen verstehen. Ein Objekt wird in eine Richtung vervielfältigt und die so entstandene Reihe wird dann in eine andere Richtung dupliziert. In NodeBox gibt es zwei Knoten, mit denen man einfach Sequenzen herstellen kann: [`range`](https://nodebox.live/reference/range) und [`sample`](https://nodebox.live/reference/sample).

Der Unterschied zwischen den beiden ist, dass bei `range` die Abstände zwischen den zu erzeugenden Werten angegeben werden und bei `sample` die Anzahl der Werte.

## Der Raster Knoten a.k.a. `grid`

Mit dem [`grid` Knoten](https://nodebox.live/reference/grid) lassen sich rechtwinklige Raster erzeugen. Die Raster entstehen, indem der Knoten eine Liste von 2D Koordinaten (Punkten) erzeugt, die dann als Ursprung für andere Formen eingesetzt werden können: [Beispiel](https://nodebox.live/reference/grid).

- grid

Ebenfalls auf dem Konzept eines recheckigen Rasters aufbauend, erlaubt es der [`snap` Knoten](https://nodebox.live/reference/snap) gegebene Formen od. Punkte mehr oder weniger in ein Raster zu zwängen: [Beispiel](https://nodebox.live/reference/snap).

Das besondere hierbei ist, dass die Formen von ihrer aktuellen Position aus zur nächstgelegenen Rasterpunkt transformiert werden. Leider sind die Standart-Werte des Knotes nicht gut gewählt. Der Pin `strength` erwartet Werte zwischen `0` (keine Anziehung / Effekt) und `1` (volle Anziehung). Dazwischen interpoliert er zwischen der aktuellen Position der Form und dem nächstgelegenen Rasterpunkt. `0.5` wäre also die halbe Strecke dazwischen.

## Wohlgeordnet am Fließband oder im Stapel

- stack
- shapeSort

## Ausblick: bricks, packing, etc.

---

Weiter zur [10 – Libraries Einleitung](10-libraries.md) oder zur [Übersicht](readme.md)
