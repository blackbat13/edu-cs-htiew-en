# Różnice w sekwencji

Masz daną sekwencję $n$ liczb całkowitych. Twoim zadaniem jest sprawdzić, czy przy obliczaniu wartości bezwzględnych różnic pomiędzy każdą parą kolejnych elementów sekwencji, uzyskamy wszystkie liczby od $1$ do $n-1$ włącznie.

Źródło: [https://onlinejudge.org/external/100/10038.pdf](https://onlinejudge.org/external/100/10038.pdf)

## Specification

### Input

* $n$ - liczba naturalna z przedziału $[1,3000]$
* $tab[n]$ - sekwencja $n$ liczb całkowitych

### Output

* "TAK" jeżeli sekwencja spełnia opisane wyżej wymaganie, lub "NIE" w przeciwnym przypadku

## Example 1

### Input

```
4
1 4 2 3
```

### Output

```
TAK
```

!!! info
	#### Wyjaśnienie
	
	Przyjrzyjmy się wartościom bezwzględnym różnic pomiędzy sąsiednimi elementami sekwencji:
	
	* $|1-4|=3$
	* $|4-2|=2$
	* $|2-3|=1$
	
	Jak widać otrzymaliśmy wszystkie wartości z przedziału $[1,n-1]$, czyli z przedziału $[1,3]$.

## Example 2

### Input

```
5
1 4 2 -1 6
```

### Output

```
NIE
```

!!! info
	#### Wyjaśnienie
	
	Przyjrzyjmy się wartościom bezwzględnym różnic pomiędzy sąsiednimi elementami sekwencji:
	
	* $|1-4|=3$
	* $|4-2|=2$
	* $|2-(-1)|=3$
	* $|-1-6|=7$
	
	Jak widać nie otrzymaliśmy wszystkich wartości z przedziału $[1,n-1]$, czyli z przedziału $[1,4]$
