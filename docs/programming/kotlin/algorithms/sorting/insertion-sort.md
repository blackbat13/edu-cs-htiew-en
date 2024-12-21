# Sortowanie przez wstawianie

## [:link: Opis problemu](../../../../algorithms/sorting/insertion-sort.md)

## Implementacja

```kotlin
fun insertionSort(array: MutableList<Int>) {
    for (i in 1 until array.count()) {
        var j = i
        while (j > 0 && array[j] < array[j - 1]) {
            val tmp = array[j]
            array[j] = array[j - 1]
            array[j - 1] = tmp
            j--
        }
    }
}

fun main() {
    val array = mutableListOf(7, 3, 0, 1, 5, 2, 5, 19, 10, 5)

    insertionSort(array)

    println(array)
}
```

### Link do implementacji

[Sortowanie przez wstawianie](https://ideone.com/g6l7oJ)