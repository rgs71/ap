# Was muss man für die Kursarbeit können?

Du solltest Vorgänge beschreiben können und zwischen den Darstellungen wechseln können:
- **Pseudocode**
- einen **Programmablaufplan**
- ein **Struktogramm**

Als weitere Hilfe kann man auch nachvollziehen, was ein Programm macht, indem man während dem Programmablauf eine **Trace-Tabelle** anlegt:
| x | y | a |
|:---:|:---:|:---:|
| 0 | 6 | 4 |
| 1 | 2 | 4 |
||...||

Natürlich ist es am Ende das Ziel, diese Anweisungen in ein gültiges **Python-Programm** umzuwandelt, daher musst Du folgendes kennne:
- Definition von **Variablen** (`x = 3`)
- Verändern von Variablen (`x = x + 2`)
- `while`-**Schleifen**   
    ```python
    x = 0
    while x < 7:
        print(x)
        x = x + 1
    ```
- **Verzweigungen** mit `if-elif-else`   
    ```python
    if x > 0:
        print("positiv")
    elif x < 0:
        print("negativ")
    else:
        print("null")
    ```