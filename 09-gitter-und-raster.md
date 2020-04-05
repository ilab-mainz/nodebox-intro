# Gitter, Raster, Ordnung

In NodeBox gibt es verschiedene Wege Ordnung zu schaffen. Prominentester Knoten ist dabei der `grid` Knoten. Aber auch mittels `stack` und anderer Knoten können interessante Layouts erzeugt werden.

Da viele der Knoten mit Listen von Elementen arbeiten, oder Listen generieren, ist es wichtig sich zuvor nochmals die [Dokumentation zu Listen](00-grundlagen.md) durch zu lesen.

## In Reih' und Glied

Viele Raster lassen sich als verschachtelte Sequenzen verstehen. Ein Objekt wird in eine Richtung vervielfältigt und die so entstandene Reihe wird dann in eine andere Richtung dupliziert. In NodeBox gibt es zwei Knoten, mit denen man einfach Sequenzen herstellen kann: [`range`](https://nodebox.live/reference/range) und [`sample`](https://nodebox.live/reference/sample).

Der Unterschied zwischen den beiden ist, dass bei `range` die Abstände zwischen den zu erzeugenden Werten angegeben werden und bei `sample` die Anzahl der Werte.

## Der Raster Knoten

Mit dem [`grid` Knoten](https://nodebox.live/reference/grid) lassen sich rechtwinklige Raster erzeugen. Die Raster entstehen, indem der Knoten eine Liste von 2D Koordinaten (Punkten) erzeugt, die dann als Ursprung für andere Formen eingesetzt werden können: [Beispiel](https://nodebox.live/reference/grid).

Ebenfalls auf dem Konzept eines recheckigen Rasters aufbauend, erlaubt es der [`snap` Knoten](https://nodebox.live/reference/snap) gegebene Formen od. Punkte mehr oder weniger in ein Raster zu zwängen: [Beispiel](https://nodebox.live/reference/snap).

Das besondere hierbei ist, dass die Formen von ihrer aktuellen Position aus zur nächstgelegenen Rasterpunkt transformiert werden. Leider sind die Standart-Werte des Knotes nicht gut gewählt. Der Pin `strength` erwartet Werte zwischen `0` (keine Anziehung / Effekt) und `1` (volle Anziehung). Dazwischen interpoliert er zwischen der aktuellen Position der Form und dem nächstgelegenen Rasterpunkt. `0.5` wäre also die halbe Strecke dazwischen.

## Wohlgeordnet nebeneinander

Mit dem [`stack` Knoten](https://nodebox.live/reference/stack) lassen sich die Formen in einer Liste in die vier Himmelsrichtungen „aufeinander stapeln“, dabei werden sie nebeneinander ausgerichtet. Über den Pin `margin` kann man dabei die Abstände zwischen den Elementen bestimmen. Zu beachten ist, dass die Elemente dabei an ihrer Mittelachse ausgerichtet werden.

Der [`shapeSort` Knoten](https://nodebox.live/reference/shapeSort) erlaubt es die Elemente einer Liste nach bestimmten geometrischen Bezügen zu einem Ursprung oder zueinander zu sortieren. Verändert wird dabei nur die Reihenfolge der Formen in der gegebenen Liste. Der Pin `orderBy` nimmt vier verschiedene Arten der Sortierung an: `No Change`, `X`, `Y`, `Angle`, `Distance`. Dabei sortieren die Einstellungen X/Y jeweils nach horizontaler oder vertikaler Position (X == Nord-Westen nach Süd-Osten, Y == West-Norden nach Ost-Westen). `Angle` sortiert nach dem Winkel zu dem an Pin `point` gegebenen Punkt und `Distance` nach Abstand zu diesem Punkt.

Ebenfalls in die Gruppe der Ordentlichen gehört der [`align` Knoten](https://nodebox.live/reference/align). Er erlaubt es, wie es der Name schon verrät, Formen an einer oder mehreren Achsen auszurichten.

Als letztes sei in dieser Gruppe noch der [`copy` Knoten](https://nodebox.live/reference/copy) erwähnt, er vervielfältigt gegebene Elemente mit zusätzlicher Transformation (Verschiebung, Rotation, Skalierung). Man kann diesen Knoten gut verwenden, um die zuvor erzeugten Reihen aus `stack` oder `align` zu einem Raster zu vervielfältigen.

## Aus nah und fern

Betrachtet man die Bildpunkte eines Bildschirms aus der Nähe, so erkennt man, dass diese aus einzelnen Farbflecken bestehen, den Pixeln (kurz für „picture element“). Mit dem [`import` Knoten](https://nodebox.live/reference/importRef) ist es möglich Pixel-Bilder in NodeBox zu importieren und dort mit einem kleinen Code als Farben auszulesen: siehe [Beispiel `pixelGrid`](https://nodebox.live/reference/importRef).

## Ausblick: bricks, packing, etc.

Das Thema Gitter, Raster, Ordnung ist natürlich endlos, da wir Menschen so einen starken Drang verspüren uns die Welt dadurch etwas klarer zu gestalten. Daher nachfolgend noch ein paar Links in andere Felder, in denen man weitere Themen und Anregungen entdecken kann.

Mit dieser [NodeBox Library (meint Bibliothek/Erweiterung) von Martin Schneider](https://nodebox.live/bitcraftlab/gridExample01) ist es möglich nicht-rechteckige, also beispielsweise hexagonale oder auf gleichseitigen Dreiecken aufbauende Raster zu erzeugen.

Im Internet findet man zahlreiche JavaScripte, mit denen es einfach möglich wird viele Elemente auf einer Webseite in unterschiedlicher Weise anzuordnen. Diese sind entstanden, da der Layout-Mechanismus des Browsers lange Zeit nur ein einfaches Ausrichten in Zeilen unterstützt hat. Will man unterschiedlich große Elemente nebeneinander zeigen, so ergaben sich dabei oft unvorteilhafte Weissräume. Inzwischen ist allerdings mit den CSS-Layout-Mechanismen [Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) und [Grid](https://css-tricks.com/snippets/css/complete-guide-grid/) hier Abhilfe geschaffen. Nichts desto trotz macht es Spass und ist inspirierend, sich die folgenden Lösungen mal anzuschauen: [Masonry](https://masonry.desandro.com/), [Muuri](https://haltu.github.io/muuri/), [Gridstack](https://gridstackjs.com/), [Gridifier](http://gridifier.io/), [Minigrid](https://minigrid.js.org/), [Isotype](https://isotope.metafizzy.co/), [Packery](https://packery.metafizzy.co/), ...

In der Mathematik und Informatik gibt es eine Reihe von Fragestellungen und Lösungen, die sich mit den sog. Packing Problemen beschäftigen. Hierbei geht es bspw. um die Frage der optimalen Anordnung von Elementen in einer gegebenen Fläche. Dies kann bspw. Anwendung im Transport (was passt in den Laster?) oder der Herstellung (wieviele T-Shirts aus meinem Stoff?) von Waren finden. Bekannteste Formen beschäftigen sich mit dem Platzieren von Rechtecken (Bin Packing [1](http://incise.org/2d-bin-packing-with-javascript-and-canvas.html), [2](https://codeincomplete.com/articles/bin-packing/)) und Kreisen ([Circle Packing](https://snorpey.github.io/circlepacker/continuous.html)).

---

Weiter zur [10 – Libraries Einleitung](10-libraries.md) oder zur [Übersicht](readme.md)
