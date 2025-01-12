# Functions

Imagine a black magic box. The kind of box into which we put something and something else falls out of it. We put **input** into it, and **output** comes out:

![](<../../assets/image (32).png>)

In other words, we put some **input** in the box, and take out **output**:

![](<../../assets/image (33).png>)

Such a box represents to us just **function**.

## What is a function?

In programming, we can understand the concept of a function in many ways. The easiest way is to think of it as a certain **fragment** of a program, which has a specific task and its own name. We pass data to the function in the form of **parameters**, and in response we get a result according to the **specification** of the function.

!!! danger
	 Do not confuse functions in programming and functions in mathematics, they are two completely different creations!

The schematic notation of the function is as follows:

```
function FunctionName(parameter1, parameter2, ...):
    Operation1
    Operation2
    ...
    Return result
```

## Example - coffee vending machine

Let's imagine a coffee vending machine, the kind that stands in the corridors of many offices, schools and train stations. We can say that it represents a certain function, according to the following specification:

### Specification

#### Input

* **choice** - selected beverage
* **money** - amount due

#### Output

* Selected beverage.

!!! info
	 Of course, this is a very simplified Specification. In reality, such a vending machine will not give us a drink unless we pay the appropriate fee. Sometimes we will get change in addition to the drink. However, such Specification will suffice for us for an example.

Let's try to write a fragment of the function carried out by such an automaton in the form of pseudocode:

```
function CoffeeVendingMachine(choice, money):
    1. If choice = "latte" and money = 3.0, then:
        2. Return Latte and stop   
```

## Procedure

Unlike a function, the procedure **does not return a specific result**. So what could be its purpose? We can use a procedure, for example, to change the values of variables passed as parameters (if we pass them appropriately), to change the values of global variables, or to print a message on the screen. We can easily imagine a greeting procedure that takes the user's name and displays the appropriate message on the screen:

```
procedure Welcome(name):
    1. Print "Hello "
    2. Print name
    3. Print "!"
    4. Print newline character
    5. Stop
```

!!! warning
	 Nowadays we practically no longer distinguish between a function and a procedure. In many programming languages there are only functions, including those that do not return a result (or whose result we ignore).

## Presentation

[:fontawesome-solid-file-pdf: Funkcje - wprowadzenie](../../assets/Funkcje - wprowadzenie.pdf)
