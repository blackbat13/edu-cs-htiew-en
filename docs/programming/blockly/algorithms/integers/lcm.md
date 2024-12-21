---
description: Najmniejsza Wspólna Wielokrotność
---

# NWW

## Opis problemu

TODO

## Implementacja

### NWW

![Funkcja obliczająca NWW dwóch podanych liczb naturalnych](../../../../assets/NWW.png)

### NWD

Skoro mamy już policzone NWW, możemy na jego podstawie policzyć także NWD (Najmniejszy Wspólny Dzielnik), korzystając z prostego wzoru:

$$
NWD(a,b)=\frac{a*b}{NWW(a,b)}
$$

![Funkcja obliczająca NWD dwóch podanych liczb naturalnych na podstawie ich NWW](../../../../assets/NWW_NWD.png)

### Kod główny

Pozostaje nam tylko poprosić użytkownika o podanie danych i wywołać dwie pokazane wyżej funkcje.

![](../../../../assets/NWW_NWD_main.png)

### Link do implementacji

[Obliczanie NWW i NWD](https://blockly-demo.appspot.com/static/demos/code/index.html?lang=pl#35v83t)
