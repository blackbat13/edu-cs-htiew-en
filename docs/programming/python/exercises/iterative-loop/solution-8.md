# Solution 8

## Treść zadania

Napisz program zgodny z poniższą specyfikacją.

### Specification

#### Input

* $n$ - liczba naturalna

#### Output

* Wszystkie trójki liczb naturalnych, których suma wynosi $n$

## Solution

```python
n = int(input("Podaj liczbę naturalną: "))

silnia = 1

for i in range((n // 3) + 1):
    for j in range(i, ((n - i) // 2) + 1):
        print(f"({i}, {j}, {n - i - j})")
```
