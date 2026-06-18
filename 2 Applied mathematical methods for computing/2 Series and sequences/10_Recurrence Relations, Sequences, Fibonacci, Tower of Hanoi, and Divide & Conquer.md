# Recurrence Relations, Sequences, Fibonacci, Tower of Hanoi, and Divide & Conquer

---

# 1. Recurrence Relation

## Definition

A **Recurrence Relation** is an equation that defines a sequence by using previous terms of the same sequence.

In simple words:

> A recurrence relation tells us how to find the next term using earlier terms.

---

## General Idea

Instead of directly giving:

a₁, a₂, a₃, ...

we give a rule such as:

aₙ = aₙ₋₁ + 2

or

aₙ = 2aₙ₋₁

and compute terms one by one.

---

## Example 1

Given:

a₁ = 1

aₙ = aₙ₋₁ + 2

Find first few terms.

a₁ = 1

a₂ = 1 + 2 = 3

a₃ = 3 + 2 = 5

a₄ = 5 + 2 = 7

Sequence:

1, 3, 5, 7, ...

---

## Example 2

Given:

a₁ = 2

aₙ = 2aₙ₋₁

a₂ = 4

a₃ = 8

a₄ = 16

a₅ = 32

Sequence:

2, 4, 8, 16, 32

---

## Example 3

Fibonacci:

a₁ = 1

a₂ = 1

aₙ = aₙ₋₁ + aₙ₋₂

Sequence:

1, 1, 2, 3, 5, 8, 13, ...

---

## Real-Life Example

Bank account:

Initial money:

₹1000

Every month:

Add ₹500

Recurrence:

aₙ = aₙ₋₁ + 500

---

# 2. Infinite Sequence

## Definition

An **Infinite Sequence** is a sequence that continues forever.

Mathematically:

A function from positive integers to real numbers.

---

## Simple Meaning

Each position has exactly one value:

1st term

2nd term

3rd term

...

and the list never ends.

---

## Example 1

Natural numbers:

1, 2, 3, 4, 5, ...

continues forever.

---

## Example 2

Even numbers:

2, 4, 6, 8, 10, ...

continues forever.

---

## Example 3

Powers of 2:

1, 2, 4, 8, 16, 32, ...

continues forever.

---

## Function View

Sequence:

1, 4, 9, 16, ...

can be written as:

aₙ = n²

---

# 3. Tower of Hanoi Problem

## Definition

The **Tower of Hanoi** is a famous puzzle involving:

- Three rods (spikes)
- Multiple disks of different sizes

Goal:

Move all disks from one rod to another.

---

## Rules

1. Move one disk at a time.
2. Larger disk cannot sit on smaller disk.
3. Use the third rod as helper.

---

## Example: 1 Disk

Move:

1 step

Answer:

a₁ = 1

---

## Example: 2 Disks

Move small disk

Move large disk

Move small disk

Answer:

a₂ = 3

---

## Example: 3 Disks

Total moves:

7

Answer:

a₃ = 7

---

## Pattern

| Disks | Moves |
|---------|---------|
| 1 | 1 |
| 2 | 3 |
| 3 | 7 |
| 4 | 15 |
| 5 | 31 |

---

## Recurrence Relation

aₙ = 2aₙ₋₁ + 1

---

### Example

For n=4:

a₄ = 2(7)+1

= 15

---

## Closed Formula

aₙ = 2ⁿ − 1

---

## Why Important?

Tower of Hanoi is one of the most famous recursion examples in computer science.

---

# 4. Linear Recurrence

## Definition

A **Linear Recurrence** is a recurrence relation where terms are combined using addition and multiplication by constants.

---

## General Form

aₙ

= c₁aₙ₋₁ + c₂aₙ₋₂ + ...

---

## Example 1

aₙ = aₙ₋₁ + 5

Linear.

---

## Example 2

aₙ = 2aₙ₋₁

Linear.

---

## Example 3

Fibonacci:

aₙ = aₙ₋₁ + aₙ₋₂

Linear.

---

## Not Linear Example

aₙ = (aₙ₋₁)²

Not linear.

Because squaring appears.

---

# 5. Linear Non-Homogeneous Recurrence

## Definition

A linear recurrence containing an extra term depending only on n.

---

## General Form

aₙ

= c₁aₙ₋₁ + c₂aₙ₋₂ + ...

+ f(n)

---

## Example 1

aₙ = aₙ₋₁ + 3

Extra term:

f(n)=3

---

### Terms

1,4,7,10,13,...

---

## Example 2

aₙ = 2aₙ₋₁ + 1

Tower of Hanoi.

Extra term:

f(n)=1

---

## Example 3

aₙ = aₙ₋₁ + n

Extra term depends on n.

---

### Terms

1

3

6

10

15

---

## Real-Life Example

Population:

Current population

+

new births

The births act like:

f(n)

---

# 6. First-Order Recurrence

## Definition

A recurrence where each term depends on only ONE previous term.

---

## General Form

aₙ = f(aₙ₋₁)

---

## Example 1

aₙ = aₙ₋₁ + 2

---

Sequence

1

3

5

7

9

---

## Example 2

aₙ = 2aₙ₋₁

---

Sequence

1

2

4

8

16

---

## Example 3

Population Growth

Start:

1000

Growth:

+100 every year

Recurrence:

Pₙ = Pₙ₋₁ + 100

---

# 7. Second-Order Recurrence

## Definition

A recurrence where each term depends on TWO previous terms.

---

## General Form

aₙ

= f(aₙ₋₁,aₙ₋₂)

---

## Example 1

Fibonacci

aₙ

= aₙ₋₁ + aₙ₋₂

---

## Example 2

aₙ

= 2aₙ₋₁ + aₙ₋₂

---

### Terms

1

1

3

7

17

41

---

## Example 3

Rabbit population models often use second-order recurrences.

Current rabbits depend on:

- Previous generation
- Generation before that

---

# 8. Fibonacci Sequence

## Definition

The Fibonacci sequence is one of the most famous sequences in mathematics.

---

## Recurrence Relation

aₙ

= aₙ₋₁ + aₙ₋₂

---

## Initial Values

a₁ = 1

a₂ = 1

---

## Sequence

1

1

2

3

5

8

13

21

34

55

---

## Example

Find:

a₆

a₆

= a₅ + a₄

= 5 + 3

= 8

---

## Real-Life Examples

Appears in:

- Plant growth
- Pinecones
- Sunflowers
- Computer algorithms

---

# 9. Arithmetic Sequence

## Definition

A sequence where consecutive terms differ by the same constant value.

---

## Formula

aₙ

= aₙ₋₁ + c

---

## Example 1

1,3,5,7,9

Difference:

2

---

## Example 2

10,20,30,40

Difference:

10

---

## Example 3

100,95,90,85

Difference:

-5

---

## Real-Life Example

Savings:

₹100

₹200

₹300

₹400

Increase always:

₹100

---

# 10. Geometric Sequence

## Definition

A sequence where consecutive terms have the same ratio.

---

## Formula

aₙ

= r·aₙ₋₁

---

## Example 1

2,4,8,16,32

Ratio:

2

---

## Example 2

3,9,27,81

Ratio:

3

---

## Example 3

100,50,25,12.5

Ratio:

1/2

---

## Real-Life Example

Bacteria doubling every hour:

1

2

4

8

16

32

---

# Arithmetic vs Geometric

| Arithmetic | Geometric |
|------------|------------|
| Add constant | Multiply constant |
| 2,4,6,8 | 2,4,8,16 |
| Difference fixed | Ratio fixed |
| Linear growth | Exponential growth |

---

# 11. Divide and Conquer Algorithm

## Definition

A **Divide and Conquer Algorithm** solves a problem by:

1. Divide
2. Solve
3. Combine

---

## General Strategy

Large Problem

↓

Smaller Problems

↓

Solve Recursively

↓

Combine Answers

---

## Example 1: Merge Sort

Sort:

8,3,6,1

---

### Divide

8,3

6,1

---

### Divide Again

8

3

6

1

---

### Solve

3,8

1,6

---

### Combine

1,3,6,8

---

## Example 2: Binary Search

Find:

50

inside sorted list.

---

Instead of checking every element:

Check middle.

Discard half.

Repeat.

---

## Example 3: Finding Maximum

Split array into halves.

Find maximum in each half.

Compare.

Return larger value.

---

## Why Divide and Conquer Works

Large problems become easier when reduced into smaller versions of themselves.

This is closely connected to:

- Recursion
- Recurrence relations
- Algorithm analysis

---

# Relationship Among Concepts

Recursion
      ↓
Recurrence Relation
      ↓
Sequences
      ↓
Fibonacci
      ↓
Algorithm Analysis
      ↓
Divide & Conquer

---

# Quick Summary Table

| Concept | Simple Meaning |
|----------|---------------|
| Recurrence Relation | Rule using previous terms to generate next terms |
| Infinite Sequence | Sequence that never ends |
| Tower of Hanoi | Recursive puzzle with recurrence aₙ=2aₙ₋₁+1 |
| Linear Recurrence | Recurrence using linear combinations of previous terms |
| Non-Homogeneous Recurrence | Linear recurrence with extra term f(n) |
| First-Order Recurrence | Depends on one previous term |
| Second-Order Recurrence | Depends on two previous terms |
| Fibonacci Sequence | Each term = sum of previous two terms |
| Arithmetic Sequence | Constant difference |
| Geometric Sequence | Constant ratio |
| Divide and Conquer | Divide, solve recursively, combine |

---

# Final Mental Model

Sequence
      ↓
Recurrence Relation
      ↓
Previous Terms Generate Next Terms

Examples:

Arithmetic:
1,3,5,7,...

Geometric:
2,4,8,16,...

Fibonacci:
1,1,2,3,5,8,...

Tower of Hanoi:
1,3,7,15,31,...

Algorithms:

Large Problem
      ↓
Break Into Smaller Problems
      ↓
Solve Recursively
      ↓
Combine Results
      ↓
Final Solution

This connection between recursion, recurrence relations, sequences, and divide-and-conquer algorithms forms one of the most important foundations of discrete mathematics and algorithm analysis.