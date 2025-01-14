# Sale

Topoland is home to a farmer named Vladimir, who sells milk, sourced from his healthy cows grazing in the lush meadows of the land. He recently introduced a special promotion: for giving away $3$ of empty milk bottles, you get a $1$ full bottle of milk free! How many bottles of milk are you able to consume using this promotion if you have already purchased $n$ bottles of milk?

PS. Vladimir will be happy to lend you empty bottles, provided you return them later.

Source: [https://onlinejudge.org/external/111/11150.pdf](https://onlinejudge.org/external/111/11150.pdf)

## Specification

### Input

* $n$ - The number of purchased bottles of milk from the range $[1,200]$

### Output

* The maximum number of bottles of milk that can be drunk using the promotion.

## Example

### Input

```
8
```

### Output

```
12
```

!!! info
	#### Explanation
	
	At the beginning we have $8$ full bottles of milk. If we borrow one empty bottle, we can exchange our $9$ of empty bottles for $3$ of new bottles. We drink $3$ bottles of milk and exchange them for one bottle of milk. We drink it too, and at the end we give back the empty bottle. So we drank first $8$, then $3$ and finally $1$ bottle of milk:
	
	$8+3+1=12$
