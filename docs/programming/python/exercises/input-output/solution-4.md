# Solution 4

## Treść zadania

Napisz program zgodny z poniższą specyfikacją.

### Specification

#### Input

* $a, b$ - dwie liczby naturalne, większe od zera

#### Output

* Wynik dzielenia całkowitego oraz reszta z dzielenia liczb $a$ i $b$ 

## Solution

```python
a = int(input("Podaj pierwszą liczbę: "))
b = int(input("Podaj drugą liczbę: "))

div = a // b
mod = a % b

print(f"{a} / {b} = {div}, r. {mod}")
```
