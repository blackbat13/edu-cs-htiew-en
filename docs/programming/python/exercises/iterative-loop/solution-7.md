# Solution 7

## Treść zadania

Napisz program zgodny z poniższą specyfikacją.

### Specification

#### Input

* $n$ - liczba naturalna

#### Output

* Wszystkie pary liczb naturalnych, których suma wynosi $n$

## Solution

```python
n = int(input("Podaj liczbę naturalną: "))

silnia = 1

for i in range((n // 2) + 1):
    print(f"({i}, {n - 1})")
```