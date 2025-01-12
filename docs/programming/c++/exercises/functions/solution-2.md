# Solution 2

## Treść zadania

Napisz program zgodny z poniższą specyfikacją. Obliczanie sumy powinno być zrealizowane za pomocą funkcji.

### Specification

#### Input

* $a, b$ - dwie liczby całkowite

#### Output

* Suma liczb $a$ i $b$ 

## Solution

```cpp
#include <iostream>

using namespace std;

int suma(int a, int b) {
    return a + b;
}

int main() {
    int a, b, wynik;
    
    cout << "Podaj dwie liczby:" << endl;
    cin >> a >> b;
    
    wynik = suma(a, b);
    
    cout << a << " + " << b << " = " << wynik << endl;
    
    return 0;
}
```
