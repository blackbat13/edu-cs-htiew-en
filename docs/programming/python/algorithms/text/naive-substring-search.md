# Naiwne wyszukiwanie wzorca w tekście

## [:link: Opis problemu](../../../../algorithms/text/naive-substring-search.md)

## Znajdowanie miejsca pierwszego wystąpienia wzorca w tekście 

```python linenums="1"
def substring_pos(a: str, b: str) -> int:
    for i in range(len(a) - len(b)):
        j = 0
        while j < len(b) and b[j] == a[i + j]:
            j += 1
 
        if j == len(b):
            return i
 
    return -1

a = "alamakota"
b = "kot"
 
pos = substring_pos(a, b)
if pos == -1:
    print(f'{b} is not a substring of {a}')
else:
    print(f'{b} is substring of {a} and starts at position {pos}')
```
