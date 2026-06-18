# Recursion, Recursive Definitions, and Recursive Algorithms

---

# 1. Recursion

## Definition

**Recursion** is the process of defining something in terms of itself.

In simple words:

> A problem is solved by using a smaller version of the same problem.

---

## Everyday Example

Imagine standing between two mirrors.

Each mirror reflects the other mirror.

You see:

Mirror
→ Mirror inside mirror
→ Mirror inside mirror
→ Mirror inside mirror

This repeating self-reference is similar to recursion.

---

## Example 1: Counting Down

Suppose we want to count down from 5.

5
4
3
2
1
0

We can think of it as:

CountDown(5)

=
5 + CountDown(4)

=
5 + 4 + CountDown(3)

and so on.

---

## Example 2: Russian Nesting Dolls

A large doll contains a smaller doll.

That doll contains another doll.

That doll contains another doll.

The same structure repeats.

This is recursion.

---

## Example 3: Folder Inside Folder

Computer folders can contain folders.

Folder A

contains Folder B

contains Folder C

contains Folder D

Each folder is similar to the previous one.

This recursive structure is common in computer science.

---

## Why Recursion Is Useful

Many complex problems become easier when broken into smaller copies of themselves.

Examples:

- Factorial
- Fibonacci numbers
- Tree structures
- Directory traversal
- Divide and conquer algorithms

---

# 2. Recursively Defined Function / Inductive Definition

## Definition

A **Recursively Defined Function** is a function whose values are defined using smaller values of the same function.

It contains:

1. Basis Step
2. Recursive Step

---

## General Structure

Basis Step:

Give initial value.

Recursive Step:

Use previous values to calculate new values.

---

## Example 1: Factorial

Basis:

0! = 1

Recursive:

n! = n × (n−1)!

---

### Calculation

3!

= 3 × 2!

= 3 × 2 × 1!

= 3 × 2 × 1 × 0!

= 3 × 2 × 1 × 1

= 6

---

## Example 2: Powers of 2

Basis:

a₀ = 1

Recursive:

aₙ = 2aₙ₋₁

---

Values:

a₁ = 2

a₂ = 4

a₃ = 8

a₄ = 16

---

## Example 3: Fibonacci Numbers

Basis:

F₀ = 0

F₁ = 1

Recursive:

Fₙ = Fₙ₋₁ + Fₙ₋₂

---

Values:

0

1

1

2

3

5

8

13

---

# 3. Basis Step (Functions)

## Definition

The **Basis Step** is the starting value of a recursive function.

Without it:

The recursion never ends.

---

## Why Important?

It gives recursion a stopping point.

---

## Example 1

Factorial

0! = 1

This is the basis step.

---

## Example 2

Fibonacci

F₀ = 0

F₁ = 1

These are basis steps.

---

## Example 3

Power Sequence

a₀ = 1

Basis step.

---

## Staircase Analogy

The basis step is the first stair.

Without the first stair,

the staircase cannot begin.

---

# 4. Recursive Step (Functions)

## Definition

The **Recursive Step** tells us how to compute larger values from smaller values.

---

## General Form

Current value

↓

Previous value(s)

↓

Rule

---

## Example 1

Factorial

n! = n × (n−1)!

---

### Compute 4!

4!

= 4 × 3!

= 4 × 3 × 2!

= 4 × 3 × 2 × 1!

= 24

---

## Example 2

Powers of 2

aₙ = 2aₙ₋₁

---

a₀ = 1

a₁ = 2

a₂ = 4

a₃ = 8

---

## Example 3

Fibonacci

Fₙ = Fₙ₋₁ + Fₙ₋₂

---

F₅

= F₄ + F₃

= 3 + 2

= 5

---

# 5. Recursively Defined Set

## Definition

A **Recursively Defined Set** is a set built by:

1. Specifying starting elements.
2. Giving rules for generating new elements.

---

## Idea

Start with a few members.

Keep creating more members.

Eventually build the entire set.

---

## Example 1: Natural Numbers

Basis:

0 ∈ N

Recursive Step:

If n ∈ N

then n+1 ∈ N

---

Generation

0

1

2

3

4

5

...

---

## Example 2: Even Numbers

Basis:

0 ∈ E

Recursive Step:

If n ∈ E

then n+2 ∈ E

---

Generation

0

2

4

6

8

10

...

---

## Example 3: Multiples of 3

Basis:

0 ∈ M

Recursive Step:

If n ∈ M

then n+3 ∈ M

---

Generation

0

3

6

9

12

15

...

---

# 6. Basis Step (Sets)

## Definition

The **Basis Step** identifies the first members of the set.

---

## Example 1

Natural Numbers

0 ∈ N

---

## Example 2

Even Numbers

0 ∈ E

---

## Example 3

Positive Integers

1 ∈ P

---

## Why Important?

Without initial elements,

the set cannot generate anything.

---

## Tree Analogy

Basis step = root node

Everything else grows from it.

---

# 7. Recursive Step (Sets)

## Definition

The **Recursive Step** explains how new elements are produced from existing elements.

---

## Example 1

Natural Numbers

If n ∈ N

then n+1 ∈ N

---

## Example 2

Even Numbers

If n ∈ E

then n+2 ∈ E

---

## Example 3

Multiples of 5

If n ∈ M

then n+5 ∈ M

---

## Factory Analogy

Basis Step:

First product.

Recursive Step:

Machine creates more products.

---

# 8. Algorithm

## Definition

An **Algorithm** is a finite sequence of precise instructions used to solve a problem.

---

## Simple Formula

Input

↓

Steps

↓

Output

---

## Example 1

Making Tea

1. Boil water
2. Add tea leaves
3. Add sugar
4. Pour into cup

This is an algorithm.

---

## Example 2

Finding Maximum Number

Input:

5, 2, 9, 1

Steps:

Compare numbers.

Output:

9

---

## Example 3

Addition

Input:

3 and 4

Step:

3+4

Output:

7

---

## Characteristics

An algorithm must be:

- Finite
- Precise
- Unambiguous
- Effective

---

# 9. Recursive Algorithm

## Definition

A **Recursive Algorithm** solves a problem by calling itself on smaller versions of the same problem.

---

## Pattern

Problem

↓

Smaller Problem

↓

Even Smaller Problem

↓

Base Case

---

## Example 1: Factorial

factorial(4)

↓

4 × factorial(3)

↓

4 × 3 × factorial(2)

↓

4 × 3 × 2 × factorial(1)

↓

4 × 3 × 2 × 1

↓

24

---

## Example 2: Countdown

countdown(3)

prints:

3

countdown(2)

prints:

2

countdown(1)

prints:

1

countdown(0)

stops

---

## Example 3: Fibonacci

fib(5)

requires:

fib(4)

and

fib(3)

which require smaller Fibonacci computations.

---

# 10. Factorial (n!)

## Definition

Factorial means:

Multiply all positive integers from 1 to n.

---

## Formula

n!

= n × (n−1) × (n−2) × ... × 2 × 1

---

## Examples

### Example 1

1!

= 1

---

### Example 2

3!

= 3×2×1

= 6

---

### Example 3

5!

= 5×4×3×2×1

= 120

---

### Example 4

6!

= 720

---

## Recursive Definition

Basis:

0! = 1

Recursive:

n! = n(n−1)!

---

## Recursive Expansion Example

5!

= 5×4!

= 5×4×3!

= 5×4×3×2!

= 5×4×3×2×1!

= 120

---

# 11. Pseudocode

## Definition

**Pseudocode** is an informal way of writing algorithms.

It looks like code,

but is written in plain language.

---

## Purpose

Focus on logic

without worrying about programming syntax.

---

## Example 1: Find Maximum

Pseudocode:

START

largest ← first number

FOR each remaining number

    IF number > largest

        largest ← number

PRINT largest

END

---

## Example 2: Factorial

Pseudocode:

FUNCTION Factorial(n)

    IF n = 0

        RETURN 1

    ELSE

        RETURN n × Factorial(n−1)

END FUNCTION

---

## Example 3: Countdown

Pseudocode:

FUNCTION Countdown(n)

    IF n = 0

        STOP

    PRINT n

    Countdown(n−1)

END FUNCTION

---

## Why Pseudocode Is Useful

It helps programmers:

- Design algorithms
- Communicate ideas
- Plan solutions
- Understand recursion

before writing actual code.

---

# Quick Summary Table

| Concept | Simple Meaning |
|----------|---------------|
| Recursion | Defining something using itself |
| Recursive Function | Function defined using smaller values of itself |
| Basis Step (Function) | Starting value of recursion |
| Recursive Step (Function) | Rule generating later values |
| Recursively Defined Set | Set built from initial elements and rules |
| Basis Step (Set) | Initial members of the set |
| Recursive Step (Set) | Rule generating new members |
| Algorithm | Step-by-step problem-solving procedure |
| Recursive Algorithm | Algorithm calling itself |
| Factorial | Product of all positive integers up to n |
| Pseudocode | Human-readable algorithm description |

---

# Final Mental Model

Recursion

Basis Step
      ↓
Recursive Step
      ↓
Smaller Problem
      ↓
Smaller Problem
      ↓
Smaller Problem
      ↓
Base Case Reached
      ↓
Answer Built Back Up

Example:

5!
      ↓
5 × 4!
      ↓
5 × 4 × 3!
      ↓
5 × 4 × 3 × 2!
      ↓
5 × 4 × 3 × 2 × 1!
      ↓
120

Recursion is simply:

"Solve a big problem by solving a smaller version of the same problem."