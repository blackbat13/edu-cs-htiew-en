# Solution 5

## Treść zadania

Napisz program zgodny z poniższą specyfikacją. Nie korzystaj z funkcji **min, max**.

### Specification

#### Input

* $a, b, c, d$ - cztery liczby całkowite

#### Output

* Największa z liczb $a, b, c$ i $d$, lub dowolna gdy są sobie równe

## Solution

```python
a = int(input("Podaj pierwszą liczbę: "))
b = int(input("Podaj drugą liczbę: "))
c = int(input("Podaj trzecią liczbę: "))
d = int(input("Podaj czwartą liczbę: "))

maks = a

if b > maks:
    maks = b

if c > maks:
    maks = c

if d > maks:
    maks = d

print(f"Maksimum z {a}, {b}, {c} i {d} wynosi {maks}")
```