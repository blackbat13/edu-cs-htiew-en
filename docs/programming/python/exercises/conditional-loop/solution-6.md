# Solution 6

## Treść zadania

Napisz program zgodny z poniższą specyfikacją.

### Specification

#### Input

* $n$ - liczba naturalna
* $p$ - liczba naturalna z zakresu $[2,9]$

#### Output

* Zapis liczby $n$ w systemie o podstawie $p$ 

## Solution

```python
n = int(input("Podaj liczbę naturalną: "))
p = int(input("Podaj podstawę systemu docelowego: "))

nowa = ""

while n > 0:
    cyfra = n % p
    
    nowa = str(cyfra) + nowa

    n = n // p

print(f"Wartość w systemie {p}: {nowa}")
```