# Newspaper

The Bitek newspaper of Bytebok is extremely popular, even in its traditional paper format. As a result, many people send their ads to the editors to be placed in the next issue. Until now, the rate has been simple: a fixed fee for each ad, depending on the number of characters. However, the publisher of "Bitek" noticed that different signs use different amounts of ink, which means that the printing costs for each of them are also different! Therefore, he decided to update the price list and set the cost of printing each sign. Now the charge for an ad is equal to the sum of the costs of all the signs included in a given ad.

Your task is to calculate how much the fee for a particular ad will be according to the new price list.

Source: [https://onlinejudge.org/external/113/11340.pdf](https://onlinejudge.org/external/113/11340.pdf)

## Specification

### Input

* $n$ - number of characters
* $(z_1, c_1), (z_2, c_2), ..., (z_n, c_n)$ - price list: sign pairs and sign price, given in pennies
* $word$ - a string of characters, lowercase and/or uppercase letters of the English alphabet, without spaces or other whitespace characters

### Output

* The fee for $word$, given in zlotys, according to the new price list. We assume that each character from the word will appear in the price list.

## Example

### Input

```
6
a 5
l 25
m 30
k 50
o 10
t 1
alamakota
```

### Output

```
1.36
```

!!! info
	#### Explanation
	
	In the word **alamakota** we can distinguish:
	
	* $4$ letters **a**
	* $1$ letter **l**
	* $1$ letter **m**
	* $1$ letters **k**
	* $1$ letter **o**
	* $1$ letter **t**
	
	It gives us: $4*5+1*25+1*30+1*50+1*10+1*1=136$ pennies, i.e. $1.36$ polish złoty.
