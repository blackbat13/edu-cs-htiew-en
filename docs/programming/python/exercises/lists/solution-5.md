# Solution 5

## Treść zadania

Napisz program zgodny z poniższą specyfikacją.

### Specification

#### Input

* $n$ - liczba naturalna, $n>2$

#### Output

* $fib[n]$ - lista zawierająca $n$ kolejnych liczb Fibonacciego

## Solution

```python
n = int(input("Podaj liczbę wartości: "))

fib = [1, 1]

for i in range(2, n):
    fib.append(fib[i - 1] + fib[i - 2])

print(f"Kolejne {n} liczb Fibonacciego: {fib}")
```