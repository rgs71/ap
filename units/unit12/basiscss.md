# Grundlagen von CSS

## Wie kann man CSS zum formatieren einer HTML-Seite verwenden?

### Direktes Einbinden durch `style`-Attribut

Jedes HTML-Element kann durch das Universalattribut `style` formatiert werden.

* HTML-Code ohne `style`-Attribut:  
    ```html
    <section> 
        Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. 
    </section>
    ```

* Ergebnis ohne `style`-Attribut:  
    <section style="padding: 25px;">
        Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. 
    </section>

* HTML-Code mit `style`-Element:  
    ```html
    <section style="color: darkred;"> 
        Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. 
    </section>
    ```

* Ergebnis mit `style`-Attribut:  
    <section style="padding: 25px; color: darkred;"> 
        Lorem ipsum dolor sit amet, consetetur sadipscing elitr,
        sed diam nonumy eirmod tempor invidunt ut labore
        et dolore magna aliquyam erat, sed diam voluptua. 
    </section>


### Formatierung mit dem `<style>`-Element

Statt einzelne HTML-Elemente durch das `style`-Attribut zu verändern, kann man direkt mehrer HTML-Elemente durch die Regeln von CSS verändern. Diese Regeln werden dafür in dem `<style>`-Element zusammengefasst.

* HTML-Code mit `<style>`-Element:
    ```html
    <style>
        section {
            background-color: lightgrey;
            color: green;
        }
        h3 {
            color: darkgreen;
        }
    </style>
    <section>
        <h3>Lorem Ipsum</h3> 
        Lorem ipsum dolor sit amet, consetetur sadipscing elitr, 
        sed diam nonumy eirmod tempor invidunt ut labore et 
        dolore magna aliquyam erat, sed diam voluptua. 
    </section>
    ```
* Ergebnis mit `<style>`-Element:  
    <section style="background-color: lightgrey;  color: green; padding: 25px;">
        <h3 style="color: darkgreen;">Lorem Ipsum</h3> 
        Lorem ipsum dolor sit amet, consetetur sadipscing elitr,
        sed diam nonumy eirmod tempor invidunt ut labore
        et dolore magna aliquyam erat, sed diam voluptua. 
    </section>


## Einbinden eines Stylesheets

Statt einem `<style>`-Element kann man auch diese Angaben in eine Datei auslagern und diese durch einen `<link>`-Element im `<head>` des HTML-Dokuments einbinden.

* Neues HTML-Grundgerüst inklusive eingebundem Stylesheet:  

    ```html
    <!DOCTYPE html>
    <html lang="de">
    <head>
        <meta charset="utf-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <link rel="stylesheet" href="style/stylesheet.css">
        <title>Titel</title>
    </head>
    <body>
        <h1>Grundgerüst</h1>
        <section>
        Aufbau eines simplen HTML-Dokuments.
        </section>
    </body>
    </html>
    ```
    Dabei befindet sich mit der HTML-Datei ein Unterorder `style` indem die Datei `stylesheet.css` ist.

* Typischer Aufbau des Stylesheets:  
    ```css
    h1 {
      color: green;
    }
    section {
        color: lightgreen;
        background-color: lightgrey;
    }
    ```


