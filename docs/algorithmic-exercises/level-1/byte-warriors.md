# Byte warriors

The structure of the Byte Warriors troop is organized in such a way that the first row consists of one warrior, the second of two, the third of three and so on. This means that each $i$th row consists of $i$ warriors.

Your task is to calculate the number of rows, knowing the total number of warriors in the troop. Note that there are not always enough warriors to fill the last row - for example, $6$ of warriors could be distributed in three rows, but similarly there could be $7$, $8$ or even $9$ of warriors distributed.

Source: [https://onlinejudge.org/external/116/11614.pdf](https://onlinejudge.org/external/116/11614.pdf)

## Specification

### Input

* $n$ - natural number, troop size, $0\leq n\leq 10^{18}$.

### Output

* The number of rows needed to form a troop.

## Example 1

### Input

```
3
```

**Output:** $2$

## Example 2

### Input

```
8
```

**Output:** $3$

## Example 3

### Input

```
10
```

**Output:** $4$
