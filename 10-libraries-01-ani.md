# Animation Library

Animation und Easing

## Beispiele

- [AniTest](https://nodebox.live/bitcraftlab/aniTest)
- [9 Squares Example](https://nodebox.live/bitcraftlab/nineSquares02)

![](assets/libraries_ani_test.gif)

## Nodes

### easing

- `time` — aktueller Zeitpunkt
- `start` — minimaler Ouptut
- `end` — maximaler Output
- `duration` — Dauer der Animation
- `type`  — Art der Interpolation  (`Linear`, `Sine`, `Cubic`, `Quint`, `Circ`, `Elastic`, `Quad`, `Quart`, `Expo`, `Back`, `Bounce`)
- `direction` — `In`, `Out` oder `InOut` (Vorwärts, Rückwärts, Hin-und-Her)


### looper

Generiert zyklische Werte für animierte Loops.

- `frame` — aktueller Frame
- `period` — Periodenlänge in Frames
- `shift` — Offset (relativ) 0 .. 1
- `min` — minimaler Output
- `max` — maximaler Output
- `direction` — `In`, `Out` oder `InOut` (Vorwärts, Rückwärts, Hin-und-Her)

### metro

Einfaches Metronom für eine vorgegebene Anzahl von Frames.

- `shift` — Offset (relativ) 0 .. 1
- `cycles` — Anzahl der Zyklen
- `direction` — `In`, `Out` oder `InOut` (Vorwärts, Rückwärts, Hin-und-Her)