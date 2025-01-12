# Pętle

## Pętla iteracyjna

### Example

```awk
#!/usr/bin/awk -f

BEGIN {
    for(i=1; i <= 10; i++) { 
        print i*i
    }
}
```

## Pętla warunkowa

### Example

```awk
#!/usr/bin/awk -f

BEGIN {
   i = 1
   while(i <= 10) {
      print i*i 
      i++
   }
      
}
```