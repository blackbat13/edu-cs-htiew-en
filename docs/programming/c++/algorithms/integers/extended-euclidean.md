# Rozszerzony algorytm Euklidesa

## [:link: Opis problemu](../../../../algorithms/integers/extended-euclidean.md)

## Implementacja

```cpp linenums="1"
#include <iostream>

using namespace std;

int extendedGCD(int a, int b, int &x, int &y) {
  int tmp, quotient, oldX = 1, rest = b, oldRest = a, oldY = 0;
  x = 0;
  y = 1;
  while (rest != 0) {
    quotient = oldRest / rest;

    tmp = rest;
    rest = oldRest - quotient * tmp;
    oldRest = tmp;

    tmp = x;
    x = oldX - quotient * tmp;
    oldX = tmp;

    tmp = y;
    y = oldY - quotient * tmp;
    oldY = tmp;
  }

  y = oldY;
  x = oldX;

  return oldRest;
}

int main() {
  int a = 6;
  int b = 21;
  int x, y, result;

  result = extendedGCD(a, b, x, y);

  cout << a << " * " << x << " + " << b << " * " << y << " = " << result
       << endl;

  return 0;
}
```
