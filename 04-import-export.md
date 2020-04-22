# Import-Export, Sharing

Ein Werkzeug für die Gestaltung ist natürlich nur so gut, wie es sich in Gestaltungsprozesse integrieren lässt. NodeBox.live ist zwar eine „Web-Anwendung“, läuft also als Webseite im Internet, kann aber dennoch Dateien laden und speichern. Genauer gesagt importieren und exportieren.

Ein weiterer Bereich ist das „Sharing“, also die Möglichkeit NodeBox Projekte mit anderen zu teilen. Dies ist ein Feature, das sich primär in online Tools findet und auch NB bietet dies an.

## Import ⇄ Export

Die wichtigsten **Eingangs-Formate** für NodeBox sind:

- SVG, „scaleable vector graphics“, das sind Dateien, die Pfadinformationen enthalten und für den Austausch mit Verktor-Software wie Illustrator oder InkScape geeignet sind.

- CSV

- Bilder im JPG und PNG Format

- Fonts (??)



**Ausgeben** kann man Grafiken aus NodeBox in den Formaten:

- SVG, s.o.

- GIF

- Bilder und Videos ... dazu kann man einfach einen Screenshot / -Recording machen 😉
  
  - Auf dem Mac geht das sehr einfach mit QuickTime, auf dem PC kann man leicht eine Software dafür finden, bspw. Camtasia, etc.



### SVGs, Fonts und Grafiken importieren

Der wichtigste Knoten für den Import von Materialien nach NodeBox ist `import` ([Beispiel](https://nodebox.live/reference/importRef)). Beim Import sind allerdings einige Aspekte zu beachten.

1) Importierte Dateien liegen bei NodeBox auf einem öffentlich zugänglichen Server, sie sind also von jedermann aufrufbar und können auch herunter geladen werden. Private Dateien und sensible Daten sollte man so also nicht einsetzen.

2) Da die Daten für jedermann zugänglich sind, gilt hier auch besondere Vorsicht bei der Verwendung von Material aus fremden Quellen. Die Verwendung gilt als Veröffentlichung und damit muss man Urheberrechte, Copyright, etc. beachten.

3) NodeBox rechnet Bilder und andere Materialien nicht um, d.h. man muss diese schon möglichst für ihren Einsatz optimiert hochladen.
   (→ hier fehlt ein Link zu den Hinweisen dazu)



### SVGs aus Illustrator

**Vor dem Export**

Um zu vermeiden, dass irgentwelche unerwünschten Pfade im SVG landen, starten wir zuerst mit einer neuen Datei. Dabei ist zu achten, dass die Datei in Pixeln und im RGB Modus ist:



  ![](assets/import_neue_datei.png)



Nodebox kann nicht gut mit großen Dateien umgehen. Am einfachsten können wir deswegen unsere Zeichnung mit `Objekt > Pfad > vereinfachen…` optimieren, indem wir Pfadpunkte reduzieren.

  ![](assets/import_vereinfachen.png)

NodeBox übernimmt nicht die Stil-Einstellungen (Farben, Linien-Stärken, etc.) der importierten SVG-Zeichnungen. Die Idee ist dass man vor allem „Formen“ importiert, weniger ausgearbeitete „Illustrationen“.


Um unerwünschte Nebeneffekte zu vermeiden, kann man Linien in der Zeichnung vor dem Export in Flächen umwandeln. So bleibt die Linienstärke erhalten.

![](assets/pinsel_werkzeug_1.png)  



Schrift sollte man ebenfalls in Pfade umwandeln.



Die Färbung von Formen geht beim Import verloren, wie im folgenden Beispiel ersichtlich.

![](assets/rechteck_werkzeug_2.png)
![](assets/rechteck_werkzeug_3.png)



Hat man die Zeichnung für den Export aus der Zeichen-Software optimiert, so kann man diese in eine Datei speichern. In Illustrator kann man dazu über den Weg „Exportieren“ oder „Als Kopie speichern“ gehen. In beiden Fällen wählt man SVG als Datentyp (nicht SVGz) und stellt in den Einstellungen SVG-1.0 ohne die zusätzlichen „Illustrator-Bearbeitungsfunktionen beibehalten“ ein.



- `Datei > Speicher unter …` 

- Im nächsten Fenster bei Format `SVG (svg)` auswählen. Und **kein** Haken bei „Zeichenflächen benutzen“ setzen

- Im Nächsten Fenster ist besonders `SVG 1.0` wichtig. Eventuell müssen auch die anderen Einstellungen angepasst werden.
  
  

![](assets/import_export_einstellungen.png)



Beim Dateinamen sollte man darauf achten, dass er eine Art Versionierung enthällt, da NodeBox Dateien beim Hochladen nur ersetzt, wenn diese einen neuen Namen haben (sonst bekommt man trotz löschen und „überschreiben“ die alte Zeichnung). (→ Bug oder Feature?)



Ist die Datei erstellt, so kann man mit dem `import` Knoten die Datei in NodeBox laden:

- `import` Knoten anlegen

- Die Einstellungen für den Knoten öffnen und am Pin `file` rechts auf `Select file` klicken

- Im sich öffnenden Dialog auf `Upload` klicken ... die Datei lädt hoch

- Die hochgeladene Datei in der Liste anklicken, um sie in den `file`-Pin aufzunehmen 
  
  

![](assets/import_node.gif)



Lädt man eine CSV oder Text-Datei hoch, so kann man am zweiten Pin einstellen, ob die evtl. enthaltenen Daten mit einem Komma oder einem anderen Zeichen getrennt sind. Ein Beispiel für CSV-Daten (Komma-separierte Werte) könnte so aussehen:

```
Name,Passwort,Alter,Email
Florian,admin123,99,florian@motionbank.org
Petra,xxpetra,22,petra@yourhoster.tdl
```



# Assets aus dem Netz laden

- Etwa für Live-Datenvisualisierung
- Mit Javascript möglich
- Siehe auch `net` library

## Animierte Gifs exportieren

- Frames
- Größe
- Weiterverarbeiten
- Verbreiten und teilen

## SVGs exportieren

- Screenshot

## Fonts exportieren

- Theoretisch möglich dank opentype.js
- Coming soon ...

---

Weiter zur [05 - Punkt und Linie](05-punkt-und-linie.md) oder zur [Übersicht](readme.md)
