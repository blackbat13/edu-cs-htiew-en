# Tablice statyczne

## Zadanie 1

Napisz program zgodny z poniższą specyfikacją.

### Specification

#### Input

* $n$ - liczba naturalna
* $a_1,a_2,\dots,a_n$ - $n$ liczb całkowitych

#### Output

* $a_n,a_{n-1},\dots,a_2,a_1$ - podane liczby w odwrotnej kolejności

### Example

#### Input

```
n := 5
a1 := 1
a2 := 2
a3 := 3
a4 := 4
a5 := 5
```

**Output**: $5, 4, 3, 2, 1$ 

## Zadanie 2

Napisz program zgodny z poniższą specyfikacją.

### Specification

#### Input

* $n$ - liczba naturalna
* $a_1,a_2,\dots,a_n$ - $n$ liczb całkowitych
* $k$ - liczba naturalna, $1<=k<=n$

#### Output

* $a_k$ - $k$-ta podana liczba

### Example

#### Input

```
n := 5

a1 := 8
a2 := 3
a3 := 9
a4 := 1
a5 := 2

k := 3
```

**Output**: $9$ 

!!! info
	**Wyjaśnienie**
	
	$k := 3$, a trzecia podana wartość wynosi $9$ (a3 := 9). 

## Zadanie 3

Napisz program zgodny z poniższą specyfikacją.

### Specification

#### Input

* $n$ - liczba naturalna
* $a_1,a_2,\dots,a_n$ - $n$ liczb całkowitych
* $p, k$ - dwie liczby naturalna, $1<=p,k<=n$, $p <= k$

#### Output

* $a_p+a_{p+1}+a_{p+2}+...+a_{k}$ - suma wartości na pozycjach od $p$ do $k$

### Example

#### Input

```
n := 5

a1 := 8
a2 := 3
a3 := 9
a4 := 1
a5 := 2

p := 3
k := 5
```

**Output**: $12$ 

!!! info
	**Wyjaśnienie**
	
	$a_3+a_4+a_5=9+1+2=12$

## Zadanie 4

Napisz program zgodny z poniższą specyfikacją.

### Specification

#### Input

* $n$ - liczba naturalna
* $t1[n],\ t2[n]$ - dwie tablice liczb całkowitych

#### Output

* Tablica powstała poprzez dodanie do siebie wartości z tablic $t1$ i $t2$ 

### Example

#### Input

```
n := 5
t1 := [4, 1, 7, 0, 2]
t2 := [2, 3, 1, 9, 6]
```

**Output**: $6, 4, 8, 9, 8$ 

!!! info
	**Wyjaśnienie**
	
	$[4+2,\ 1+3,\ 7+1,\ 0+9,\ 2+6]$ 

## Zadanie 5

Napisz program zgodny z poniższą specyfikacją.

### Specification

#### Input

* $n$ - liczba naturalna

#### Output

* $fib[n]$ - tablica zawierająca $n$ kolejnych liczb Fibonacciego

### Example

#### Input

```
n := 6
```

**Output**: $1, 1, 2, 3, 5, 8$ 

## Zadanie 6

Napisz program zgodny z poniższą specyfikacją.

### Specification

#### Input

* $n$ - liczba naturalna

#### Output

* $mno[n][n]$ - dwuwymiarowa tablica reprezentująca tabliczkę mnożenia liczb z zakresu $[0,n-1]$, gdzie $mno[i][j]=i*j$

### Example

#### Input

```
n := 3
```

#### Output

```
mno := [[0, 0, 0],
        [0, 1, 2],
        [0, 2, 4]]
```

## Zadanie 7

Napisz program zgodny z poniższą specyfikacją.

### Specification

#### Input

* $n$ - liczba naturalna
* $tab[n]$ - tablica liczb całkowitych

#### Output

* Komunikat "niemalejaco" jeżeli elementy tablicy posortowane są niemalejąco
* Komunikat "nierosnaco" jeżeli elementy tablicy posortowane są nierosnąco
* Komunikat "nieposortowane" jeżeli elementy tablicy nie są posortowane

### Example 1

#### Input

```
n := 5
tab := [1, 1, 5, 6, 8]
```

**Output**: "niemalejąco"

### Example 2

#### Input

```
n := 5
tab := [8, 5, 5, 3, 1]
```

**Output**: "nierosnąco"

### Example 3

#### Input

```
n := 5
tab := [1, 2, 3, 1, 5]
```

**Output**: "nieposortowane"