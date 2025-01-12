# Linear algorithms

What is an algorithm? An instruction, a recipe, a procedure scheme... An algorithm describes the solution to a certain problem. There are many types of algorithms, and we will start with the simplest of them - linear algorithms.

## Linear algorithm

A linear algorithm is a sequential instruction whose steps are executed one by one, line by line, operation by operation.

When constructing an algorithm, a number of questions arise. How detailed should the algorithm be? What operations must we include in it, and which ones can we omit? What operations are available? In what form should we present our algorithm? These are just some of the important issues to consider.

Consider the following example.

### Example 1

Imagine that we have to prepare a jam sandwich. This is our problem. For this problem, we will propose an example solution in the form of **algorithm**.

```
1. Take a slice of bread
2. Take butter
3. Take the jam
4. Take a knife
5. Spread butter on the bread
6. Spread the bread with jam
```

As you can see, the above example is an algorithm for preparing a jam sandwich. However, let's consider its correctness and accuracy. Have all the necessary operations been included? Or can any of them be omitted? Should we add instructions for unscrewing the jar? How about opening the refrigerator to take out the jam and then closing it? What if there is no jam and you have to go to the store? What if it's Sunday and the stores are closed? What if...

We can continue such considerations indefinitely, but we need to set some limits.

## Problem specification

First of all, we start with **specification**. Specification defines what input the algorithm takes and what the result should be. In other words, it is a formal definition of the problem. Let's go back to our example.

### Example 2

Let's start by formalizing our problem of preparing a jam sandwich with specifications.

#### Specification

**Input**:

* A slice of bread.
* Butter.
* Jam.

**Output**:

* Jam sandwich

Now we can move on to the algorithm. As you can see, we have three inputs: a slice of bread, butter and jam. So we don't have to worry about preparing these ingredients. Usually, in the writing of the algorithm, we skip the stage of loading the data, which means that in this case we leave out the instructions describing the taking of the bread, butter and jam. We simply assume, according to the specification, that these items are already given to us and available to our algorithm.

#### Algorithm

```
1. Take a knife
2. Spread butter on the bread
3. Spread the bread with jam
```

In this case, we have limited ourselves to a certain set of operations and to a certain level of detail. When we move on to more technical algorithms, it will become clear which operations we can perform and which we cannot.
