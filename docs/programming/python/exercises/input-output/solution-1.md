# Rozwiązanie 1

## Treść zadania

Napisz program zgodny z poniższą specyfikacją.

### Specyfikacja

#### Dane

* $imie$ - ciąg znaków, małych i wielkich liter alfabetu angielskiego

#### Wynik

* Komunikat powitania w formie "_Witaj \[**imie**]!_", np. "_Witaj Damian!_"

## Rozwiązanie

```python
imie = input("Podaj swoje imię: ")
    
print(f"Witaj {imie}!")
```
