# Sortowanie przez zliczanie

## [:link: Opis problemu](../../../../algorithms/sorting/counting-sort.md)

## Implementacja

```kotlin
fun countOccurrences(array: MutableList<Int>, maxNumber: Int): Array<Int> {
    val occurrences = Array<Int>(maxNumber + 1){0}

    for (number in array) {
        occurrences[number]++
    }
        
    return occurrences
}

fun countingSort(array: MutableList<Int>) {
    val occurrences = countOccurrences(array, 100)
    var index = 0
    
    for (i in occurrences.indices) {
        for (j in 1..occurrences[i]) {
            array[index] = i
            index++
        }
    }
}

fun main() {
    val array = mutableListOf(7, 3, 0, 1, 5, 2, 5, 19, 10, 5)

    countingSort(array)

    println(array)
}
```

### Link do implementacji

[Sortowanie przez zliczanie](https://ideone.com/Vcw5BN)