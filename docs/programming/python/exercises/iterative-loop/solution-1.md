# Solution 1

## Treść zadania

Napisz program zgodny z poniższą specyfikacją.

### Specification

#### Input

* $n$ - liczba naturalna

#### Output

* $n!$ 

## Solution

```python
n = int(input("Podaj liczbę naturalną: "))

silnia = 1

for i in range(2, n + 1):
    silnia *= i

print(f"{n}! = {silnia}")
```
