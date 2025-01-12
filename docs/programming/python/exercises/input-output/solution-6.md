# Solution 6

## Treść zadania

Napisz program zgodny z poniższą specyfikacją. Wykorzystaj funkcję **min**.

### Specification

#### Input

* $a, b$ - dwie liczby całkowite

#### Output

* Mniejsza z liczb $a$ i $b$, lub dowolna gdy są sobie równe

## Solution

```python
a = int(input("Podaj pierwszą liczbę: "))
b = int(input("Podaj drugą liczbę: "))

wynik = min(a, b)

print(f"Minimum z {a} i {b} wynosi {wynik}")
```
