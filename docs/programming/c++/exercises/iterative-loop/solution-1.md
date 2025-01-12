# Solution 1

## Treść zadania

Napisz program zgodny z poniższą specyfikacją.

### Specification

#### Input

* $n$ - liczba naturalna

#### Output

* $n!$ 

## Solution

```cpp
#include <iostream>

using namespace std;

int main() {
    int n, silnia;
    
    silnia = 1;
    
    cout << "Podaj liczbe:" << endl;
    cin >> n;
    
    for (int i = 2; i <= n; i++) {
        silnia *= i;
    }
    
    cout << n << "! = " << silnia << endl;
    
    return 0;
}
```
