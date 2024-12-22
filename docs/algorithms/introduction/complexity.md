# Complexity

**Complexity** is a very important element in the discussion of algorithms. It is often the key factor by which we compare the **efficiency** of two solutions/algorithms. We distinguish primarily between:

* **time/computation complexity** - i.e. how many operations, depending on the size of the input data, the program must perform,
* **memory complexity** - how much memory (depending on the size of the input data) the program needs.

In this course, we will not discuss or calculate the exact complexity of algorithms. We will focus on their **estimated pessimistic complexity**.

Therefore, we will not go deep into mathematical details. If you are interested, I refer you to external sources, such as:

* [https://pl.wikipedia.org/wiki/Z%C5%82o%C5%BCono%C5%9B%C4%87\_obliczeniowa](https://pl.wikipedia.org/wiki/Z%C5%82o%C5%BCono%C5%9B%C4%87\_obliczeniowa)
* [https://pl.wikipedia.org/wiki/Asymptotyczne_tempo_wzrostu](https://pl.wikipedia.org/wiki/Asymptotyczne_tempo_wzrostu)

## Big O notation (asymptotic)

Here we will not go into the details of the asymptotic notation of large O. In a nutshell, we will use it to determine the **pesimistic** time complexity of the algorithm. For example, if an algorithm has a complexity of $O(n)$ this means that in the worst case it will run linearly with respect to the size of the data. Of course, it toes not exclude to situations in which such an algorithm will work faster.

## Basic complexity classes

| Zapis            | Nazwa                                   | Przykład                               |
| ---------------- | --------------------------------------- | -------------------------------------- |
| $O(1)$         | constant                                   | Checking the triangle condition           |
| $O(\log{n})$   | logarithmic                           | Binary search                   |
| $O(n)$         | linear                                 | Linear search                  |
| $O(n\log{n})$  | linear logarithmic                   | Merge sort              |
| $O(n^2)$       | square                              | Bubble sort                   |
| $O(n^3)$       | cubic                              | Floyda-Warshall algorithm              |
| $O(n^k)$       | polynomial ( $k$ - constant, $k>1$ ) | -                                      |
| $O(n!)$        | n-factorial                                | Listing all permutations of the set |
| $O(2^n)$       | exponential                             | Listing all subsets of the set |

## Complexity estimation

### Example - linear complexity

```
1. From i := 1 to n, do:
    2. Print i
```

### Example - quadratic complexity

```
1. From i := 1 to n, do:
    2. From j := 1 to n, do:
        3. Print i * j
```

### Example - cubic complexity

```
1. From i := 1 to n, do:
    2. From j := 1 to n, do:
        3. From k := 1 to n, do:
            4. Print i * j * k
```

### Example - logarithmic complexity

```
1. While n > 0, do:
    2. Print n
    3. n := n div 2
```

!!! info
    **div** means integer division

## Cheatsheet

[https://github.com/ro31337/bigoposter/blob/master/bigoposter.pdf](https://github.com/ro31337/bigoposter/blob/master/bigoposter.pdf)
