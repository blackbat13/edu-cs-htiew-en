# Solution 7

## Treść zadania

Napisz program zgodny z poniższą specyfikacją.

### Specification

#### Input

* $n$ - liczba naturalna

#### Output

* Wszystkie pary liczb naturalnych, których suma wynosi $n$

## Solution

```cpp
#include <iostream>

using namespace std;

int main() {
    int n;
    
    cout << "Podaj liczbe:" << endl;
    cin >> n;
    
    for (int i = 0; i <= n / 2; i++) {
        cout << "(" << i << ", " << n - i << ")" << endl;
    }
    
    return 0;
}
```
