# Interface

*Arbeiten mit [nodebox.live](http://nodebox.live)*

 ![](assets/screenshot-nodebox-live.png)
 
 Das Bedienfenster eines geöffneten Projekts hat im Grunde 5 Bereiche.
 
 1) Den Titel-Balken (hier dunkelgrün) mit dem Namen des Projekts und einem Link zur Projekte-Übersicht (das Logo links) dem Mitteilungsfeld in der Mitte und einem Menu rechts mit globalen Funktionen wie Undo / Redo, Projekt-Einstellungen, Projekt-Export und Hilfe.
 
 2) Darunter Links befindet sich die Funktions-Liste (`Functions`). Funktionen sind im Grunde Unter-Projekte oder -Bereiche des geöffneten Projekts. Man kann hier eigene Knoten anlegen, die dann einen modularen Programmaufbau ermöglichen.
 
 3) Rechts daneben ist das Fenster mit dem Programm-Ablauf (`Network`) zum in der Funktions-Liste gewählten Unterbereich. Dies ist der Hauptarbeitsbereich, in dem man seine Programme erstellt.
 
 4) Neben dem Programm-Ablauf sieht man das Ausgabe-Fenster (`Viewer`). Hier wird das Ergebnis eures Programmes „gerendert“, d.h. in das Fenster gemalt, oder hier ausgegeben (falls es Text o.Ä. ist).
 
 5) Ganz rechts ist die Hilfe (`Help`) zu sehen. Diese lässt sich wie eine kleine Webseite navigieren. Zudem kann man die Hilfe aus den Knoten heraus mit der entsprechenden Hilfeseite zum Knoten öffnen lassen. Die Hilfe ist allerdings nicht immer hilfreich … da sie momentan noch die code-basierte Bibliothek namens [g.js](http://g.js.org/), die hinter NodeBox steht, behandelt.

## Gotchas

[nodebox.live](http://nodebox.live) ist noch in einer frühen Phase (sog. Alphasoftware) und daher nicht fertig und eher experimentell.

### Browser und Systemvoraussetzungen

Aktuell unterstützt nodebox.live vor allem den Chrome Browser in der neuesten Version.

Gerade bei komplexen Projekten kann es dazu kommen, dass der Browser den Computer sehr fordert. Sollte euer Projekt also unglaublich langsam werden … dann probiert mal einen schnelleren Rechner aus.
  
### Bedienung

- zum Zoomen der Arbeitsfläch niemals Pinch oder Zoom-Einstellungen des Browsers benutzen. Das heißt, die Tastenkombination `CTRL + +/-` oder `CMD + +/-` können nicht Zoomen verwendet werden.
	
	![](assets/zoomen_1.gif)
	
- Durch die Sroll-Bewegung kann jedoch mit dem Touchpad ran- und rausgezoomt werden.
	
	![](assets/zoomen_2.gif)
	
- Auf OSX `CMD + 0` in Windows `CTRL + 0` um die Zoom-Stufe des Browsers auf 100% zu setzen. Ebenfalls kann die Maus genutzt werden um rein oder raus zu zoomen.
	
	![](assets/zoomen_3.gif)
	
- Immer einloggen!
	- Sonst geht das Programm verloren
	- [Login-Seite](https://nodebox.live/login)
- Programme regelmässig sichern!

## Neues Programm erstellen 

- Programm ID

	![](assets/newproject_1.png)
	
	![](assets/newproject_2.png)
	
- Programm Name und Farbe können direkt im Programm selbst beim Einstellungssymbol nach Wünsch verändert werden.

	![](assets/änderung.gif)

- Das Programm sicher von selbst solange man mit dem Internet verbunden ist. Dies lässt sich immer an der Anzeige kontrollieren.

	![](assets/project_saved.png)

## Programm sichern & wiederherstellen

- JSON-Quellcode
- Quellcode runterladen (aktuelle Version sichern)
	- mit dem Browser
- Quellcode hochladen (alte Version wiederherstellen)
	- mit dem Brower
	
	![](assets/raw.gif)

## Programme klauen

- Nur für Fortgeschrittene ;-)
	- Quellcode kopieren
	- Suchen + Ersetzen des Programm-Namens

