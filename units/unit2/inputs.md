# Darstellung von Eingaben

* Wir benötigen eine stadartisierte Darstellung von Eingaben zu unseren Problemen.

* Beispiel: Zählen
    > Wir wollen die Anzahl der Personen in einem Raum zählen.

* Es gibt verschiedene Möglichkeiten:

    - 

    -   

    -   



## Binärzahlen

* Computer speichern Daten auf der unteresten Ebene als binäre Daten in Bits (**bi**nary digi**ts**).

* Die einzigen Speicherzustände sind 0 und 1, was mit Elektrizität an und aus korresponiert.

* Wir rechnen im Zehnersystem:

    $(123)_{10} = 1 \cdot 10^2 + 2 \cdot 10^1 + 3 \cdot 10^0$

* Im Binärsystem (Zweiersystem) stehen die entsprechenden Stellen für Potenzen von 2.

    $(1101)_2 = 1 \cdot 2^3 + 1 \cdot 2^2 + 0 \cdot 2^1 + 1 \cdot 2^0$

* Mit ausreichend vielen Bits können Computer viel höher zählen.


## Darstellung von Buchstaben

* Im Jahr 1963 wurde mit dem [ASCII-Code](https://de.wikipedia.org/wiki/American_Standard_Code_for_Information_Interchange) eine erste Zordnung zwischen den Zahlen 0 bis 127 und 95 druckbaren und 33 Steuerzeichen vereinbart.

* Zuordnung Buchstabe zu Zahl:

    ```
    A = 65
    B = 66
    C = 67
    ...
    Z = 95
    ```

* Damit lassen sich Buchstaben durch 8 Bits beschreiben. 8 Bits werden als 1 Byte bezeichnet.

* Computerprogramme wissen aus dem Kontext heraus, wie sie die binärgespeicherten Daten verwenden müssen. Der Kontext bestimmt, ob diese als 
    - Zahl
    - Buchstabe
    - Ton
    - Farbe

    interpretiert werden.



## Repräsentation von Daten

* **Abstraktion** ist eine Grundidee in der Informatik, wo eine grundlegende Implementation (so wie das tatsächliche Speichern von Daten in Bits) angenommen wird, um so übergeordnete Konzepte (wie die Represäntation von Buchstaben durch Zahlen) zu ermöglichen.

* Auf einer typischen Tastatur sind nicht alle Symbole und Buchstaben sichtbar.

* Alle möglichen Buchstaben mit beliebigen Akzenten, sogar Emoji können als Buchstabe bestehend aus mehrer Bytes beschrieben werden - der zugehörige Standard ist Unicode.

* Computer können binäre Daten auch als Bilder verstehen. Die drei Bytewerte geben dabei die Anteile von **R**ot, **B**lau und **G**rün an. So können wir viele Millionen ($256^3$) Farben darstellen.

* Kombiniert man die Farbwerte (Farbaddition) erhält so beliebe Farbtöne.

* Viele farbige Pixel können dann zu Bildern zusammengefasst werden.

* Filme lassen sich als Abfolge von Bildern kodieren.