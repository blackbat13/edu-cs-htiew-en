# Solution 1

## Treść zadania

Napisz program zgodny z poniższą specyfikacją.

### Specification

#### Input

* $n$ - liczba naturalna
* $a_1,a_2,\dots,a_n$ - $n$ liczb całkowitych

#### Output

* $a_n,a_{n-1},\dots,a_2,a_1$ - podane liczby w odwrotnej kolejności

## Solution

```python
n = int(input("Podaj liczbę wartości: "))
tab = [int(input(f"Podaj liczbę nr {i + 1}: ")) for i in range(n)]

tab.reverse()

print(tab)
```

### Description rozwiązania

Na początku wczytujemy od użytkownika liczbę elementów i zapisujemy ją w zmiennej $n$ (**linia 1**).

Następnie tworzymy listę wczytując do niej wartości (**linia 2**).

Ostatnim etapem rozwiązania jest odwrócenie kolejności elementów listy za pomocą polecenia `reverse` (**linia 4**). Na końcu wypisujemy odwróconą listę (**linia 6**).
