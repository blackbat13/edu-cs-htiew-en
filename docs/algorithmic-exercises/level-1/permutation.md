# Permutation

Arrays are the foundation of programming, and sorted arrays are one of its key elements. And what is a sorted array if not a certain **permutation** of the original array?

The permutation of an array can be characterized by indicating the target order of the individual elements of the array, as well as their original arrangement. Your task is to generate a permuted array based on such a defined description.

Source: [https://onlinejudge.org/external/4/482.pdf](https://onlinejudge.org/external/4/482.pdf)

## Specification

### Input

* $n$ - number of elements in the array
* $p_1,p_2,...,p_n$ - description of permutation: target order of elements, unique (without repetition) integers in the range $[1,n]$
* $a_1,a_2,...,a_n$ - values of the array in its initial arrangement, integers

### Output

* A given permutation of the array, i.e., such that the element $a_i$ is located at position $p_i$.

## Example

### Input

```
5
3 5 2 1 4
20 41 84 93 12
```

### Output

```
93 84 20 12 41  
```

!!! info
	#### Explanation
	
	The permutation description tells us the target position of the elements:
	
	* $20$ at position $3$
	* $41$ at position $5$
	* $84$ at position $2$
	* $93$ at position $1$
	* $12$ at position $4$
