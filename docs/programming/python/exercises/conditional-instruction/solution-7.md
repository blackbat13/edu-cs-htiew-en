# Solution 7

## Treść zadania

Napisz program zgodny z poniższą specyfikacją.

### Specification

#### Input

* $rok$ - liczba naturalna

#### Output

* Komunikat określający, czy podany rok jest przestępny czy też nie

## Solution

```python
rok = int(input("Podaj rok: "))

if (rok % 4 == 0 and rok % 100 != 0) or rok % 400 == 0:
    print(f"{rok} jest przestępny")
else:
    print(f"{rok} nie jest przestępny")
```
