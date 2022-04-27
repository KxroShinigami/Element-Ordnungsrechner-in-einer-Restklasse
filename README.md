# Ordnungsrechner in einer Einheitengruppe

## Inhaltsverzeichnis
+ [Beschreibung](#beschreibung)
+ [Installation](#installation)
+ [Verwendung](#verwendung)

## Beschreibung
Der Ordnungsrechner berechnet die Ordnung eines Elements von einer Restklasse in einer Gruppe mit entweder einer additiven oder multiplikativen Verknüpfung.
Für eine weitere Erläuterung einer Ordnung eines Gruppenelements, siehe: [Ordnung eines Gruppenelements, Wikipedia](https://de.wikipedia.org/wiki/Ordnung_eines_Gruppenelementeshttps://de.wikipedia.org/wiki/Ordnung_eines_Gruppenelementes)

![Ordnungsdefinition](https://wikimedia.org/api/rest_v1/media/math/render/svg/3c163afaa8f541e4aea6ffec4d41636b92c960d8)

## Installation
Man kann entweder Python auf dem eigenen Computer installieren und das Programm herunterladen und ausführen, oder man nutzt einen [Online Python Compiler](https://www.online-python.com)

Folgende Beispiele wurden mit dem Online Python Compiler erzeugt.

### Beispiel 1: Exception Handling & Eingabeüberprüfung
```
Bitte geben Sie eine gültige Ganzzahl ein.

Modulo n der Restklasse: 
abc



Fehlercode:  invalid literal for int() with base 10: 'abc'

Bitte geben Sie eine gültige Ganzzahl ein.

Modulo n der Restklasse: 
123

Bitte geben Sie eine gültige Ganzzahl ein.

Element g, deren Ordnung bestimmt werden muss: 
abc



Fehlercode:  invalid literal for int() with base 10: 'abc'

Bitte geben Sie eine gültige Ganzzahl ein.

Element g, deren Ordnung bestimmt werden muss: 
123

Bitte geben Sie eine gültige Verknüpfung (+, *, Beide) ein.

Verknüpfung, welche in der Gruppe herrscht: 
-

Bitte geben Sie eine gültige Verknüpfung (+, *, Beide) ein.

Verknüpfung, welche in der Gruppe herrscht: 
*

Multiplikative Verknüpfung

Teileranzahl:  4
Die Teiler sind:  [1, 2, 61, 122]



Bei der Berechnung der Ordnung ist entweder ein Fehler unterlaufen oder es kann keine Ordnung für dieses Element in dem Körper mit einer multiplikativen Verknüpfung berechnet werden. Überprüfen Sie ihre Eingabe oder kontaktieren Sie den Hersteller


** Process exited - Return Code: 0 **
```

### Beispiel 2: Additive Verknüpfung
```
Bitte geben Sie eine gültige Ganzzahl ein.

Modulo n der Restklasse: 
100

Bitte geben Sie eine gültige Ganzzahl ein.

Element g, deren Ordnung bestimmt werden muss: 
2

Bitte geben Sie eine gültige Verknüpfung (+, *, Beide) ein.

Verknüpfung, welche in der Gruppe herrscht: 
+

Additive Verknüpfung


Die Ordnung des Elements  2  in der Restklasse  100  mit der additiven Verknüpfung ist:  50


** Process exited - Return Code: 0 **
```

### Beispiel 3: Multiplikative Verknüpfung
```
Bitte geben Sie eine gültige Ganzzahl ein.

Modulo n der Restklasse: 
719

Bitte geben Sie eine gültige Ganzzahl ein.

Element g, deren Ordnung bestimmt werden muss: 
33

Bitte geben Sie eine gültige Verknüpfung (+, *, Beide) ein.

Verknüpfung, welche in der Gruppe herrscht: 
*

Multiplikative Verknüpfung

Teileranzahl:  4
Die Teiler sind:  [1, 2, 359, 718]

Die Ordnung des Elements  33  in der Restklasse  719  mit der multiplikativen Verknüpfung ist:  718


** Process exited - Return Code: 0 **
```

### Beispiel 4: Beide Verknüpfungen
```
Bitte geben Sie eine gültige Ganzzahl ein.

Modulo n der Restklasse: 
719

Bitte geben Sie eine gültige Ganzzahl ein.

Element g, deren Ordnung bestimmt werden muss: 
37

Bitte geben Sie eine gültige Verknüpfung (+, *, Beide) ein.

Verknüpfung, welche in der Gruppe herrscht: 
Beide

Multiplikative Verknüpfung

Teileranzahl:  4
Die Teiler sind:  [1, 2, 359, 718]

Die Ordnung des Elements  37  in der Restklasse  719  mit der multiplikativen Verknüpfung ist:  359

Additive Verknüpfung


Das Element  37  in der Restklasse  719  mit der additiven Verknüpfung hat keine Ordnung


** Process exited - Return Code: 0 **
```

## Verwendung

Bei der Verwendung des Programmes ist auf die Eingabe zu achten. Es gibt Exception Handling, also falls etwas Falsches eingegeben wird, dann wird man aufgefordert seine Eingabe zu prüfen.

Wenn genauere Infos über den Prozess im Programm benötigt werden, dann können Kommentare "#" vor einem print(???) entfernt werden, sodass somit Variablenwerte bei Programmlaufzeit ausgegeben werden.

Zum Beispiel:
```
#print(ordnung)
```

### Zur Eingabe:
Es gibt 3 Eingabevariablen:

| Variablen   | Eingabemöglichkeiten | Beschreibung                                  |
|-------------|----------------------|-----------------------------------------------|
| modulo      | Ganzzahlen / Int     | Modulo n der Restklasse                       |
| element     | Ganzzahlen / Int     | Element g, deren Ordnung bestimmt werden muss |
| Verknüpfung | + / * / Beide        | Verknüpfung in einer Gruppe                   |

