# Instrukcja warunkowa

## Zadanie 1

Napisz program zgodny z poniższą specyfikacją. Nie korzystaj z funkcji **abs, fabs**

### Specification

#### Input

* $a$ - liczba całkowita

#### Output

* Wartość bezwzględna z $a$

### Example

#### Input

```
a := -2
```

**Output**: $2$ 

## Zadanie 2

Napisz program zgodny z poniższą specyfikacją.

### Specification

#### Input

* $a$ - liczba całkowita

#### Output

* Znak liczby $a$, tzn. $1$ gdy $a$ jest dodatnie, $-1$ gdy $a$ jest ujemne, $0$ gdy $a$ wynosi $0$ 

### Example 1

#### Input

```
a := 5
```

**Output**: $1$ 

### Example 2

#### Input

```
a := -5
```

**Output**: $-1$ 

### Example 3

#### Input

```
a := 0
```

**Output**: $0$ 

## Zadanie 3

Napisz program zgodny z poniższą specyfikacją.

### Specification

#### Input

* $a, b$ - dwie liczby całkowite

#### Output

* Wynik dzielenia liczb $a$ i $b$, lub komunikat, że nie można wykonać dzielenia.

### Example

#### Input

```
a := 1
b := 2
```

**Output**: $0.5$ 

## Zadanie 4

Napisz program zgodny z poniższą specyfikacją. Nie korzystaj z funkcji **min, max**.

### Specification

#### Input

* $a, b, c$ - trzy liczby całkowite

#### Output

* Największa z liczb $a$, $b$ i $c$ , lub dowolna gdy są sobie równe

### Example

#### Input

```
a := 4
b := 1
c := 3
```

**Output**: $4$ 

## Zadanie 5

Napisz program zgodny z poniższą specyfikacją. Nie korzystaj z funkcji **min, max**.

### Specification

#### Input

* $a, b, c, d$ - cztery liczby całkowite

#### Output

* Największa z liczb $a, b, c$ i $d$, lub dowolna gdy są sobie równe

### Example

#### Input

```
a := 3
b := 1
c := 3
d := 5
```

**Output**: $5$ 

## Zadanie 6

Napisz program zgodny z poniższą specyfikacją. Zadbaj o czytelność programu.

### Specification

#### Input

* $a, b$ - dwie liczby całkowite
* $op$ - znak jednej z dozwolonych operacji: $+,-,*,/$ 

#### Output

* Wynik działania$a\ op\ b$ (np. $a+b$), lub komunikat, że nie można wykonać dzielenia.

### Example

#### Input

```
a := 3
b := 1
op := '+'
```

**Output**: $4$ 

## Zadanie 7

Napisz program zgodny z poniższą specyfikacją.

!!! info
	**Rok przestępny** to taki, który:
	
	* jest podzielny przez 4, ale nie jest podzielny przez 100, lub
	* jest podzielny przez 400

### Specification

#### Input

* $rok$ - liczba naturalna

#### Output

* Komunikat określający, czy podany rok jest przestępny czy też nie

### Example

#### Input

```
rok := 2021
```

**Output**:  "Rok 2021 nie jest przestępny"
