# Cięcie kosztów

W ramach przeprowadzanej przez pewną firmę redukcji zatrudnienia, pracownicy działający w trzyosobowych zespołach podlegają ocenie. Zarobki w obrębie każdego zespołu mogą się różnić. Zarząd firmy podjął decyzję, że z każdego zespołu zwolnione zostaną dwie osoby o skrajnych zarobkach - osoba zarabiająca najmniej oraz osoba zarabiająca najwięcej. Twoim zadaniem jest określenie, kto przetrwa redukcję i pozostanie zatrudniony w zespole.

Source: [https://onlinejudge.org/external/117/11727.pdf](https://onlinejudge.org/external/117/11727.pdf)

## Specification

### Input

* $a,b,c$ - trzy liczby naturalne określające zarobki pracowników, wszystkie w zakresie $[1000, 10000]$

### Output

* Zarobki pracownika, który pozostanie zatrudniony

## Example

### Input

```
a := 1500
b := 1200
c := 1800
```

**Output:** $1500$

!!! info
    #### Explanation

    Najmniejsza z wartości to $1200$, a największa do $1800$, pozostaje więc $1500$.
