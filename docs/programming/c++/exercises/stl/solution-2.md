# Solution 2

Napisz program zgodny z poniższą specyfikacją. W implementacji wykorzystaj klasę `stack`.

### Specification

#### Input

* $nawiasy$ - ciąg składający się jedynie ze znaków reprezentujących nawiasy okrągłe i kwadratowe, tzn.: $(, ), [, ]$

#### Output

* **TRUE** jeżeli podany na wejściu ciąg jest reprezentacją poprawnego nawiasowania, **FALSE** w przeciwnym przypadku.

## Solution

```cpp
#include <iostream>
#include <stack>

using namespace std;

int main() {
    string brackets;
    stack<char> st;
    bool ok = true;
    
    cin >> brackets;

    for (auto ch : brackets) {
        if (ch == '(' || ch == '[') {
            st.push(ch);
        } else if (ch == ']') {
            if (st.empty() || st.top() != '[') {
                ok = false;
                break;
            }

            st.pop();
        } else {
            if (st.empty() || st.top() != '(') {
                ok = false;
                break;
            }

            st.pop();
        }
    }

    if (ok) {
        cout << "TRUE" << endl;
    } else {
        cout << "FALSE" << endl;
    }

    return 0;
}
```