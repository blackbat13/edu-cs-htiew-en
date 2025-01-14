# Robot

PYou settle a robot, capable of moving only along the *x* axis, with the ability to move left or right. The robot starts its route from the position marked $0$. It can execute the following instructions::

* LEFT - move one unit to the left,
* RIGHT - move one unit to the right,
* AS IN $i$ - make the same move as in the $i$-th instruction. The $i$ is always a natural number and does not exceed the number of the instruction in which it appears. We count the instructions from one.

You wonder if the robot is working properly. Your task is to write a program that, for a given set of instructions, determines the position at which the robot will eventually be placed.

Source: [https://onlinejudge.org/external/125/12503.pdf](https://onlinejudge.org/external/125/12503.pdf)

## Specification

### Input

* $n$ - natural number, number of instructions to be executed, $1\leq p\leq 100$.
* $n$ lines containing one of the instructions as described earlier.

### Output

* An integer indicating the position of the robot after all instructions have been executed.

## Example 1

### Input

```
3
LEFT
RIGHT
AS IN 2
```

**Output:** $1$

## Example 2

### Input

```
5
LEFT
AS IN 1
AS IN 2
AS IN 1
AS IN 4
```

**Output:** $-5$
