# Podstawowe

## Zadanie 1

Napisz funkcję `CnaF` zgodną z poniższą specyfikacją.

Skorzystaj z następującego wzoru:

$F = \frac{9}{5} * C + 32$

gdzie:

* $C$ - temperatura podana w stopniach Celsjusza
* $F$ - temperatura podana w stopniach Fahrenheita

### Specification

#### Input

* $temp$ - liczba rzeczywista, temperatura podana w stopniach Celsjusza

#### Output

* Podana temperatura przekonwertowana na stopnie Fahrenheita.

### Example

```
CnaF(-50) = -58
CnaF(0) = 32
CnaF(100) = 212
```

## Zadanie 2

Napisz funkcję `KonwTemp` zgodną z poniższą specyfikacją.

Skorzystaj z następujących wzorów:

- $C = K - 273.15$
- $C = \frac{5}{9} * (F - 32)$
- $F = \frac{9}{5} * C + 32$
- $F = \frac{9}{5} * K - 459.67$
- $K = C + 273.15$
- $K = \frac{5}{9} * (F + 459.67)$

gdzie:

* $C$ - temperatura podana w stopniach Celsjusza
* $F$ - temperatura podana w stopniach Fahrenheita
* $K$ - temperatura podana w stopniach Kelvina

### Specification

#### Input

* $temp$ - liczba rzeczywista, temperatura do konwersji
* $jednZ$ - jeden znak, wielka litera oznaczająca jednostkę temperatury z której należy dokonać konwersji
* $jednDo$ - jeden znak, wielka litera oznaczająca jednostkę temperatury do której należy dokonać konwersji

#### Output

* Podana temperatura przekonwertowana z jednostki $jednZ$ do jednostki $jednDo$.

### Example

```
KonwTemp(0; "C"; "F") = 32
KonwTemp(32; "F"; "C") = 0
KonwTemp(212; "F"; "K") = 373.15
KonwTemp(100; "K"; "F") = -279.67
KonwTemp(-40; "C"; "K") = 233.15
KonwTemp(273.15; "K"; "C") = 0
```

## Zadanie 3

Napisz funkcję `CzyParzysta` zgodną z poniższą specyfikacją.

### Specification

#### Input

* $n$ - liczba naturalna

#### Output

* TRUE, jeżeli $n$ jest liczbą parzystą, FALSE w przeciwnym przypadku.

### Example

```
CzyParzysta(0) = TRUE
CzyParzysta(1) = FALSE
```

## Zadanie 4

Napisz funkcję `IleParzystych` zliczającą ile komórek z podanego zakresu zawiera liczby parzyste.

### Example

```
IleParzystych(A1:A10) = 3
```

## Zadanie 5

Napisz funkcję `NWW` zgodną z poniższą specyfikacją.

### Specification

#### Input

* $a$ - liczba naturalna
* $b$ - liczba naturalna

#### Output

* Najmniejsza wspólna wielokrotność liczb $a$ i $b$.

### Example

```
NWW(4; 8) = 8
NWW(3; 5) = 15
NWW(10; 6) = 30
```

## Zadanie 6

Napisz funkcję `IleCyfr` zgodną z poniższą specyfikacją.

### Specification

#### Input

* $n$ - liczba naturalna

#### Output

* Liczba cyfr liczby $n$.

### Example

```
IleCyfr(12345) = 5
IleCyfr(212) = 3
IleCyfr(0) = 1
```

## Zadanie 7

Napisz funkcję `Fibonacci` zgodną z poniższą specyfikacją.

### Specification

#### Input

* $n$ - liczba naturalna

#### Output

* Liczba Fibonacciego o indeksie $n$.

### Example

```
Fibonacci(0) = 0
Fibonacci(1) = 1
Fibonacci(2) = 1
Fibonacci(3) = 2
Fibonacci(4) = 3
```

## Zadanie 8

Napisz funkcję `ZWielkiej` zgodną z poniższą specyfikacją.

### Specification

#### Input

* $wyraz$ - ciąg znaków

#### Output

* Podany wyraz, w którym pierwsza litera jest wielka.

### Example

```
ZWielkiej("Ala") = "Ala"
ZWielkiej("ala") = "Ala"
ZWielkiej("ALA") = "ALA"
```
