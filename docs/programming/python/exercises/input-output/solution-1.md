# Solution 1

## Treść zadania

Napisz program zgodny z poniższą specyfikacją.

### Specification

#### Input

* $imie$ - ciąg znaków, małych i wielkich liter alfabetu angielskiego

#### Output

* Komunikat powitania w formie "_Witaj \[**imie**]!_", np. "_Witaj Damian!_"

## Solution

```python
imie = input("Podaj swoje imię: ")
    
print(f"Witaj {imie}!")
```
