# Sortowanie bąbelkowe

## [:link: Opis problemu](../../../../algorithms/sorting/bubble-sort.md)

## Implementacja

```julia linenums="1"
function bubbleSort(array)
    sorted = false
    i = 2
    while !sorted
        sorted = true
        for j = length(array):-1:i
            if array[j] < array[j-1]
                array[j], array[j-1] = array[j-1], array[j]
                sorted = false
            end
        end

        i += 1
    end
end

array = [7, 3, 0, 1, 5, 2, 5, 19, 10, 5]

bubbleSort(array)

println(array)
```

### Opis implementacji

Zaczynamy od utworzenia funkcji sortującej *bubbleSort* (**linia 1**), która przyjmuje jeden argument: listę elementów do posortowania.

Wewnątrz funkcji tworzymy zmienne pomocnicze do pamiętania, czy lista jest już posortowana (**linia 2**) oraz do pamiętania liczby posortowanych elementów (**linia 3**). Następnie uruchamiamy pętlę, która będzie wykonywać operacje aż do posortowania całej listy (**linia 4**). W pętli na początku zakładamy, że lista została już posortowana (**linia 5**), a następnie zaczynamy kolejną pętlę przechodzącą indeksami od końca tablicy do jej początku, uwzględniając liczbę posortowanych już elementów (**linia 6**). W tej zagnieżdżonej pętli porównujemy ze sobą sąsiednie elementy listy (**linia 7**), a gdy są ułożone niezgodnie z porządkiem sortowania, to zamieniamy je miejscami (**linia 8**). Zapamiętujemy także, że lista nie została jeszcze posortowana, ponieważ dokonaliśmy zamiany (**linia 9**). Po wyjściu z zagnieżdżonej pętli zwiększamy licznik posortowanych elementów (**linia 13**).

W części głównej tworzymy listę do sortowania (**linia 18**), sortujemy ją wywołując naszą funkcję sortującą *bubbleSort* (**linia 20**) i wypisujemy posortowaną listę na ekranie (**linia 22**).
