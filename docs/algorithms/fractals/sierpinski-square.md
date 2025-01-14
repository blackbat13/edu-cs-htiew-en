# Kwadrat Sierpińskiego

**Kwadrat Sierpińskiego** (inaczej **Dywan Sierpińskiego**), to fraktal podobny do Trójkąta Sierpińskiego. Główna różnica jest taka, że podstawową figurą jest kwadrat.

## Specification

### Input

- **stopień** - stopień kwadratu Sierpińskiego
- **długość** - długość boku głównego kwadratu

## Solution

### Pseudocode

```
procedura KwadratSierpińskiego(stopień, długość):
    1. Jeżeli stopień = 0, to:
        2. Dla i := 1 do 4, wykonuj:
            3. Przód(długość)
            4. Lewo(90)
        5. Zakończ
    6. Dla i := 1 do 4, wykonuj:
        7. Dla j := 1 do 2, wykonuj:
            8. Przód(długość / 3)
            9. KwadratSierpińskiego(stopień - 1, długość / 3)
        10. Przód(długość / 3)
        11. Lewo(90)
```

### Block diagram

```mermaid
%%{init: {"flowchart": {"curve": "linear"}, "theme": "neutral"} }%%
flowchart TD
    START(["KwadratSierpińskiego(stopień, długość)"]) --> K1{stopień = 0}
    K1 -- TRUE --> K2p[i := 1]
    K2p --> K2{i <= 4}
    K2 -- TRUE --> K3["Przód(długość)
    Lewo(90)"]
    K3 --> K2i[i := i + 1]
    K2i --> K2
    K2 -- FALSE --> STOP([STOP])
    K1 -- FALSE --> K6p[i := 1]
    K6p --> K6{i <= 4}
    K6 -- TRUE --> K7p[j := 1]
    K7p --> K7{j <= 2}
    K7 -- TRUE --> K8["Przód(długość / 3)
    KwadratSierpińskiego(stopień - 1, długość / 3)"]
    K8 --> K7i[j := j + 1]
    K7i --> K7
    K7 -- FALSE --> K10["Przód(długość / 3)
    Lewo(90)"]
    K10 --> K6i[i := i + 1]
    K6i --> K6
    K6 -- FALSE ---> STOP
```

## Implementation

### [:simple-cplusplus: C++](../../programming/c++/algorithms/fractals/sierpinski-square.md){ .md-button }

### [:simple-python: Python](../../programming/python/algorithms/fractals/sierpinski-square.md){ .md-button }

### [Blockly](../../programming/blockly/algorithms/fractals/sierpinski-square.md){ .md-button }
