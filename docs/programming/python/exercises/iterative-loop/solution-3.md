# Solution 3

## Treść zadania

Napisz program zgodny z poniższą specyfikacją.

### Specification

#### Input

* $n$ - liczba naturalna
* $n$ liczb całkowitych

#### Output

* Suma podanych $n$ liczb

## Solution

```python
n = int(input("Podaj liczbę wartości: "))

suma = 0

for i in range(n):
    liczba = int(input(f"Podaj liczbę nr {i + 1}: "))
    suma += liczba

print(f"Suma podanych liczb wynosi {suma}")
```
