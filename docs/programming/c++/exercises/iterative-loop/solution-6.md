# Solution 6

## Treść zadania

Napisz program zgodny z poniższą specyfikacją.

### Specification

#### Input

* $n$ - liczba naturalna

#### Output

* Tabliczka mnożenia z zakresu $[1,n]$

## Solution

```cpp
#include <iostream>

using namespace std;

int main() {
    int n;
    
    cout << "Podaj liczbe:" << endl;
    cin >> n;
    
    for (int i = 1; i <= n; i++) {
        for (int j = 1; j <= n; j++) {
            cout << i * j << " ";
        }
        
        cout << endl;
    }
    
    return 0;
}
```
