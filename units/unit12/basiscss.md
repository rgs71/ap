# Grundlagen von CSS

## Wie kann man CSS zum formatieren einer HTML-Seite verwenden?

### Direktes Einbinden durch `style`-Attribut

Jedes HTML-Element kann durch das Universalattribut `style` formatiert werden.

* HTML-Code ohne `style`-Attribut  
    ```html
    <section style="color: darkred;"> 
    Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. 
</section>
```

* Ergebnis ohne `style`-Attribut  
    <section> 
    Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. 
</section>

* HTML-Code mit `style`-Element  
    ```html
<section> 
    Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. 
</section>
```
* Ergebnis mit `style`-Attribut  
    <section style="color: darkred;"> 
    Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. 
</section>



