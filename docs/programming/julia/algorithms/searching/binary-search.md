# Wyszukiwanie binarne

## [:link: Opis problemu](../../../../algorithms/searching/binary-search.md)

## Wersja iteracyjna

### Implementacja

```julia linenums="1"
function binarySearch(array, number)
    left = 1
    right = length(array)

    while left <= right
        middle = (left + right) ÷ 2

        if number < array[middle]
            right = middle
        elseif number > array[middle]
            left = middle + 1
        else
            return middle
        end
    end

    return -1
end

array = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
number = 8

println(binarySearch(array, number))
```
