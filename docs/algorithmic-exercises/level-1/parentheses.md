# Parentheses

Given a string composed of round brackets () and square brackets []. Your goal is to check whether the string contains **correct parentheses** or not. We consider a string to be **correct** when:

* is an empty string,
* if $A$ and $B$ are correct, then $AB$ is also correct,
* if $A$ is correct, then $(A)$ and $[A]$ are also correct.

Source: [https://onlinejudge.org/external/6/673.pdf](https://onlinejudge.org/external/6/673.pdf)

## Specification

### Input

* $par$ - string of parentheses

### Output

* Information whether the string is correct or not.

## Example 1

### Input

```
([])
```

### Output

```
Correct
```

## Example 2

### Input

```
(([()])))
```

### Output

```
Incorrect
```

## Example 3

### Input

```
([()[]()])()
```

### Output

```
Correct
```