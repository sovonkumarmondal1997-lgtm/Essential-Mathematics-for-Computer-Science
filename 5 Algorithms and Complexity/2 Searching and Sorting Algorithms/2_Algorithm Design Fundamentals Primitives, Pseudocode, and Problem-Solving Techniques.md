# Algorithm Design Fundamentals: Primitives, Pseudocode, and Problem-Solving Techniques

These beginner-friendly notes explain the basic building blocks used to
design algorithms before writing code.

------------------------------------------------------------------------

# 1. Primitives

## Definition

**Primitives** are the basic building blocks used to write algorithms.

Think of them as the "basic instructions" that every algorithm is built
from.

Examples include:

-   Assigning values
-   Making decisions
-   Repeating steps
-   Calling functions

------------------------------------------------------------------------

## Real-Life Analogy

Building a house uses basic materials:

-   Bricks
-   Cement
-   Steel
-   Wood

Similarly, algorithms use primitives as their building blocks.

------------------------------------------------------------------------

## Example

Making tea:

1.  Boil water
2.  Add tea leaves
3.  Stir
4.  Pour into a cup

Each step is a primitive action.

------------------------------------------------------------------------

# 2. Pseudocode

## Definition

**Pseudocode** is an informal way of writing an algorithm using simple
English mixed with programming-like statements.

It is designed for humans, not computers.

------------------------------------------------------------------------

## Example 1

Problem: Add two numbers

Pseudocode

    START

    Read A

    Read B

    SUM = A + B

    Print SUM

    STOP

------------------------------------------------------------------------

## Example 2

Find the largest number

    IF A > B

        Print A

    ELSE

        Print B

    END IF

------------------------------------------------------------------------

## Why Use Pseudocode?

-   Easy to understand
-   Independent of programming language
-   Helps design algorithms before coding

------------------------------------------------------------------------

# 3. Value Assignment Primitive

## Definition

A **value assignment** stores a value inside a variable.

Usually represented by

    =

------------------------------------------------------------------------

## Example 1

    Age = 20

Variable

    Age

stores

    20

------------------------------------------------------------------------

## Example 2

    Sum = A + B

The result of the addition is stored in `Sum`.

------------------------------------------------------------------------

## Real-Life Analogy

Writing money into your bank account.

Your account stores the value.

------------------------------------------------------------------------

# 4. Conditional Primitive (If-Else)

## Definition

A conditional checks whether a condition is true.

If true, one block runs.

Otherwise, another block runs.

------------------------------------------------------------------------

## Example 1

    IF Age >= 18

        Print "Adult"

    ELSE

        Print "Minor"

    END IF

------------------------------------------------------------------------

## Example 2

Check whether a number is even.

    IF Number MOD 2 == 0

        Print "Even"

    ELSE

        Print "Odd"

    END IF

------------------------------------------------------------------------

## Everyday Analogy

Traffic light:

If green → Drive.

Else → Stop.

------------------------------------------------------------------------

# 5. Loop Primitive (While Loop)

## Definition

A **while loop** repeats instructions as long as a condition remains
true.

------------------------------------------------------------------------

## Example 1

Print numbers from 1 to 5.

    i = 1

    WHILE i <= 5

        Print i

        i = i + 1

    END WHILE

------------------------------------------------------------------------

## Example 2

Countdown

    Count = 5

    WHILE Count > 0

        Print Count

        Count = Count - 1

    END WHILE

------------------------------------------------------------------------

## Real-Life Analogy

Keep climbing stairs while there are stairs left.

------------------------------------------------------------------------

# 6. Function Primitive

## Definition

A **function** is a reusable block of instructions that performs a
specific task.

Instead of writing the same steps repeatedly, we call the function.

------------------------------------------------------------------------

## Example 1

    FUNCTION Add(A,B)

    RETURN A+B

Usage

    Answer = Add(5,10)

------------------------------------------------------------------------

## Example 2

Square a number

    FUNCTION Square(x)

    RETURN x*x

------------------------------------------------------------------------

## Everyday Analogy

Using a washing machine.

Press the same button whenever you need to wash clothes.

------------------------------------------------------------------------

# 7. Divide and Conquer

## Definition

Divide a large problem into smaller problems.

Solve each smaller problem.

Combine the answers.

------------------------------------------------------------------------

## Example 1

Searching a phone book.

Instead of checking every page,

split the book into halves repeatedly.

This is how Binary Search works.

------------------------------------------------------------------------

## Example 2

Merge Sort

Split:

    8 3 5 1

↓

    8 3

    5 1

↓

Sort each part.

↓

Merge them.

Result

    1 3 5 8

------------------------------------------------------------------------

## Real-Life Analogy

Cleaning a large house one room at a time.

------------------------------------------------------------------------

# 8. Greedy Algorithm

## Definition

A greedy algorithm chooses what looks best **right now** without
considering all future possibilities.

------------------------------------------------------------------------

## Example 1

Coin change.

Need

    37

Coins

    25

    10

    1

Greedy chooses

    25

    10

    1

    1

------------------------------------------------------------------------

## Example 2

Scheduling meetings.

Always choose the meeting that finishes earliest.

This leaves maximum time for later meetings.

------------------------------------------------------------------------

## Everyday Analogy

Always taking the shortest visible road.

It often works,

but not always.

------------------------------------------------------------------------

# 9. Backtracking

## Definition

Backtracking tries one solution.

If it fails,

it goes back and tries another.

------------------------------------------------------------------------

## Example 1

Maze

    Start

    ↓

    Wrong path

    ↓

    Back

    ↓

    Try another path

    ↓

    Exit

------------------------------------------------------------------------

## Example 2

Sudoku

Fill one number.

If later it becomes impossible,

erase it and try another number.

------------------------------------------------------------------------

## Example 3

N-Queens

Place a queen.

If queens attack each other,

remove one queen and try another position.

------------------------------------------------------------------------

## Everyday Analogy

Trying keys to open a lock.

Wrong key?

Try another.

------------------------------------------------------------------------

# Complete Example

Problem

Print all even numbers from 2 to 10.

Pseudocode

    START

    Number = 2

    WHILE Number <= 10

        Print Number

        Number = Number + 2

    END WHILE

    STOP

Primitives used

-   Assignment
-   While Loop
-   Output

------------------------------------------------------------------------

# Quick Summary

  Concept              Simple Meaning
  -------------------- --------------------------------------
  Primitives           Basic building blocks of algorithms
  Pseudocode           Human-readable algorithm description
  Value Assignment     Store a value in a variable
  If-Else              Make decisions
  While Loop           Repeat while a condition is true
  Function             Reusable block of instructions
  Divide and Conquer   Split, solve, combine
  Greedy Algorithm     Choose the best immediate option
  Backtracking         Try, fail, go back, try again
