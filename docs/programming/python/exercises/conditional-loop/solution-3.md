# Solution 3

## Treść zadania

Napisz program zgodny z poniższą specyfikacją.

### Specification

#### Input

* $n$ - liczba naturalna

#### Output

* Liczba powstała poprzez odwrócenie cyfr liczby $n$

## Solution

```python
n = int(input("Podaj liczbę naturalną: "))

odwrocona = 0

while n > 0:
    cyfra = n % 10
    
    ofwrocona *= 10
    odwrocona += cyfra

    n = n // 10

print(f"Liczba powstała z odwrócenia cyfr podanej liczby to {odwrocona}")
```
