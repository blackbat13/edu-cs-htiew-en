# Solution 8

## Treść zadania

Napisz program zgodny z poniższą specyfikacją.

### Specification

#### Input

* $sekundy$ - liczba naturalna

#### Output

* Czas podany w czytelnej formie ** **$H:M:S$ ($H$ - godziny, $M$ - minuty, $S$ - sekundy)

## Solution

```cpp
#include <iostream>

using namespace std;

int main() {
    int sekundy, godziny, minuty;
    
    cout << "Podaj liczbe sekund:" << endl;
    cin >> sekundy;
    
    godziny = sekundy / (60 * 60);
    
    sekundy = sekundy % (60 * 60);
    
    minuty = sekundy / 60;
    
    sekundy = sekundy % 60;
    
    cout << godziny << ":" << minuty << ":" << sekundy << endl;
    
    return 0;
}
```
