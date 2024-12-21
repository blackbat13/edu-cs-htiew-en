# Płatek Kocha

## [:link: Opis problemu](../../../../algorithms/fractals/koch-snowflake.md)

## Implementacja 

```python linenums="1"
import turtle

def koch_curve(rank, length):
    if rank > 0:
        koch_curve(rank - 1, length / 2)
        turtle.left(60)
        koch_curve(rank - 1, length / 2)
        turtle.right(120)
        koch_curve(rank - 1, length / 2)
        turtle.left(60)
        koch_curve(rank - 1, length / 2)
    else:
        turtle.forward(length)

def koch_snowflake(rank, length):
    for i in range(0, 3):
        koch_curve(rank, length)
        turtle.right(120)

turtle.speed(0)
turtle.penup()
turtle.back(350)
turtle.pendown()

koch_snowflake(3, 100)

turtle.done()
```

### Link do implementacji

[https://replit.com/@damiankurpiewski/Koch-Snowflake#main.py](https://replit.com/@damiankurpiewski/Koch-Snowflake#main.py)
