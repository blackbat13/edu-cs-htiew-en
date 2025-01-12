# Solution 2

## Treść zadania

Napisz program zgodny z poniższą specyfikacją.

### Specification

#### Input

* $a$ - liczba całkowita

#### Output

* Znak liczby $a$, tzn. $1$ gdy $a$ jest dodatnie, $-1$ gdy $a$ jest ujemne, $0$ gdy $a$ wynosi $0$ 

## Solution

```cpp
#include <iostream>

using namespace std;

int main() {
    int a;
    
    cout << "Podaj liczbe:" << endl;
    cin >> a;
    
    cout << "Znak podanej liczby: ";
    if (a < 0) {
        cout << -1 << endl;
    } else if (a > 0) {
        cout << 1 << endl;
    } else {
        cout << 0 << endl;
    }
    
    return 0;
}
```
