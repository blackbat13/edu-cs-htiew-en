# Solution 3

## Treść zadania

Napisz program zgodny z poniższą specyfikacją.

### Specification

#### Input

* $n$ - liczba naturalna
* $a_1,a_2,\dots,a_n$ - $n$ liczb całkowitych
* $p, k$ - dwie liczby naturalna, $1<=p,k<=n$, $p <= k$

#### Output

* $a_p+a_{p+1}+a_{p+2}+...+a_{k}$ - suma wartości na pozycjach od $p$ do $k$

## Solution

```python
n = int(input("Podaj liczbę wartości: "))
tab = [int(input(f"Podaj liczbę nr {i + 1}: ")) for i in range(n)]
p = int(input("Podaj początek zakresu: "))
k = int(input("Podaj koniec zakresu: "))

p -= 1
suma = sum(tab[p:k])

print(f"Suma elementów z podanego zakresu wynosi {suma}")
```