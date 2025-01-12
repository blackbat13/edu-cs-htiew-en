# Nawiasy

Dany jest ciąg złożony z nawiasów okrągłych () oraz kwadratowych []. Twoim celem jest sprawdzenie, czy ciąg zawiera **poprawne nawiasowanie**, czy też nie. Ciąg uznajemy za **poprawny**, gdy:

* jest pustym ciągiem,
* jeżeli $A$ i $B$ są poprawne, to $AB$ także jest poprawne,
* jeżeli $A$ jest poprawne, to $(A)$ oraz $[A]$ także są poprawne.

Źródło: [https://onlinejudge.org/external/6/673.pdf](https://onlinejudge.org/external/6/673.pdf)

## Specification

### Wejście

* $par$ - ciąg nawiasów

### Wyjście

* Informacja, czy ciąg jest poprawny, czy też nie.

## Example 1

### Wejście

```
([])
```

### Wyjście

```
Correct
```

## Example 2

### Wejście

```
(([()])))
```

### Wyjście

```
Incorrect
```

## Example 3

### Wejście

```
([()[]()])()
```

### Wyjście

```
Correct
```