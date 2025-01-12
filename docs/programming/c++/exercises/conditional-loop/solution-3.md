# Solution 3

## Treść zadania

Napisz program zgodny z poniższą specyfikacją.

### Specification

#### Input

* $n$ - liczba naturalna

#### Output

* Liczba powstała poprzez odwrócenie cyfr liczby $n$

## Solution

```cpp
#include <iostream>

using namespace std;

int main() {
    int n, cyfra, odwrocona;
    
    odwrocona = 0;
    
    cout << "Podaj liczbe:" << endl;
    cin >> n;
    
    while (n > 0) {
        cyfra = n % 10;
        
        odwrocona *= 10;
        odwrocona += cyfra;
        
        n = n / 10;
    }
    
    cout << "Odwrocona liczba: " << odwrocona << endl;
    
    return 0;
}
```
