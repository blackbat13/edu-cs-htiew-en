# Different digits

Your task is to determine the number of numbers in a given range that consist only of unique digits, that is, in their notation the digits do not repeat. For example, the number $123$ consists of different digits, while the number $100$ no longer does, due to the repeating character $0$.

Source: [https://onlinejudge.org/external/125/12527.pdf](https://onlinejudge.org/external/125/12527.pdf)

## Specification

### Input

* $a, b$ - integers in the interval $[1,5000]$

### Output

* The number of all numbers in the interval $[a,b]$ that consist only of different digits.

## Example

### Input

```
87 104
```

### Output

```
14
```

!!! info
	#### Explanation
	
	From the interval $[87,104]$ the following numbers consist only of different digits:
	
	$87,89,90,91,92,93,94,95,96,97,98,102,103,104$
