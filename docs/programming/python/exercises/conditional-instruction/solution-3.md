# Solution 3

## Treść zadania

Napisz program zgodny z poniższą specyfikacją.

### Specification

#### Input

* $a, b$ - dwie liczby całkowite

#### Output

* Wynik dzielenia liczb $a$ i $b$, lub komunikat, że nie można wykonać dzielenia.

## Solution

```python
a = int(input("Podaj pierwszą liczbę: "))
b = int(input("Podaj drugą liczbę: "))

if b == 0:
    print("Nie można dzielić przez 0")
else:
    print(f"{a} / {b} = {a / b}")
```
