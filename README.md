# Pattern-Framework

## Game Design Dokument

### Übersicht
„Zell-Attacke“ ist ein Spiel für zwei Spieler. Zu Beginn entscheidet man sich für eine Fraktion – entweder „Zelle“ oder „Virus“. Ziel ist es den Gegenspieler durch Angriffsaktionen zu besiegen.

### Spiel
* [Frontend](https://github.com/fb-bht/ZellAttacke)
* [Backend](https://github.com/fb-bht/ZellAttacke-JWTBackend)

### Avatar
Der Avatar des Spielers ist entweder ein Virus oder eine Zelle (im Folgenden als Kern bezeichnet).

* Attacken: Um den Kern rotiert ein Ring der durch absondern einer kleinen Zelle einen Angriff auf den Gegenspieler starten kann.
* Zeit: Attacken können nicht direkt hintereinander ausgeführt werden, sondern es muss kurz gewartet werden bis die „Energie“ wieder aufgeladen ist. Dieses Zeitfenster wird mit einem sich aufbauenden Ring dargestellt, der zwischen Kern und Angriffsring dargestellt wird.

Zelle | Virus
------|------
![Avatar](/images/zelle.png) | ![Avatar](/images/virus.png)

### Spiel
Nachdem der Spieler sich für seinen Avatar entschieden hat, wird dieser am unteren bzw. oberen Bildschirmrand plaziert und verändert seine Position im weiteren Spiel nicht. Zwischen den beiden Spielern schweben „neutrale“ Zellen (im Folgenden als Neutrale bezeichnet). Nur diese sind in der Lage den Gegenspieler zu eliminieren. Dazu muss der Spieler Neutrale mit seinem Angriff treffen und diese so von einer neutralen Bahn in Richtung des Gegenspielers ablenken. Je nach Level sind unterschiedlich viele Treffer erforderlich um den Gegenspieler zu besiegen.

### Spielfeld
Die linke und rechte Begrenzung des Spielfelds lässt die Neutralen davon abprallen. Die untere und obere Begrenzung des Spielfelds hat keine Wirkung auf die Neutralen aber auf die Angriffszellen.

![Spielfeld](/images/spielfeld.png)

### Steuerung
Mit den Buchstaben "C" für Zelle und "V" für Virus wird eine Angriffszelle vom Spieler gestartet.


