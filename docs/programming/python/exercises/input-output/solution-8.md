# Solution 8

## Treść zadania

Napisz program zgodny z poniższą specyfikacją.

### Specification

#### Input

* $sekundy$ - liczba naturalna

#### Output

* Czas podany w czytelnej formie ** **$H:M:S$ ($H$ - godziny, $M$ - minuty, $S$ - sekundy)

## Solution

```python
sekundy = int(input("Podaj liczbę sekund: "))
    
godziny = sekundy // (60 * 60)
    
sekundy = sekundy % (60 * 60)
    
minuty = sekundy // 60
    
sekundy = sekundy % 60

print(f"{godziny}:{minuty}:{sekundy}")
```
