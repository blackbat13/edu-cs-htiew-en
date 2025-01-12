# Solution 5

## Treść zadania

Napisz program zgodny z poniższą specyfikacją.

### Specification

#### Input

* $n$ - liczba naturalna

#### Output

* Zapis binarny liczby $n$

## Solution

```cpp
#include <iostream>

using namespace std;

int main() {
    int n, cyfra;
    string binarna = "";
    
    cout << "Podaj liczbe:" << endl;
    cin >> n;
    
    while (n > 0) {
        cyfra = n % 2;
        
        binarna = (char)(cyfra + '0') + binarna;
        
        n = n / 2;
    }
    
    cout << "Wartosc binarna: " << binarna << endl;
    
    return 0;
}
```
