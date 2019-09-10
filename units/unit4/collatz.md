# Lösungen zur Hausaufgabe

## Collatzfolge als Pythoncode

```python
n = 1017

while n > 1:
    if n % 2 == 0:
        n = n // 2
    else:
        n = 3 * n + 1
    print(n)
```

## Collatzfolge im Programmablaufplan

(Erstellt mit dem [Structorizer](https://structorizer.fisch.lu/))

![Struktogramm des Codes zum Collatzfolge](collatz_struct.png)

## Collatzfolge im Programmablaufplan

(Erstellt mit dem [PAPDesigner](https://www.heise.de/download/product/papdesigner-51889))

![Programmablaufplan des Codes zum Collatzfolge](collatz_pap.png)

Alternativ, ohne Verwendung der speziellen Schleifendarstellung:

![Programmablaufplan des Codes zum Collatzfolge](collatz_pap2.png)

