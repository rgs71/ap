# Grundlagen von CSS

## Wie kann man CSS zum formatieren einer HTML-Seite verwenden?

### Direktes Einbinden durch `style`-Attribut

Jedes HTML-Element kann durch das Universalattribut `style` formatiert werden.

* HTML-Code ohne `style`-Attribut  
    ```html
    <section> 
        Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. 
    </section>
    ```

* Ergebnis ohne `style`-Attribut  
    <section style="padding: 25px;">
        Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. 
    </section>

* HTML-Code mit `style`-Element  
    ```html
    <section style="color: darkred;"> 
        Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. 
    </section>
    ```

* Ergebnis mit `style`-Attribut  
    <section style="padding: 25px; color: darkred;"> 
        Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. 
    </section>


### Formatierung mit dem `<style>`-Element

Statt einzelne HTML-Elemente durch das `style`-Attribut zu verändern, kann man direkt mehrer HTML-Elemente durch die Regeln von CSS verändern. Diese Regeln werden dafür in dem `<style>`-Element zusammengefasst.

* HTML-Code mit `<style>`-Element
    ```html
    <style>
        section {
            background-color: lightgreen;
        }
        h3 {
            color: darkgreen;
        }
    </style>
    <section>
        <h3>Lorem Ipsum</h3> 
        Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. 
    </section>
    ```


    <section style="background-color: lightgrey;  color: green;">
        <h3 style="color: darkgreen; font: serif;">Lorem Ipsum</h3> 
        Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. 
    </section>
