# [CSS Selekoren & Kombinatoren](https://wiki.selfhtml.org/wiki/CSS/Selektoren)


## Selektoren

### Universalselektor `*`

Eine CSS Regel, die mit `*` beginnt, wählt alle Elemente des Dokumentes aus. Später könne mit den Kombinatoren, bestimmte Teile des HTML-Dokuments angesprochen werden.


### Typselektoren: `element`

Steht ein Elementename zu Beginn einer Regel, beziehen sich die Aussagen, genau auf die Elemente von diesem Typ. D.h. 
```css
a {
    background-color: silver;
}
```
würde alle `a`-Elemente vor einem silbernem Hintergrund darstellen.


### Klassenselektoren: `.class`

Es git die Möglichkeit HTML-Elmente ein Attribut `class` zuzuweisen und diese dann über CSS anzusprechen. Die folgende Kombination würde auch den Hintergrund eines Links grau machen.
```css
.grey {
    color = grey;
}

<a class='grey' href='...'>LINK</a>
```


### ID-Selektoren: `#id`

Entsprechend der Klasse, kann man einzelnen HTML-Elementen auch das Attribut `id` setzten - diese müssen aber eindeutig gewählt werden. Diese lassen sich dann auch über CSS formatieren.
```css
#homepage {
    color = red;
}

<a id="homepage" href="...">LINK</a>
```

### Attributselektoren

Theoretisch kann man auch CSS Regeln formulieren, die für Elmente bestimmten Attributen gelten sollen.
```css
[alt] {
    color = red;
}

<img src="mypic.jpg" alt="Bildbeschreibung">
```

Für diesen Fall gibt es sehr viele Möglichkeiten - mit begrenztem Nutzen. Eine [Übersicht](https://wiki.selfhtml.org/wiki/CSS/Selektoren/Attributselektor) gibt es z.B. bei `selfhtml.org`.

## Kombinatoren


Kombinatoren sind Zeichen, die zwei Selektoren miteinander verketten. Durch diese Verkettung bildet der erste Teilselektor eine Bedingung und der zweite Teilselektor das Ziel, das angesprochen werden soll, wenn die Bedingung erfüllt wurde. Der Kombinator gibt dabei an, in welchem Verhältnis die Teilselektoren vor und nach ihm zueinander stehen müssen.

Zwischen zwei Selektoren kann nur ein Kombinator stehen, jedoch kann an diese Kette ein weiterer Kombinator zusammen mit einem weiteren Teilselektor angehängt werden.

### HTML-Elementstruktur

Je nachdem, wie verschiedene HTML-Elemente in einander verschachtelt werden werden zwischen diesen Beziehungen festgelegt. Die Struktur einer HTML-Seite (DOM: Document Object Model) kann man z.B. mit dem [Live-DOM-Viewer](https://software.hixie.ch/utilities/js/live-dom-viewer/) analysieren.

Für unsere Angaben beziehen wir uns auf folgendes Beispiel:

```html
<article>
    <figure>
        <img src="bild.jpg" alt="Bild">
    </figure>
    <section>
        Bla <em>blubb</em> bla bla.
    </section>
</article>
```

### Kindkombinator: `e > f`

Das Element `f` ist ein Kind von `e`, falls es sich direkt innerhalb dessen befindet. D.h. sowohl `figure` und `section` sind Kinder von `article`, aber `img` ist nur Kind von `figure`, `em` ist nur Kind von `section`. 

Hinweis: `e > * > f` würde die Enkel von `e` auswählen.


### Nachfahrenkombinator: `e f`

`f` ist Nachfahre von `e`, wenn es irgendwo in dem Element vorkommt. D.h. im obigen Beispiel sind alle Elemente zwischen `article` Nachfahren.



### Nachbarkombinator: `e + f`

Das Nachbarschaftsverhältnis bedeutet, dass zwei Elemente tatsächlich im HTML-Code benachbart sind, d.h. `f`muss direkt auf `e` folgen.  In unserem Beispiel wäre also `section` Nachbar von `figure`.

### Geschwisterkombinator: `e ~ f`

`f` hat eine Geschwisterbeziehung zu `e`, falls diese das Elternelement gemeinsam haben. `section` und `figure` sind damit Geschwister, da diese Kindelemente  von `article`sind.
