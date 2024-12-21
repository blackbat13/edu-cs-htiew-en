# Rozszerzony algorytm Euklidesa

## [:link: Opis problemu](../../../../algorithms/integers/extended-euclidean.md)

## Implementacja

```python linenums="1"
def extended_gcd(a: int, b: int) -> tuple:
  old_x, x = 1, 0
  old_y, y = 0, 1
  rest, old_rest = b, a
  
  while rest != 0:
    quotient = old_rest // rest

    old_x, x = x, old_x - quotient * x
    old_y, y = y, old_y - quotient * y
    old_rest, rest = rest, old_rest - quotient * rest

  return old_rest, old_x, old_y

a = 6
b = 21

gcd, x, y = extended_gcd(a, b)

print(f"{a} * {x} + {b} * {y} = {gcd}")
```
