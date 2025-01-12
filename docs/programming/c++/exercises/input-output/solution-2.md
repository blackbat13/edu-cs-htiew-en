# Solution 2

## Treść zadania

Napisz program zgodny z poniższą specyfikacją.

### Specification

#### Input

* $a, b$ - dwie liczby całkowite

#### Output

* Suma liczb $a$ i $b$ 

## Solution

```cpp
#include <iostream>

using namespace std;

int main() {
    int a, b, suma;
    
    cout << "Podaj dwie liczby:" << endl;
    cin >> a >> b;
    
    suma = a + b;
    
    cout << a << " + " << b << " = " << suma << endl;
    return 0;
}
```
