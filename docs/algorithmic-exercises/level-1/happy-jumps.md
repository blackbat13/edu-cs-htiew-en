# Sequence differences

You are given a sequence of $n$ integers. Your task is to see if calculating the absolute values of the differences between each pair of consecutive elements of the sequence will yield all numbers from $1$ to $n-1$ inclusive.

Source: [https://onlinejudge.org/external/100/10038.pdf](https://onlinejudge.org/external/100/10038.pdf)

## Specification

### Input

* $n$ - natural number from the interval $[1,3000]$
* $tab[n]$ - sequence of $n$ integers

### Output

* "YES" if the sequence meets the requirement described above, or "NO" otherwise

## Example 1

### Input

```
4
1 4 2 3
```

### Output

```
YES
```

!!! info
	#### Explanation
	
	Let's look at the absolute values of the differences between adjacent elements of the sequence:
	
	* $|1-4|=3$
	* $|4-2|=2$
	* $|2-3|=1$
	
	As you can see, we obtained all values in the interval $[1,n-1]$, that is, in the interval $[1,3]$.

## Example 2

### Input

```
5
1 4 2 -1 6
```

### Output

```
NO
```

!!! info
	#### Explanation
	
	Let's look at the absolute values of the differences between adjacent elements of the sequence:
	
	* $|1-4|=3$
	* $|4-2|=2$
	* $|2-(-1)|=3$
	* $|-1-6|=7$
	
	As you can see, we did not get all the values in the interval $[1,n-1]$, that is, in the interval $[1,4]$
