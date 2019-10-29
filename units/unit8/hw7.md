# Alte Hausaufgabe


## Die `next_prime`-Funktion

```python
def next_prime(n):
    k = n + 1
    while not is_prime(k):
        k = k + 1
```

Die Idee ist, dass man Zahlen `k`, die größer als `n` sind sytematisch mit der `is_prime`-Funktion testet, bis man die nächste Primzahl gefunden hat.

## Visualisierung mit Python-Tutor

[Link zur Visualisierung](http://www.pythontutor.com/visualize.html#code=def%20is_prime%28n%29%3A%0A%20%20%20%20k%20%3D%202%0A%20%20%20%20while%20k%20%3C%20n%3A%0A%20%20%20%20%20%20%20%20if%20n%20%25%20k%20%3D%3D%200%3A%0A%20%20%20%20%20%20%20%20%20%20%20%20return%20False%0A%20%20%20%20%20%20%20%20k%20%3D%20k%20%2B%201%0A%20%20%20%20%0A%20%20%20%20return%20n%20%3E%201%0A%20%20%20%20%0A%20%20%20%20%0Adef%20next_prime%28n%29%3A%0A%20%20%20%20k%20%3D%20n%20%2B%201%0A%20%20%20%20while%20not%20is_prime%28k%29%3A%0A%20%20%20%20%20%20%20%20k%20%3D%20k%20%2B%201%0A%20%20%20%20%0A%20%20%20%20return%20k%0A%20%20%20%20%0Aprint%28next_prime%287%29%29&cumulative=false&curInstr=27&heapPrimitives=nevernest&mode=display&origin=opt-frontend.js&py=3&rawInputLstJSON=%5B%5D&textReferences=false)

## Ergebnisse

| 10er Potenz | Nächste Primzahl |
|:---:|----:|
| 10^0 | 2 |
| 10^1 | 11 |
| 10^2 | 101 |
| 10^3 | 1009 |
| 10^4 | 10007 |
| 10^5 | 100003 |
| 10^6 | 1000003 |
| 10^7 | 10000019 |
| 10^8 | 100000007|
| 10^9 | 1000000007 |
| 10^10 | 10000000019 |