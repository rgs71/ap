## Algorithms

* Zwischen den Ein- und Ausgaben steht unsere *black box*, die die Verabreitung übernimmt. In vielen Fällen wird es sich dabei um einen **Algorithmus** handeln, d.h. eine präzise Anweisungen, die nachvollziehbar aus den Eingaben zu den Ausgaben führen.

* Beispiel: Suche im Telefonbuch
  - Algorithmus 1: Blättere von vorne nach hinten und überprüfe jede Seite nach dem gesuchten Namen
  - Algorithmus 2: Schlage jede zweite Seite auf und suche nach dem Namen
  - Algorithmus 3: Schlage die Mitte auf, falls der Name nicht sort steht arbeite mit der alphabetisch richtigen Hälfte und wiederhole solange, bis der Name gefunden wurde.


  * Algorithmus 1 und 3 sind korrekt und führen sicher zu richtigen Ausgabe, Algorithmus 2 könnte den Namen überblättern. Aber Algorithmus 3 ist für große Eingaben (Telefonbuch mit vielen Seiten) der effizientere Algorithmus!

## Pseudocode

* Wir können in *Pseudocode*, einer unformalen Syntax die etwas spezifischer als gewöhnliches Deutsch ist, einen Algorithmus beschreiben:
  <pre>
   0 <b>nehme</b> das Telefonbuch
   1 <b>öffne</b> das Telefonbuch auf der mittleren Seite
   2 <b>sehe</b> Dir die Namen an
   3 <b>falls</b> Meyer unter den Namen ist
   4     <b>rufe</b> Meyer an
   5 <b>sonst falls</b> Meyer früher im Buch vorkommt
   6     <b>öffne</b> die Mitte der vorderen Hälfte
   7     <b>gehe zu </b> Schritt 2
   8 <b>sonst</b> falls Meyer später im Buch vorkommt
   9     <b>öffne</b> die Mitte der hinteren Hälfte
  10     <b>gehe zu </b> Schritt 2
  11 <b>sonst</b>
  12     <b>stoppe</b>
  </pre>

* Einige der Schritte starten mit Verben, die man später als *Funktionen* beschreiben würde.

* Außerdem kommen Fragen vor, deren Antwort richtig oder falsch sein können, solche Beziehungen werden als *Bedingungen* bezeichnet.

* Da wir abhängig von solchen Bedingungen unterschiedliche Schritte ausführen, bezeichnet man eine solche *falls*-*sonst wenn*-*sonst* Konstruktion als *Fallunterscheidung*.

* Die Teile des Codes, die durch zurückgehen mehrfach durchgeführt werden, heißen *Wiederholungen* 

## Scratch

* einfache grafische Programmiersprache, mit der man vor allem Figuren auf einer Bühne steuert.

* Alle wesentlichen Elemente einer vollständigen Programmiersprache sind vorhanden.

* Die Ergebnisse sind durch die graphische Darstellung sofort überprüfbar.