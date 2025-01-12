# Solution 4

## Treść zadania

Napisz program zgodny z poniższą specyfikacją.

### Specification

#### Input

* $n$ - liczba naturalna, większa od $0$ 
* $n$liczb naturalnych

#### Output

* Największa z podanych $n$ liczb

## Solution

```python
n = int(input("Podaj liczbę wartości: "))

maks = -1

for i in range(n):
    liczba = int(input(f"Podaj liczbę nr {i + 1}: "))
    if liczba > maks:
        maks = liczba

print(f"Maksimum z podanych liczb wynosi {maks}")
```

## Solution alternatywne

```python
n = int(input("Podaj liczbę wartości: "))

maks = -1

for i in range(n):
    liczba = int(input(f"Podaj liczbę nr {i + 1}: "))
    maks = max(maks, liczba)

print(f"Maksimum z podanych liczb wynosi {maks}")
```