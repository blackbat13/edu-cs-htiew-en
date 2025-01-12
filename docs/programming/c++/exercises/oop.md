# Programowanie obiektowe

## Zadanie 1

Napisz program zgodny z poniższą specyfikacją. Do reprezentacji ułamków i wykonywania na nich operacji wykorzystaj własną implementację klasy.

### Specification

#### Input

* $l1, m1$ - licznik i mianownik pierwszego ułamka, liczby całkowite
* $op$ - znak operacji: $+$, $-$, $*$ lub $/$
* $l2, m2$ - licznik i mianownik drugiego ułamka, liczby całkowite

#### Output

* Wynik działania operacji $\frac{l1}{m2}\ op\ \frac{l2}{m2}$ przedstawiony w formie ułamka zwyczajnego (maksymalnie skróconego), wypisany w formacie `licznik / mianownik`, np. `3 / 4`

### Example 1

#### Input

```
l1 := 5
m1 := 8
op := '+'
l2 := 5
m2 := 8
```

#### Output

```
5 / 4
```

### Example 2

#### Input

```
l1 := -1
m1 := 2
op := '*'
l2 := 2
m2 := 4
```

#### Output

```
-1 / 4
```

## Zadanie 2

Napisz program zgodny z poniższą specyfikacją. Do reprezentacji liczb i wykonywania na nich operacji wykorzystaj własną implementację klasy.
Możesz założyć, że wartości wszystkich liczb w systemie dziesiętnym zmieszczą się w typie `int`. Wszystkie litery powinny być **drukowane**.

### Specification

#### Input

* $l1, p1$ - liczba $l1$ reprezentowana w podstawie $p1$, $2 \leq p1 \leq 16$
* $l2, p2$ - liczba $l2$ reprezentowana w podstawie $p2$, $2 \leq p2 \leq 16$
* $p3$ - docelowa podstawa, $2 \leq p3 \leq 16$

#### Output

* Suma podanych wartości przedstawiona w podstawie $p3$

### Example 1

#### Input

```
l1 := 1010
p1 := 2
l2 := 5
p2 := 10
p3 := 8
```

#### Output

```
17
```

!!! info
	**Wyjaśnienie**
	
	$1010_2+5_{10}=17_8$

### Example 2

#### Input

```
l1 := 1010
p1 := 2
l2 := 5
p2 := 10
p3 := 16
```

#### Output

```
F
```

!!! info
	**Wyjaśnienie**
	
	$1010_2+5_{10}=F_16$

## Zadanie 3

Napisz program zgodny z poniższą specyfikacją. Do reprezentacji liczb zespolonych i wykonywania na nich operacji wykorzystaj własną implementację klasy.
Operacje arytmetyczne, a także wczytywanie i wypisywanie liczb na ekran zrealizuj za pomocą **przeciążonych operatorów**.
Informacje na temat liczb zespolonych można znaleźć na stronie Wikipedii: [https://pl.wikipedia.org/wiki/Liczby_zespolone](https://pl.wikipedia.org/wiki/Liczby_zespolone)

### Specification

#### Input

* $re1, im1$ - część rzeczywista i urojona pierwszej liczby, liczby całkowite
* $op$ - znak operacji: $+$, $-$, $*$ lub $/$
* $re2, im2$ - część rzeczywista i urojona drugiej liczby, liczby całkowite

#### Output

* Wynik działania operacji $\Re{re1}+\Im{im1} op\ \Re{re2}+\Im{im2}$ przedstawiony w formacie `re + imi`, np. `3 + 4i`

### Example

#### Input

```
3 5
+
7 11
```

#### Output

```
10 + 16i
```

## Zadanie 4

Napisz program zgodny z poniższą specyfikacją. 
Dane przechowuj w tablicy dynamicznej, którą samodzielnie zaimplementujesz za pomocą klasy.
Zaimplementuj dostęp do danych za pomocą przeciążenia operatora **[]**.
Wszystkie arytmetyczne obliczenia zaimplementuj jako metody w klasie.
Zadbaj o czyszczenie pamięci przy użyciu destruktora klasy.

### Specification

#### Input

* $a1, a2, a3...$ - ciąg liczb całkowitych

#### Output

* Średnia, suma oraz mediana podanych liczb wypisane w odpowiednim komunikacie.

### Example

#### Input

```
1 2 3 4 5 6 7 8 9
```

#### Output

```
average = 5
sum = 45
median = 5
```