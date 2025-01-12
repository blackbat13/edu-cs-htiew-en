# Instrukcje warunkowe

### Example 1

```awk
#!/usr/bin/awk -f

{
   if($2==$3) {
      
   } else {
      print $0
   }    
}
```