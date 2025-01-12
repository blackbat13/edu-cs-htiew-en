# Solution 1

## Treść zadania

Napisz program zgodny z poniższą specyfikacją. Nie korzystaj z funkcji **abs**

### Specification

#### Input

* $a$ - liczba całkowita

#### Output

* Wartość bezwzględna z $a$

## Solution

```python
a = int(input("Podaj liczbę całkowitą: "))

if a < 0:
    print(f"|{a}| = {-a}")
else:
    print(f"|{a}| = {a}")
```
