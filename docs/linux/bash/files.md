# Pliki

## Czytanie plików

### Example

```bash
#!/bin/bash

wynik=`cat wynik.txt`
echo "$wynik"
```

## Pisanie do plików

### Example

```bash
#!/bin/bash

plik=wynik.txt

# Przekierowujemy wynik polecenia ls do pliku
ls -la> $plik

cat $plik
```