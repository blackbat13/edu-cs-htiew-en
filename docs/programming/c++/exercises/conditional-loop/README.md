# Pętla warunkowa

## Zadanie 1

Napisz program zgodny z poniższą specyfikacją.

### Specification

#### Input

* $n$ - liczba naturalna

#### Output

* Kolejne cyfry liczby $n$, wypisane od końca, tzn. zaczynając od cyfry jedności

## Zadanie 2

Napisz program zgodny z poniższą specyfikacją.

### Specification

#### Input

* $n$ - liczba naturalna

#### Output

* Suma cyfr liczby $n$

### Example

#### Input

```
n := 1234
```

**Output**: $10$

!!! info
	**Wyjaśnienie**
	
	$1+2+3+4=10$ 

## Zadanie 3

Napisz program zgodny z poniższą specyfikacją.

### Specification

#### Input

* $n$ - liczba naturalna

#### Output

* Liczba powstała poprzez odwrócenie cyfr liczby $n$

### Example

#### Input

```
n := 1234
```

**Output**: $4321$

## Zadanie 4

Napisz program zgodny z poniższą specyfikacją.

### Specification

#### Input

* $n$ - liczba naturalna
* $k$ - liczba naturalna z zakresu $[0,9]$

#### Output

* Liczba powstała poprzez zastąpienie każdej cyfry liczby $n$ przez wartość bezwzględną różnicy liczby $k$ i danej cyfry

### Example

#### Input

```
n := 1234
k := 3
```

**Output**: $2101$

!!! info
	Wyjaśnienie
	
	$|3-1|=2$ 
	
	$|3-2|=1$ 
	
	$|3-3|=0$ 
	
	$|3-4|=1$ 

## Zadanie 5

Napisz program zgodny z poniższą specyfikacją.

### Specification

#### Input

* $n$ - liczba naturalna

#### Output

* Zapis binarny liczby $n$

### Example

#### Input

```
n := 10
```

**Output**: $1010$

!!! info
	**Wyjaśnienie**
	
	$10_{10}=1010_2$ 

## Zadanie 6

Napisz program zgodny z poniższą specyfikacją.

### Specification

#### Input

* $n$ - liczba naturalna
* $p$ - liczba naturalna z zakresu $[2,9]$

#### Output

* Zapis liczby $n$ w systemie o podstawie $p$ 

### Example

#### Input

```
n := 10
p := 3
```

**Output**: $101$

!!! info
	**Wyjaśnienie**
	
	$10_{10}=101_3$ 
