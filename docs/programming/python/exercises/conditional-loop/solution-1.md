# Solution 1

## Treść zadania

Napisz program zgodny z poniższą specyfikacją.

### Specification

#### Input

* $n$ - liczba naturalna

#### Output

* Kolejne cyfry liczby $n$, wypisane od końca, tzn. zaczynając od cyfry jedności

## Solution

```python
n = int(input("Podaj liczbę naturalną: "))

while n > 0:
    cyfra = n % 10
    print(cyfra)
    n = n // 10
```
