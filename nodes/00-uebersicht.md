# Übersicht aller Knoten (Nodes)

In nodebox.live sind die Knoten thematisch gegliedert. Die Liste aller Knoten öffnet sich, wenn man in die Arbeitsfläche doppel-klickt, oder oben links darüber auf den Link „+ New Node“ klickt, oder mit Rechtsklick das Maus-Kontext-Menu öffnet und dort „New Node“ auswählt.

![](../assets/new-node-interface.png)

Die Kategorien sind:

| *Inhalt* | *Name* | *Beschreibung* |
| ------ | ------ | ------ |
| Farbe | Color | Herstellen, Verändern, Anwenden von Farbe auf Shapes (Formen) |
| Daten | Data | Laden, Aufarbeiten, Konvertieren, Filtern von Daten |
| Geräte | Device | Die Mouse auslesen |
| Geografie | Geo | Verarbeitung von geografischen Daten |
| Grafisches | Graphics | Herstellen, Verändern, Ausrichten von Formen (Shapes) |
| HTML | Html | Schnittstelle zu HTML und dem DOM des Browsers |
| Listen | List | Arbeit mit Listen (Arrays) von Werten |
| Mathematik | Math | Mathematische Methoden und Generatoren von Werten |
| Zustand | State | Speichern und Laden von Zuständen |
| Text | String | Erstellen, Veränderung von Texten |
| Zeit | Time | Auslesen von Zeit und zeitliche Funktionen (Easings) |
| Sonstiges | Uncategorized | ... |

Nachfolgend sind die Knoten der Kategorien aufgelistet und kurz beschrieben.

## Farbe / Color

| ------ | ------ | ------ |
| ------ | ------ | ------ |
| colorize | Change the color of a shape. | <link> |
| grayColor | Create a gray color. | <link> |
| hexColor | Create a color using a hexadecimal value. | <link> |
| hslAdjust | Adjust hue, saturation and lightness of a shape. | <link> |
| hslColor | Create a HSL color. | <link> |
| invert | Invert a color or the colors of a shape. | <link> |
| parseColor | Parse a named or hexadecimal color. | <link> |
| rgbAdjust | Adjust red, green, blue and alpha values of an input object. | <link> |
| rgbColor | Create a RGB color. | <link> |

## Daten / Data

| ------ | ------ | ------ |
| ------ | ------ | ------ |
| addColumn | Add or replace column in existing table. | <link> |
| convert | Convert values from one range to another. | <link> |
| fetchJSON | Perform a HTTP GET request to an API and return the JSON. | <link> |
| filterData | Filter the input data by comparing the columns of each row with a value. | <link> |
| groupBy | Group the data based on key/value. | <link> |
| import | Import data (CSV, SVG) from a file. | <link> |
| keys | Get the keys from a table. | <link> |
| lookup | Look up a value in a table or object. | <link> |
| zipMap | Combine a list of keys and values together in a map. | <link> |

## Geräte / Device

| ------ | ------ | ------ |
| ------ | ------ | ------ |
| mousePosition | Get the current mouse position. | <link> |

## Geografie / Geo

| ------ | ------ | ------ |
| ------ | ------ | ------ |
| geoProject | Project a longitude / latitude to X/Y coordinates. | <link> |

## Grafisches / Graphics

| ------ | ------ | ------ |
| ------ | ------ | ------ |
| align | Align a shape in relation to the origin. | <link> |
| arc | Create an arc, pie or wedge shape. | <link> |
| bounds | Get the bounds of a shape. | <link> |
| centerPoint | Calculate the geometric center point of a shape. | <link> |
| compound | Add, subtract or intersect geometry. | <link> |
| connectPoints | Connect all points in a path. | <link> |
| coordinates | Calculate a new point based on the angle and distance from an original point. | <link> |
| copy | Create multiple copies of a shape. | <link> |
| curve | Create a quadratic curve with one off-curve point. | <link> |
| deletePaths | Delete paths based on a bounding path. | <link> |
| deletePoints | Delete points based on a bounding path. | <link> |
| desaturate | Desaturate a shape. | <link> |
| distance | Calculate the distance between two points. | <link> |
| ellipse | Create an ellipse or circle. | <link> |
| fit | Fit a shape within bounds. | <link> |
| fitTo | Fit a shape to another shape. | <link> |
| flip | Flip a shape or image. | <link> |
| grid | Create a grid of points. | <link> |
| group | Combine multiple shapes together. | <link> |
| line | Create a line between two points. | <link> |
| lineAngle | Create a line between a point and an angle + distance. | <link> |
| link | Generate a visual link between two shapes. | <link> |
| makePoint | Create a point from X/Y coordinates. | <link> |
| mirror | Mirror the geometry around an invisible axis. | <link> |
| pathLength | Get the contour length of the path. | <link> |
| perlinNoise | Compute Perlin noise. | <link> |
| pointOnPath | Calculate a point along the path. | <link> |
| polygon | Create a multi-sided polygon. | <link> |
| quad | Create a four-sided polygon from points. | <link> |
| rect | Create a rectangle or square. | <link> |
| resampleByAmount | Distribute points along a shape by amount. | <link> |
| resampleByLength | Distribute points along a shape by segment length. | <link> |
| rotate | Rotate the shape according to the given angle. | <link> |
| roundedSegments | Convert straight segments of a shape into rounded ones. | <link> |
| scale | Resize the shape by scaling it. | <link> |
| scatterPoints | Generate random points within the boundaries of a shape. | <link> |
| shapeSort | Sort points or shapes using different sorting methods. | <link> |
| skew | Skew the shape. | <link> |
| snap | Snap geometry to a grid. | <link> |
| stack | Arrange shapes in a horizontal or vertical layout. | <link> |
| star | Create a star shape. | <link> |
| textPath | Create a path out of text. | <link> |
| toPoints | Convert the shape to points that make up the shape. | <link> |
| translate | Move the shape, changing its position. | <link> |
| ungroup | Decompose the input group into a list of paths. | <link> |
| wiggleContours | Shift elements of a shape by a random amount. | <link> |
| wigglePaths | Shift paths of a group by a random amount. | <link> |
| wigglePoints | Shift points of the shape by a random amount. | <link> |

## HTML

| ------ | ------ | ------ |
| ------ | ------ | ------ |
| htmlImport | Import a HTML or SVG file as a set of HTML elements. | <link> |
| htmlString | Convert a string of HTML to elements on the page. | <link> |
| htmlWrap | Wrap a list of HTML elements or strings with a tag. | <link> |
| toSVG | Convert one or more shapes to SVG. | <link> |

## Listen / List

| ------ | ------ | ------ |
| ------ | ------ | ------ |
| combine | Combine multiple lists into one. | <link> |
| contains | Determine if the list contains a given value. | <link> |
| count | Count the number of items in the list. | <link> |
| cull | Keep only items from the list where the corresponding boolean is `true`. | <link> |
| cycle | Repeat the items in the list until the new list is of a certain length. | <link> |
| distinct | Remove all duplicate items from a list. | <link> |
| equals | Determine if two objects are equal. | <link> |
| first | Take the first item in the list. | <link> |
| flatten | Recursively flattens an array. | <link> |
| get | Take an item in the list at a certain index. | <link> |
| interleave | Mix multiple lists by alternating between them. | <link> |
| last | Take the last item in the list. | <link> |
| merge | Combine different shapes into one. | <link> |
| pick | Take random items from a list. | <link> |
| repeat | Repeat the items in the list a given number of times. | <link> |
| rest | Take all but the first item in the list. | <link> |
| reverse | Reverse the items in the list. The first item becomes the last and vice versa. | <link> |
| second | Take the second item in the list. | <link> |
| shift | Move items from the beginning of a list to the end of the list. | <link> |
| shuffle | Randomise the ordering of items in the list. | <link> |
| slice | Take a portion of the list. | <link> |
| sort | Sort the items in the list. | <link> |
| switch | Select one of multiple inputs based on an index. | <link> |
| takeEvery | Take every `n`th element of a list. | <link> |

## Mathematik / Math

| ------ | ------ | ------ |
| ------ | ------ | ------ |
| abs | Convert any number to a positive value (the absolute value). | <link> |
| accumulate | Generate in between totals of a list of numbers. | <link> |
| add | Add two numbers. | <link> |
| and | Perform the logical AND operation. | <link> |
| angle | Calculate the angle between two points. | <link> |
| average | Calculate the average of a list of numbers. | <link> |
| boolean | Create a boolean value that can be used as a variable. | <link> |
| ceil | Round up a number to the nearest bigger integer. | <link> |
| clamp | Limit a number between a minimum and maximum. | <link> |
| compare | Return true or false by comparing two values using a comparison operation. | <link> |
| cos | Calculate the trigonometric cosine of an angle. | <link> |
| degrees | Convert an angle specified in radians to degrees. | <link> |
| divide | Divide two numbers. | <link> |
| e | The value of the mathematical constant e, the base of the natural logarithm. | <link> |
| even | Determine if a number is even. | <link> |
| floor | Round down a number to the nearest smaller integer. | <link> |
| integer | Create an integer value that can be used as a variable. | <link> |
| log | Calculate the natural logarithm. | <link> |
| makeNumbers | Transform a string to a list of numbers. | <link> |
| max | Take the largest value from a list of numbers. | <link> |
| min | Take the smallest value from a list of numbers. | <link> |
| mix | Linearly interpolate between two values. | <link> |
| mixList | Linearly interpolate between the values of a list. | <link> |
| mod | Calculate the modulo by dividing two numbers and keeping the remainder. | <link> |
| multiply | Multiply two numbers. | <link> |
| negate | Switch the sign of the input value.  | <link> |
| not | Perform the logical NOT operation. | <link> |
| number | Create a number value. | <link> |
| odd | Determine if a number is odd. | <link> |
| or | Perform the logical OR operation. | <link> |
| pi | The value of the mathematical constant pi. | <link> |
| pow | Raise a number to the given power. | <link> |
| radians | Convert an angle specified in degrees to radians. | <link> |
| randomNumbers | Create a list of random numbers. | <link> |
| randomSample | Take a random sample from a list. | <link> |
| range | Generate a list of numbers between a minimum and maximum. | <link> |
| round | Round off a number to the nearest integer. | <link> |
| sample | Generate numbers within the given bounds. | <link> |
| sawtoothWave | Calculate a value based on a sawtooth wave. | <link> |
| sign | Take the sign of a number. | <link> |
| sin | Calculate the trigonometric sine of an angle. | <link> |
| sineWave | Calculate a value based on a sine wave. | <link> |
| sqrt | Calculate the square root of a number. | <link> |
| squareWave | Calculate a value based on a square wave. | <link> |
| subtract | Subtract two numbers. | <link> |
| tan | Calculate the trigonometric tangens of an angle. | <link> |
| ticks | Generate tick values for use in axes. | <link> |
| total | Calculate the sum of a list of numbers. | <link> |
| triangleWave | Calculate a value based on a triangle wave. | <link> |
| xor | Perform the logical XOR operation. | <link> |

## Zustand / State

| ------ | ------ | ------ |
| ------ | ------ | ------ |
| stateLoad | Load the global state. | <link> |
| stateSave | Save the input into global state. | <link> |

## Text / String

| ------ | ------ | ------ |
| ------ | ------ | ------ |
| characterAt | Output the character at a given index. | <link> |
| concatenate | Add strings together. | <link> |
| endsWith | Check if the string ends with a given string. | <link> |
| startsWith | Check if the string starts with a given string. | <link> |
| string | Create a string value that can be used as a variable. | <link> |
| stringContains | Determine if the string contains a given substring. | <link> |
| stringEquals | Determine if the string equals a given string. | <link> |
| stringLength | Count the number of characters in a string. | <link> |
| stringReplace | Replace part of a string. | <link> |
| stringSplit | Split a string into a list of strings. | <link> |
| stringTemplate | Output a string with placeholders replaced by data. | <link> |
| stringTrim | Remove white space from the start and end of the string. | <link> |
| substring | Take a portion of a string. | <link> |
| text | Create a text element. | <link> |
| toCharacterCodes | Convert a string into a list of character codes. | <link> |
| toCharacters | Create a list of characters from a string. | <link> |
| toLowerCase | Convert a string to lower case (small letters). | <link> |
| toTitleCase | Convert a string to title case. | <link> |
| toUpperCase | Convert a string to upper case (small letters). | <link> |
| toWords | Extract a list of words from a string. | <link> |
| wordCount | Count the number of words in a string. | <link> |

## Zeit / Time

| ------ | ------ | ------ |
| ------ | ------ | ------ |
| easing | Calculate a value based on an easing function. | <link> |
| elapsedSeconds | Get the number of seconds since the start of the animation. | <link> |
| frame | Get the current frame number. | <link> |

## Sonstiges / Uncategorized

| ------ | ------ | ------ |
| ------ | ------ | ------ |
| looper | ... | <link> |
| metro | ... | <link> |
| teasing | teasing function to interpolate between two values over time. | <link> |

## Alle in alphabetischer Reihenfolge

| ------ | ------ | ------ |
| ------ | ------ | ------ |
| abs | Convert any number to a positive value (the absolute value). | <link> |
| accumulate | Generate in between totals of a list of numbers. | <link> |
| add | Add two numbers. | <link> |
| addColumn | Add or replace column in existing table. | <link> |
| align | Align a shape in relation to the origin. | <link> |
| and | Perform the logical AND operation. | <link> |
| angle | Calculate the angle between two points. | <link> |
| arc | Create an arc, pie or wedge shape. | <link> |
| average | Calculate the average of a list of numbers. | <link> |
| boolean | Create a boolean value that can be used as a variable. | <link> |
| bounds | Get the bounds of a shape. | <link> |
| ceil | Round up a number to the nearest bigger integer. | <link> |
| centerPoint | Calculate the geometric center point of a shape. | <link> |
| characterAt | Output the character at a given index. | <link> |
| clamp | Limit a number between a minimum and maximum. | <link> |
| colorize | Change the color of a shape. | <link> |
| combine | Combine multiple lists into one. | <link> |
| compare | Return true or false by comparing two values using a comparison operation. | <link> |
| compound | Add, subtract or intersect geometry. | <link> |
| concatenate | Add strings together. | <link> |
| connectPoints | Connect all points in a path. | <link> |
| contains | Determine if the list contains a given value. | <link> |
| convert | Convert values from one range to another. | <link> |
| coordinates | Calculate a new point based on the angle and distance from an original point. | <link> |
| copy | Create multiple copies of a shape. | <link> |
| cos | Calculate the trigonometric cosine of an angle. | <link> |
| count | Count the number of items in the list. | <link> |
| cull | Keep only items from the list where the corresponding boolean is `true`. | <link> |
| curve | Create a quadratic curve with one off-curve point. | <link> |
| cycle | Repeat the items in the list until the new list is of a certain length. | <link> |
| degrees | Convert an angle specified in radians to degrees. | <link> |
| deletePaths | Delete paths based on a bounding path. | <link> |
| deletePoints | Delete points based on a bounding path. | <link> |
| desaturate | Desaturate a shape. | <link> |
| distance | Calculate the distance between two points. | <link> |
| distinct | Remove all duplicate items from a list. | <link> |
| divide | Divide two numbers. | <link> |
| e | The value of the mathematical constant e, the base of the natural logarithm. | <link> |
| easing | Calculate a value based on an easing function. | <link> |
| elapsedSeconds | Get the number of seconds since the start of the animation. | <link> |
| ellipse | Create an ellipse or circle. | <link> |
| endsWith | Check if the string ends with a given string. | <link> |
| equals | Determine if two objects are equal. | <link> |
| even | Determine if a number is even. | <link> |
| fetchJSON | Perform a HTTP GET request to an API and return the JSON. | <link> |
| filterData | Filter the input data by comparing the columns of each row with a value. | <link> |
| first | Take the first item in the list. | <link> |
| fit | Fit a shape within bounds. | <link> |
| fitTo | Fit a shape to another shape. | <link> |
| flatten | Recursively flattens an array. | <link> |
| flip | Flip a shape or image. | <link> |
| floor | Round down a number to the nearest smaller integer. | <link> |
| frame | Get the current frame number. | <link> |
| geoProject | Project a longitude / latitude to X/Y coordinates. | <link> |
| get | Take an item in the list at a certain index. | <link> |
| grayColor | Create a gray color. | <link> |
| grid | Create a grid of points. | <link> |
| group | Combine multiple shapes together. | <link> |
| groupBy | Group the data based on key/value. | <link> |
| hexColor | Create a color using a hexadecimal value. | <link> |
| hslAdjust | Adjust hue, saturation and lightness of a shape. | <link> |
| hslColor | Create a HSL color. | <link> |
| htmlImport | Import a HTML or SVG file as a set of HTML elements. | <link> |
| htmlString | Convert a string of HTML to elements on the page. | <link> |
| htmlWrap | Wrap a list of HTML elements or strings with a tag. | <link> |
| import | Import data (CSV, SVG) from a file. | <link> |
| integer | Create an integer value that can be used as a variable. | <link> |
| interleave | Mix multiple lists by alternating between them. | <link> |
| invert | Invert a color or the colors of a shape. | <link> |
| keys | Get the keys from a table. | <link> |
| last | Take the last item in the list. | <link> |
| line | Create a line between two points. | <link> |
| lineAngle | Create a line between a point and an angle + distance. | <link> |
| link | Generate a visual link between two shapes. | <link> |
| log | Calculate the natural logarithm. | <link> |
| lookup | Look up a value in a table or object. | <link> |
| looper |  | <link> |
| makeNumbers | Transform a string to a list of numbers. | <link> |
| makePoint | Create a point from X/Y coordinates. | <link> |
| max | Take the largest value from a list of numbers. | <link> |
| merge | Combine different shapes into one. | <link> |
| metro |  | <link> |
| min | Take the smallest value from a list of numbers. | <link> |
| mirror | Mirror the geometry around an invisible axis. | <link> |
| mix | Linearly interpolate between two values. | <link> |
| mixList | Linearly interpolate between the values of a list. | <link> |
| mod | Calculate the modulo by dividing two numbers and keeping the remainder. | <link> |
| mousePosition | Get the current mouse position. | <link> |
| multiply | Multiply two numbers. | <link> |
| negate | Switch the sign of the input value.  | <link> |
| not | Perform the logical NOT operation. | <link> |
| number | Create a number value. | <link> |
| odd | Determine if a number is odd. | <link> |
| or | Perform the logical OR operation. | <link> |
| parseColor | Parse a named or hexadecimal color. | <link> |
| pathLength | Get the contour length of the path. | <link> |
| perlinNoise | Compute Perlin noise. | <link> |
| pi | The value of the mathematical constant pi. | <link> |
| pick | Take random items from a list. | <link> |
| pointOnPath | Calculate a point along the path. | <link> |
| polygon | Create a multi-sided polygon. | <link> |
| pow | Raise a number to the given power. | <link> |
| quad | Create a four-sided polygon from points. | <link> |
| radians | Convert an angle specified in degrees to radians. | <link> |
| randomNumbers | Create a list of random numbers. | <link> |
| randomSample | Take a random sample from a list. | <link> |
| range | Generate a list of numbers between a minimum and maximum. | <link> |
| rect | Create a rectangle or square. | <link> |
| repeat | Repeat the items in the list a given number of times. | <link> |
| resampleByAmount | Distribute points along a shape by amount. | <link> |
| resampleByLength | Distribute points along a shape by segment length. | <link> |
| rest | Take all but the first item in the list. | <link> |
| reverse | Reverse the items in the list. The first item becomes the last and vice versa. | <link> |
| rgbAdjust | Adjust red, green, blue and alpha values of an input object. | <link> |
| rgbColor | Create a RGB color. | <link> |
| rotate | Rotate the shape according to the given angle. | <link> |
| round | Round off a number to the nearest integer. | <link> |
| roundedSegments | Convert straight segments of a shape into rounded ones. | <link> |
| sample | Generate numbers within the given bounds. | <link> |
| sawtoothWave | Calculate a value based on a sawtooth wave. | <link> |
| scale | Resize the shape by scaling it. | <link> |
| scatterPoints | Generate random points within the boundaries of a shape. | <link> |
| second | Take the second item in the list. | <link> |
| shapeSort | Sort points or shapes using different sorting methods. | <link> |
| shift | Move items from the beginning of a list to the end of the list. | <link> |
| shuffle | Randomise the ordering of items in the list. | <link> |
| sign | Take the sign of a number. | <link> |
| sin | Calculate the trigonometric sine of an angle. | <link> |
| sineWave | Calculate a value based on a sine wave. | <link> |
| skew | Skew the shape. | <link> |
| slice | Take a portion of the list. | <link> |
| snap | Snap geometry to a grid. | <link> |
| sort | Sort the items in the list. | <link> |
| sqrt | Calculate the square root of a number. | <link> |
| squareWave | Calculate a value based on a square wave. | <link> |
| stack | Arrange shapes in a horizontal or vertical layout. | <link> |
| star | Create a star shape. | <link> |
| startsWith | Check if the string starts with a given string. | <link> |
| stateLoad | Load the global state. | <link> |
| stateSave | Save the input into global state. | <link> |
| string | Create a string value that can be used as a variable. | <link> |
| stringContains | Determine if the string contains a given substring. | <link> |
| stringEquals | Determine if the string equals a given string. | <link> |
| stringLength | Count the number of characters in a string. | <link> |
| stringReplace | Replace part of a string. | <link> |
| stringSplit | Split a string into a list of strings. | <link> |
| stringTemplate | Output a string with placeholders replaced by data. | <link> |
| stringTrim | Remove white space from the start and end of the string. | <link> |
| substring | Take a portion of a string. | <link> |
| subtract | Subtract two numbers. | <link> |
| switch | Select one of multiple inputs based on an index. | <link> |
| takeEvery | Take every `n`th element of a list. | <link> |
| tan | Calculate the trigonometric tangens of an angle. | <link> |
| teasing | teasing function to interpolate between two values over time. | <link> |
| text | Create a text element. | <link> |
| textPath | Create a path out of text. | <link> |
| ticks | Generate tick values for use in axes. | <link> |
| toCharacterCodes | Convert a string into a list of character codes. | <link> |
| toCharacters | Create a list of characters from a string. | <link> |
| toLowerCase | Convert a string to lower case (small letters). | <link> |
| toPoints | Convert the shape to points that make up the shape. | <link> |
| toSVG | Convert one or more shapes to SVG. | <link> |
| toTitleCase | Convert a string to title case. | <link> |
| toUpperCase | Convert a string to upper case (small letters). | <link> |
| toWords | Extract a list of words from a string. | <link> |
| total | Calculate the sum of a list of numbers. | <link> |
| translate | Move the shape, changing its position. | <link> |
| triangleWave | Calculate a value based on a triangle wave. | <link> |
| ungroup | Decompose the input group into a list of paths. | <link> |
| wiggleContours | Shift elements of a shape by a random amount. | <link> |
| wigglePaths | Shift paths of a group by a random amount. | <link> |
| wigglePoints | Shift points of the shape by a random amount. | <link> |
| wordCount | Count the number of words in a string. | <link> |
| xor | Perform the logical XOR operation. | <link> |
| zipMap | Combine a list of keys and values together in a map. | <link> |
