# Solution 4

## Treść zadania

Napisz program zgodny z poniższą specyfikacją.

### Specification

#### Input

* $a, b$ - dwie liczby naturalne, większe od zera

#### Output

* Wynik dzielenia całkowitego oraz reszta z dzielenia liczb $a$ i $b$ 

## Solution

```cpp
#include <iostream>

using namespace std;

int main() {
    int a, b, div, mod;
    
    cout << "Podaj dwie liczby:" << endl;
    cin >> a >> b;
    
    div = a / b;
    mod = a % b;
    
    cout << a << " / " << b << " = " << div << ", r. " << mod << endl;
    
    return 0;
}
```
