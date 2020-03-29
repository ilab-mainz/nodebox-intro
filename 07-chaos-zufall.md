# Chaos und Zufall

## Kontrollierter Zufall mit Random Seeds

Fast alle Knoten, die mit Zufall zu tun haben, bieten einen Port (Parameter) namens `seed` an (siehe den [Wikipedia Eintrag](https://de.wikipedia.org/wiki/Seed_key) dazu). Diese Zahl bildet die Basis, auf der der Computer seine pseudo-zufälligen Werte erzeugt. Verändert man diese Basis, entstehen völlig neue Zufallszahlen. `seed` erlaubt es einem also schnell durch viele Varianten hindurch zu „schrubben“: [Beispiel `randomNumbers`](https://nodebox.live/reference/randomNumbers).

Stellt man `seed` auf den gleichen Wert wie zu einem früheren Zeitpunkt, so reproduziert er _genau die gleichen Zufallszahlen_ wie zuvor. Diesen Effekt kann man nutzen um sich „gute Zufallsergebnisse“ zu merken, indem man sich den `seed` dazu notiert.

## Zufalls-Zahlen

Die häufigste Anwendung von Zufall ist in Form von Zufallszahlen, die man mittels `randomNumbers` erzeugen kann.

Häufig werden diese Werte verwendet um Formen zu transformieren, also zu verschieben, skalieren, rotieren, etc. Ein weiterer beliebter Anwendungsfall ist das Erzeugen zufälliger Farben.

[Beispiel `randomNumbers`](https://nodebox.live/reference/randomNumbers)

Ursprünglich in den 1980ern von Ken Perlin entwickelt um realistischere Texturen für 3D Anwendungen zu generieren, ist [„Perlin Noise“](https://de.wikipedia.org/wiki/Perlin-Noise) heute eine Standart-Funktion um 2D und 3D Zufallsflächen und -Volumen zu erzeugen. Dies lässt sich wunderbar für das Generieren von Hügellandschaften oder alle möglichen anderen Strukturen nutzen.

[Beispiel `perlinNoise`](https://nodebox.live/reference/perlinNoise)

## Zufällige Ordnung / Zufall und Listen

Mit dem [`shuffle` Knoten](https://nodebox.live/reference/shuffle) kann man Listen durcheinander würfeln lassen. Dabei werden die Einträge innerhalb der Liste zufällig auf eine andere Position verschoben.

Der [`randomSample` Knoten](https://nodebox.live/reference/randomSample) gibt aus einer Liste ein zufällig gewähltes Element zurück. Denkt man über einen Würfel als Liste der Zahlen [1, 2, 3, 4, 5, 6] nach, so würde `randomSample` dem Vorgang des Würfelns gleich kommen und immer eine der Zahlen erzeugen.

Unter dem Namen [`pick`](https://nodebox.live/reference/pick) ist die gleiche Funktionalität wie `randomSample` nochmals verfügbar.

## Zufalls-Verwandlung

Mit den Knoten `wigglePoints`, `wiggleContours` und `wigglePaths` lassen sich bestehende Formen zufällig verändern. `to wiggle` bedeutet im Englischen „wackeln“, man kann sich also eine Art Durchschütteln der Formen vorstellen.

Mit [`wigglePoints`](https://nodebox.live/reference/wigglePoints) verschiebt man die Vektor-Punkte einer Form zufällig.

Der [Knoten `wigglePaths`](https://nodebox.live/reference/wigglePaths) verschiebt die einzelnen Elemente einer Gruppe von Formen.

Formen, die aus komplexeren Konturen mit Öffnungen bestehen, wie bspw. der Buchstabe „B“, können mit dem [`wiggleContours` Knoten](https://nodebox.live/reference/wiggleContours) durchgerüttelt werden.

---

Weiter zur [08 – Nodes vs. Codes](08-nodes-codes.md) oder zur [Übersicht](readme.md)
