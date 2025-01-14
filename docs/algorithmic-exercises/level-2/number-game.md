# Gra w liczby

Wyobraź sobie prostą grę dla dzieci: masz kilka liczb, zapisanych na osobnych kartach, a twoim zadaniem jest ułożenie tych kart obok siebie tak, aby utworzyły jak największą możliwą liczbę.

Weźmy na przykład trzy liczby: $90$, $101$ oraz $3$.
Istnieje wiele sposobów na ich połączenie, co prowadzi do utworzenia nowych liczb: $901013$, $903101$, $101903$, $101390$, $310190$ oraz $390101$.
Jak możemy zauważyć, mamy tu do dyspozycji $6$ kombinacji. Największa liczba, którą możemy w ten sposób uzyskać to $903101$. Twoim celem jest znalezienie takiej największej liczby i wygranie gry!

Source: [https://onlinejudge.org/external/109/10905.pdf](https://onlinejudge.org/external/109/10905.pdf)

## Specification

### Input

* $n$ - liczba naturalna
* $a_1, a_2, ..., a_n$ - $n$ liczb naturalnych

### Output

* Największa liczba jaka może zostać utworzona poprzez połączenie ze sobą liczb $a_1, a_2, ..., a_n$ w wybranym porządku.

## Example 1

### Input

```
4
123 124 56 90
```

### Output

```
9056124123
```

## Example 2

### Input

```
5
123 124 56 90 9 
```

### Output

```
99056124123
```
