# Solution 2

## Treść zadania

Napisz program zgodny z poniższą specyfikacją. Obliczanie sumy powinno być zrealizowane za pomocą funkcji.

### Specification

#### Input

* $a, b$ - dwie liczby całkowite

#### Output

* Suma liczb $a$ i $b$ 

## Solution

```python
def suma(a: int, b: int) -> int:
    return a + b

a = int(input("Podaj pierwszą liczbę: "))
b = int(input("Podaj drugą liczbę: "))

wynik = suma(a, b)

print(f"{a} + {b} = {wynik}")
```
