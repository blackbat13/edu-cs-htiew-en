# Variables

What is a variable? We can say that it is a kind of data box. We can perform all sorts of operations on variables: we can "insert" (**assign**) various values into them, perform operations on them, use them in calculations, and also read their values.

Variables are an indispensable part of virtually every algorithm. Therefore, their correct and in-depth understanding is required to be able to construct and implement advanced algorithms.

## Types of variables

Imagine two boxes: one plastic and one metal. In the plastic box we can only put fruit, and in the metal box we can only put nails. Each box has its own purpose. Its **type** of stored items.

The same is true of variables. Each variable can only store a certain type of value. We then say that a variable has its type. For example, we can create a variable to store integers. To such a variable we will no longer assign a value of another type, such as text.

!!! warning
	 In some programming languages we explicitly specify the type of a variable when we create it, in others we do not. Similarly, there are languages in which an attempt to assign a different type of value to a variable will end in an error. There are also those in which this type of operation will be allowed. However, this does not mean that we should do it! It is very important to respect the type of variables. This is important from the point of view of the readability of the program code, but also from the level of mechanics that lie underneath.

## Variable values

We already know that we can assign values to variables. But does this mean that once assigned a value to a variable, it remains unchanged? As you can guess from the name **variable,** this is not the case. It is very important to understand that we determine the value of a variable over time, that is, at a given point in the program's operation. To better understand this, let's look at the following examples.

### Example 1

```
1. a := 10
2. Print a
3. a := 2 * a
4. Print a
5. a := a + 5
6. Print a
```

Take a look at the pseudocode above. Can you tell what values will be output in instructions 2, 4 and 6? Try to answer this question before continuing.

The best way is to perform a **simulation** of the given pseudocode. Take a piece of paper and a pen and perform successive operations, writing down the values of the variables at each point. This can be done in many ways, one of which we present below.

```
1. [a = 10]
2. Print 10
3. [a = 2 * 10 = 20]
4. Print 20
5. [a = 20 + 5 = 25]
6. Print 25
```

As you can see, the algorithm presented earlier will enter the numbers sequentially: $10,\ 20,\ 25$.

### Example 2

```
1. a := 0
2. While a < 10, do:
    3. a := a + 2
    4. Print a
```

Again, before you go any further try to think about what further values the above algorithm will write out.

In this example, it is very important to correctly understand how the loop works. The loop repeats certain operations repeatedly, which means that we will execute the same instructions several times. Let's try to break it down.

```
1. [a = 0]

2. While 0 < 10 - OK
    3. [a = 0 + 2 = 2]
    4. Print 2
    
2. While 2 < 10 - OK
    3. [a = 2 + 2 = 4]
    4. Print 4
    
 2. While 4 < 10 - OK
     3. [a = 4 + 2 = 6]
     4. Print 6
     
 2. While 6 < 10 - OK
     3. [a = 6 + 2 = 8]
     4. Print 8
     
 2. While 8 < 10 - OK
     3. [a = 8 + 2 = 10]
     4. Print 10
     
 2. While 10 < 10 - NO (end of loop)
```

## Presentation

[:fontawesome-solid-file-pdf: Wprowadzenie](../../assets/Zmienne - wprowadzenie.pdf)

[:fontawesome-solid-file-pdf: Ćwiczenia](../../assets/Zmienne - ćwiczenia.pdf)

[:fontawesome-solid-file-pdf: Zmienne w pamięci](../../assets/Zmienne w Pamięci - Ćwiczenia.pdf)