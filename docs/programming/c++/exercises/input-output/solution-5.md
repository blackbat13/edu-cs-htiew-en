# Solution 5

## Treść zadania

Napisz program zgodny z poniższą specyfikacją.

### Specification

#### Input

* $a$ - liczba naturalna

#### Output

* Pierwiastek z $a$

## Solution

```cpp
#include <iostream>
#include <cmath>

using namespace std;

int main() {
    int a;
    double pierwiastek;
    
    cout << "Podaj liczbe:" << endl;
    cin >> a;
    
    pierwiastek = sqrt(a);
    
    cout << "Pierwiastek z " << a << " = " << pierwiastek << endl;
    
    return 0;
}
```
