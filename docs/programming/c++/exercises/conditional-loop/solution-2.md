# Solution 2

## Treść zadania

Napisz program zgodny z poniższą specyfikacją.

### Specification

#### Input

* $n$ - liczba naturalna

#### Output

* Suma cyfr liczby $n$

## Solution

```cpp
#include <iostream>

using namespace std;

int main() {
    int n, cyfra, suma;
    
    suma = 0;
    
    cout << "Podaj liczbe:" << endl;
    cin >> n;
    
    while (n > 0) {
        cyfra = n % 10;
        suma += cyfra;
        n = n / 10;
    }
    
    cout << "Suma cyfr podanej liczby wynosi " << suma << endl;
    
    return 0;
}
```
