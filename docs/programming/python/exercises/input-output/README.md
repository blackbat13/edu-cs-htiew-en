# Obsługa wejścia/wyjścia

## Zadanie 1

Napisz program zgodny z poniższą specyfikacją.

### Specification

#### Input

* $imie$ - ciąg znaków, małych i wielkich liter alfabetu angielskiego.

#### Output

* Komunikat powitania w formie "_Witaj \[**imie**]!_"

### Example

#### Input

```
imie := "Damian"
```

**Output**: "Witaj Damian!"

## Zadanie 2

Napisz program zgodny z poniższą specyfikacją.

### Specification

#### Input

* $a, b$ - dwie liczby całkowite.

#### Output

* Suma liczb $a$ i $b$.

### Example

#### Input

```
a := 2
b := 3
```

**Output**: $5$ 

## Zadanie 3

Napisz program zgodny z poniższą specyfikacją.

### Specification

#### Input

* $a, b$ - dwie liczby całkowite, różne od zera.

#### Output

* Iloraz (wynik dzielenia), iloczyn (wynik mnożenia), suma oraz różnica liczb $a$ i $b$.

### Example

#### Input

```
a := 1
b := 2
```

**Output**: 
```
Iloraz: 0.5
Iloczyn: 2
Suma: 3
Różnica: -1
``` 

## Zadanie 4

Napisz program zgodny z poniższą specyfikacją.

### Specification

#### Input

* $a, b$ - dwie liczby naturalne, większe od zera.

#### Output

* Wynik dzielenia całkowitego oraz reszta z dzielenia liczb $a$ i $b$.

### Example

#### Input

```
a := 7
b := 3
```

**Output**: $2$, reszty $1$.

## Zadanie 5

Napisz program zgodny z poniższą specyfikacją.

!!! info
	**Podpowiedź**
	
	Skorzystaj z funkcji **`sqrt`** z biblioteki **`math`**.

### Specification

#### Input

* $a$ - liczba naturalna.

#### Output

* Pierwiastek z $a$

### Example

#### Input

```
a := 4
```

**Output**: $2$ 

## Zadanie 6

Napisz program zgodny z poniższą specyfikacją. Wykorzystaj funkcję **min**.

### Specification

#### Input

* $a, b$ - dwie liczby całkowite.

#### Output

* Mniejsza z liczb $a$ i $b$, lub dowolna gdy są sobie równe.

### Example

#### Input

```
a := 5
b := 3
```

**Output**: $3$ 

## Zadanie 7

Napisz program zgodny z poniższą specyfikacją. Wykorzystaj funkcję **max**.

### Specification

#### Input

* $a, b, c$ - trzy liczby całkowite.

#### Output

* Największa z liczb $a$, $b$ i $c$ , lub dowolna gdy są sobie równe.

### Example

#### Input

```
a := 3
b := 1
c := 3
```

**Output**: $3$ 

## Zadanie 8

Napisz program zgodny z poniższą specyfikacją.

### Specification

#### Input

* $sekundy$ - liczba naturalna.

#### Output

* Czas podany w czytelnej formie $H:M:S$ ($H$ - godziny, $M$ - minuty, $S$ - sekundy).

### Example

#### Input

```
sekundy := 9179
```

**Output**: $2:32:59$ 

!!! info
	**Wyjaśnienie**
	
	$2H=7200S$ 
	
	$32M=1920S$ 
	
	$2H+32M+59S=7200S+1920S+59S=9179S$ 
