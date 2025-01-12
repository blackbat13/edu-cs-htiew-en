# Problem bankomatu (wydawanie reszty)

Problem bankomatu, czy też problem wydawania reszty, to problem, w którym zadajemy sobie następujące pytanie: ile co najmniej monet i/lub banknotów potrzeba do wydania zadanej kwoty?

## Specification

### Input

* $n$ — liczba naturalna, ilość dostępnych nominałów
* $nominały[1..n]$ — tablica dostępnych nominałów (liczb całkowitych) o rozmiarze $n$
* $kwota$ — liczba naturalna, kwota do wydania

### Output

* Minimalna liczba potrzebnych monet i/lub banknotów do wydania podanej kwoty przy użyciu dostępnych nominałów.

## Example 1

### Input

```
n := 4
nominały := [1, 2, 5, 10]
kwota := 28
```

### Output

Minimalna liczba potrzebnych monet i/lub banknotów: $5$.

Wykorzystane monety/banknoty: $1, 2, 5, 10, 10$

## Example 2

### Input

```
n := 3
nominały := [1, 7, 10]
kwota := 14
```

### Output

Minimalna liczba potrzebnych monet i/lub banknotów: $2$.

Wykorzystane monety/banknoty: $7, 7$
