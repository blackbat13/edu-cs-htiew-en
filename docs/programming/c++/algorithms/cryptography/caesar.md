# Szyfr Cezara

## [:link: Opis problemu](../../../../algorithms/cryptography/symmetric/caesar.md)

## Szyfrowanie

### Implementacja

```cpp linenums="1"
#include <iostream>

using namespace std;

string encryptCaesar(string message, int key) {
    string result = "";
    char encrypted;
    
    key %= 26;
    
    for(char letter : message) {
        encrypted = letter + key;
        if(encrypted > 'z') {
            encrypted = encrypted - 'z' + 'a' - 1;
        }
        
        result += encrypted;
    }
    
    return result;
}

int main() {
    string message = "alamakota";
    int key = 3;
    
    string encrypted = encryptCaesar(message, key);
    
    cout << encrypted << endl;
    
    return 0;
}
```

## Deszyfrowanie

### Implementacja

```cpp linenums="1"
#include <iostream>

using namespace std;

string decryptCaesar(string encrypted, int key) {
    string result = "";
    char decrypted;
    
    key %= 26;
    
    for(char letter : encrypted) {
        decrypted = letter - key;
        if(decrypted < 'a') {
            decrypted = 'z' - ('a' - decrypted - 1);
        }
        
        result += decrypted;
    }
    
    return result;
}

int main() {
    string encrypted = "dodpdnrwd";
    int key = 3;
    
    string decrypted = decryptCaesar(encrypted, key);
    
    cout << decrypted << endl;
    
    return 0;
}
```
