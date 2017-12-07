# Animation

*Animationen fürs Web und Animierte Gifs mit Nodebox.live*

## So geht's

- Screenshot Interface
- Animation abspielen
- Export als animiertes GIF

## Animations-Knoten

- Frame-basiert vs. Echtzeit
   - Aktueller Frame: `frame`
   - Sekunden seit Start:`eleapsedSeconds`

- Wellenfuntionen
	- Sinus
	- Dreieck
	- Sägezahn
	- Rechteck

## Gotchas

- Für zyklische GIFs muss die Phase muss ein Teiler der Framezahl sein.
- bei 100 Frames z.B. 50, 33, 25, 20, 10 oder 5. 