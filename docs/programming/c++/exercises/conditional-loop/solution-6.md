# Solution 6

## Treść zadania

Napisz program zgodny z poniższą specyfikacją.

### Specification

#### Input

* $n$ - liczba naturalna
* $p$ - liczba naturalna z zakresu $[2,9]$

#### Output

* Zapis liczby $n$ w systemie o podstawie $p$ 

## Solution

```cpp
#include <iostream>

using namespace std;

int main() {
    int n, p, cyfra;
    string nowa = "";
    
    cout << "Podaj liczbe dziesietna:" << endl;
    cin >> n;
    
    cout << "Podaj nowa podstawe:" << endl;
    cin >> p;
    
    while (n > 0) {
        cyfra = n % p;
        
        nowa = (char)(cyfra + '0') + nowa;
        
        n = n / p;
    }
    
    cout << "Po zamianie: " << nowa << endl;
    
    return 0;
}
```
