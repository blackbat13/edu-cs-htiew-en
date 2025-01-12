# Wyrazy

### Example 1

```awk
#!/usr/bin/awk -f

# Polecenia piszemy w nawiasach klamrowych
{
   # Wypisujemy pierwszy wyraz z kazdej linii
   print $1 
}
```

### Example 2

```awk
#!/usr/bin/awk -f

# Polecenia piszemy w nawiasach klamrowych
{
   # Wypisujemy kazda linie w okreslonym formacie
   print "username: " $1 "; IP: " $5 
}
```

### Example 3

```awk
#!/usr/bin/awk -f

# Polecenia piszemy w nawiasach klamrowych
{
   # Wypisujemy ostatni wyraz z kazdej linii
   print $NF 
}
```

### Example 4

```awk
#!/usr/bin/awk -f

# Dla przykladu stosujemy skrypt na wyniku polecenia date

# Na poczatku mozemy dac opcje konfiguracyjne

# OFS - Output Field Separator, czyli znak, ktorym oddzielamy dane na wyjsciu
OFS=":"

# Polecenia piszemy w nawiasach klamrowych
{
   print $2,$3,$4
}
```

### Example 5

```awk
#!/usr/bin/awk -f

# Uruchamiamy na pliki /etc/passwd

# FS - Field Separator, czyli znak oddzielajacy pola na wejsciu
FS=":"

# Polecenia piszemy w nawiasach klamrowych
{
   # Wypisujemy pierwszy wyraz z kazdej linii
   print $1 
}
```