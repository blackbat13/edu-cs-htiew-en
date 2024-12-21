# Rozwiązania - Python

## Zadanie 1

```python linenums="1"
with open("sequences.txt") as file:
    sequences = []
    for line in file:
        sequences.append(list(map(int, line.split()))[1:])

for seq in sequences:
    print(sum(seq))
```

## Zadanie 2

```python linenums="1"
with open("sequences.txt") as file:
    sequences = []
    for line in file:
        sequences.append(list(map(int, line.split()))[1:])

for seq in sequences:
    print(f"Minimum: {min(seq)}, Maksimum: {max(seq)}")
```

## Zadanie 3

```python linenums="1"
def is_prime(n):
    if n < 2:
        return False

    i = 2
    while i * i <= n:
        if n % i == 0:
            return False

        i += 1

    return True

with open("sequences.txt") as file:
    sequences = []
    for line in file:
        sequences.append(list(map(int, line.split()))[1:])

for seq in sequences:
    primes = []
    for num in seq:
        if is_prime(num):
            primes.append(num)

    print(f"Ile pierwszych: {len(primes)}, Liczby pierwsze: ", end="")
    print(*primes)
```

## Zadanie 4

```python linenums="1"
with open("sequences.txt") as file:
    sequences = []
    for line in file:
        sequences.append(list(map(int, line.split()))[1:])

for seq in sequences:
    current_length = max_length = 1
    current_start = max_start = 0
    for i in range(1, len(seq)):
        if seq[i] > seq[i - 1]:
            current_length += 1
            if current_length > max_length:
                max_length = current_length
                max_start = current_start
        else:
            current_length = 1
            current_start = i

    print(f"Dlugosc: {max_length}, Sekwencja: ", end="")
    print(*seq[max_start : max_start + max_length])
```

## Zadanie 5

```python linenums="1"
from math import gcd

with open("sequences.txt") as file:
    sequences = []
    for line in file:
        sequences.append(list(map(int, line.split()))[1:])

for seq in sequences:
    count = 0
    for i in range(len(seq)):
        for j in range(i + 1, len(seq)):
            if gcd(seq[i], seq[j]) == 1:
                count += 1

    print(count)
```
