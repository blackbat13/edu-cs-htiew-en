# Wszystkie dzielniki

## [:link: Opis problemu](../../../../algorithms/integers/divisors.md)

## Solution zupełnie naiwne

### Implementation

```kotlin
fun printDivisors(n: Int) {
  for (i in 1 until n + 1) {
    if (n % i == 0) {
      println(i)
    }
  }
}

fun main() {
  val n = 12

  println("Dzielniki liczby $n:")
  printDivisors(n)
}
```

### Link do implementacji

[Wszystkie dzielniki - podejście zupełnie naiwne](https://ideone.com/hfECmZ)

### Description implementacji

TODO

## Solution naiwne

### Implementation

```kotlin
fun printDivisors(n: Int) {
  for (i in 1 until (n / 2) + 1) {
    if (n % i == 0) {
      println(i)
    }
  }

  if (n > 1) {
    println(n)
  }
}

fun main() {
  val n = 12

  println("Dzielniki liczby $n:")
  printDivisors(n)
}
```

### Link do implementacji

[Wszystkie dzielniki - podejście naiwne](https://ideone.com/iD7tJJ)

### Description implementacji

TODO

## Solution optymalne

### Implementation

```kotlin
import kotlin.math.sqrt

fun printDivisors(n: Int) {
  for (i in 1 until sqrt(n.toDouble()).toInt() + 1) {
    if (n % i == 0) {
      println(i)

      if (i != n / i) {
        println(n / i)
      }
    }
  }
}

fun main() {
  val n = 12

  println("Dzielniki liczby $n:")
  printDivisors(n)
}
```

### Link do implementacji

[Wszystkie dzielniki - podejście optymalne](https://ideone.com/m5v9Hi)

### Description implementacji

TODO
