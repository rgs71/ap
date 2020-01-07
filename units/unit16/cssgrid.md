# CSS Grid

Mit CSS Grid können die HTML-Elemente auf dem Bildschirm angeordnet werden.

Hier eine Beispielkonfiguration:

```css

.container {
    height: 100vh;
    width: 100wh;
    display: grid;
    grid-template-rows: 200px 1fr 50px;
    grid-template-columns: 12% 22% 22% 22% 22%;
    grid-template-areas:
        "header header header header header"
        "sidebar content content content content"
        "footer footer footer footer footer"
    ;
}

header {
    grid-area: header;
    background-color: #ffaabb;
    text-align: center;
    margin: 10px;

}
```

Dabei wird hier der Bildschirm in drei Reihen und 5 Spalten aufgeteilt und die entsprechenden Elemente jeweils Rechtecken zugeordnet, indem diese benannt werden (`sidebar`).

Per CSS können dann HTML-Elementen durch `grid-area: ...` entsprechende Flächen zugewiesen werden. 

Die Größe der so entstehenden Rechtecke können entweder über die Anzahl der Reihen und Spalten oder über die Angabe der Spaltenbreiten in den `grid-template-columns` bzw. die Angabe der Reihenhöhen über `grid-template-rows` festgelegt werden. Dabei sind prozentuale Angaben, Anteile (`fr` Fraction) oder absolute Angaben in Pixeln `px` möglich.
Die ersten beiden Zeilen geben an, dass 100% der Höhe und Breite ausgenutzt werden.