# Solution 2

## Treść zadania

Napisz program zgodny z poniższą specyfikacją.

### Specification

#### Input

* $a$ - liczba całkowita

#### Output

* Znak liczby $a$, tzn. $1$ gdy $a$ jest dodatnie, $-1$ gdy $a$ jest ujemne, $0$ gdy $a$ wynosi $0$ 

## Solution

```python
a = int(input("Podaj liczbę całkowitą: "))

znak = 0

if a < 0:
    znak = -1
elif a > 0:
    znak = 1
else:
    znak = 0

print(f"Znak liczby {a}: {znak}")
```
