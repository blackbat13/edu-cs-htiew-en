# Solution 4

## Treść zadania

Napisz program zgodny z poniższą specyfikacją. Nie korzystaj z funkcji **min, max**.

### Specification

#### Input

* $a, b, c$ - trzy liczby całkowite

#### Output

* Największa z liczb $a$, $b$ i $c$, lub dowolna gdy są sobie równe

## Solution

```python
a = int(input("Podaj pierwszą liczbę: "))
b = int(input("Podaj drugą liczbę: "))
c = int(input("Podaj trzecią liczbę: "))

maks = -1

if a >= b and a >= c:
    maks = a
elif b >= a and b >= c:
    maks = b
else:
    maks = c

print(f"Maksimum z {a}, {b} i {c} wynosi {maks}")
```
