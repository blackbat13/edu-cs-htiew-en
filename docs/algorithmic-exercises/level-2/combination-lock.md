# Kłódka

Czas zająć się projektowaniem Escape Roomu, a kłódki szyfrowe czekają na swoją kolej. W swoim magazynie posiadasz kłódki z okrągłą tarczą, takie jak na zdjęciu poniżej. Tarcza kłódki składa się z $40$ przedziałek, które są numerowane od $0$ do $39$. Kombinacja do kłódki składa się z trzech liczb z tego zakresu.

![Thegreenj, CC BY-SA 3.0 <http://creativecommons.org/licenses/by-sa/3.0/>, via Wikimedia Commons](https://upload.wikimedia.org/wikipedia/commons/a/a1/Masterpadlock.jpg)

Aby otworzyć kłódkę, należy postępować zgodnie z poniższym schematem:

* Obróć tarczę dwa razy w pełnym obwodzie zgodnie z ruchem wskazówek zegara.
* Kontynuując ruch, zatrzymaj się na pierwszej liczbie z kombinacji.
* Wykonaj pełny obrót tarczy przeciwnie do ruchu wskazówek zegara.
* Kontynuując ruch, zatrzymaj się na drugiej liczbie z kombinacji.
* Następnie obróć tarczę zgodnie z ruchem wskazówek zegara, zatrzymując się na trzeciej liczbie z kombinacji.
* Teraz możesz pociągnąć za zamek i otworzyć kłódkę.

Twoim zadaniem jest wyliczenie, o ile stopni musisz łącznie obrócić tarczę, aby otworzyć kłódkę. Te informacje przydadzą się przy tworzeniu jednej z zagadek w Escape Roomie!

Source: [https://onlinejudge.org/external/105/10550.pdf](https://onlinejudge.org/external/105/10550.pdf)

## Specification

### Input

* $p$ - liczba naturalna, początkowe ustawienie tarczy, $0\leq p\leq 39$.
* $c1$ - liczba naturalna, pierwsza liczba kombinacji, $0\leq c1\leq 39$.
* $c2$ - liczba naturalna, druga liczba kombinacji, $0\leq c2\leq 39$.
* $c3$ - liczba naturalna, trzecia liczba kombinacji, $0\leq c3\leq 39$.

### Output

* Liczba naturalna oznaczająca łączną liczbę stopni, o które należy obrócić tarczę, by otworzyć kłódkę.

## Example 1

### Input

```
0 30 0 30
```

**Output:** $1350$

## Example 2

### Input

```
5 35 5 35
```

**Output:** $1350$

## Example 3

### Input

```
0 20 0 20
```

**Output:** $1620$

## Example 4

### Input

```
7 27 7 27
```

**Output:** $1620$

## Example 5

### Input

```
0 10 0 10
```

**Output:** $1890$

## Example 6

### Input

```
9 19 9 19
```

**Output:** $1890$
