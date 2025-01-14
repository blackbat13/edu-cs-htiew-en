# Image coding

Computer graphics is an extremely important area of computer science. Since we store a lot of images on computers, it is important to represent them efficiently in computer memory. In this assignment, we will focus on a special case of encoding graphics. We represent graphics as a rectangular array of letters of the English alphabet, where each letter encodes one region. Identical regions are represented by the same letters.

Your task is to calculate how many bytes of memory are needed to represent the graphic presented in this way. The rules are simple: the highest priority region is represented with 2 bytes, while all other regions are represented with one byte.

The area with the **highest** priority is the one that occurs **most often**, that is, the letter representing this area appears the most times in the description of the graphic. If several areas have the same highest number of occurrences, we consider all of them to be the highest priority areas.

Source: [https://onlinejudge.org/external/115/11588.pdf](https://onlinejudge.org/external/115/11588.pdf)

## Specification

### Input

* $h, w$ - dimensions of the board, its height and width
* $pix[h][w]$ - oGraphic writing, a two-dimensional array of $h\times w$, each element of which is a capital letter of the English alphabet

### Output

* The number of bytes needed to represent the specified graphic

## Example

### Input

```
1
5 4
ABCD
ABCA
EFAC
BCAG
AZIP
```

### Output

```
26
```

!!! info
	#### Explanation
	
	The most frequently occurring region is the **A** region. It occurs exactly $6$ times. This means that we encode the **A** region with $2$ bytes, and all the others (of which there are $14$), with $1$ bytes. Hence, we get the result: $6*2 + 14*1 = 12 + 14 = 26$
