# Płatek Kocha

Płatek Kocha to fraktal stworzony poprzez złożenie ze sobą trzech krzywych Kocha, tak że razem tworzą strukturę przypominającą płatek śniegu.

## Specification

### Input

* $stopień$ - stopień fraktala
* $długość$ - długość linii

### Output

* Płatek Kocha stopnia $stopień$ i długości $długość$.

## Solution

### Pseudocode

```
procedura KrzywaKocha(stopień, długość):
    1. Jeżeli stopień = 0, to:
        2. Przód(długość)
        3. Zakończ
    4. KrzywaKocha(stopień - 1, długość)
    5. Lewo(60)
    6. KrzywaKocha(stopień - 1, długość)
    7. Prawo(120)
    8. KrzywaKocha(stopień - 1, długość)
    9. Lewo(60)
    10. KrzywaKocha(stopień - 1, długość)
```

```
procedura PłatekKocha(stopień, długość):
    1. Dla i := 1 do 3, wykonuj:
        2. KrzywaKocha(stopień, długość)
        3. Prawo(120)
```

### Block diagram

```mermaid
%%{init: {"flowchart": {"curve": "linear"}, "theme": "neutral"} }%%
flowchart TD
    START(["KrzywaKocha(stopień, długość"]) --> K1{stopień = 0}
    K1 -- TRUE --> K2["Przód(długość)"]
    K2 --> STOP([STOP])
    K1 -- FALSE --> K4["KrzywaKocha(stopień - 1, długość)
    Lewo(60)
    KrzywaKocha(stopień - 1, długość)
    Prawo(120)
    KrzywaKocha(stopień - 1, długość)
    Lewo(60)
    KrzywaKocha(stopień - 1, długość)"]
    K4 --> STOP
```

```mermaid
%%{init: {"flowchart": {"curve": "linear"}, "theme": "neutral"} }%%
flowchart TD
    START(["PłatekKocha(stopień, długość"]) --> K0[i := 1]
    K0 --> K1{i <= 3}
    K1 -- TRUE --> K2["KrzywaKocha(stopień, długość)
    Prawo(120)"]
    K2 --> K1i[i := i + 1]
    K1i --> K1
    K1 -- FALSE ---> STOP([STOP])
```

## Implementation

### [:simple-cplusplus: C++](../../programming/c++/algorithms/fractals/koch-snowflake.md){ .md-button }

### [:simple-python: Python](../../programming/python/algorithms/fractals/koch-snowflake.md){ .md-button }

### [Blockly](../../programming/blockly/algorithms/fractals/koch-snowflake.md){ .md-button }
