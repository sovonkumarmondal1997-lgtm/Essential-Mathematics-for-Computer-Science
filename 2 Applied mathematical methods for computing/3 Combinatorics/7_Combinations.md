# Combinations - Complete Beginner's Guide

# Table of Contents

1. Introduction to Combinations
2. Combination
3. r-Combination
4. Combination Formula C(n,r)
5. Factorial Expansion and Simplification
6. Symmetry of Combinations
7. Case-Based Counting (The Sum Rule)
8. Permutations vs Combinations
9. Quick Summary Sheet

---

# Introduction to Combinations

One of the most important topics in combinatorics is:

```text
Combination
```

A combination focuses on:

```text
Selecting objects
```

without caring about their order.

The most important idea is:

> Order Does Not Matter

---

# Combination

## Simple Definition

A **Combination** is an unordered selection of objects.

If the same objects are selected, changing their positions does not create a new combination.

---

# Easy Way to Remember

```text
Combination = Selection
```

```text
Order Does NOT Matter
```

---

# Example 1: Choosing a Team

Students:

```text
Alice
Bob
Charlie
```

Choose:

```text
2 students
```

Possible selections:

```text
{Alice, Bob}
{Alice, Charlie}
{Bob, Charlie}
```

Notice:

```text
{Alice, Bob}
```

and

```text
{Bob, Alice}
```

are the same team.

---

# Example 2: Pizza Toppings

Available toppings:

```text
Cheese
Onion
Mushroom
```

Choose:

```text
2 toppings
```

Selection:

```text
Cheese + Onion
```

is identical to:

```text
Onion + Cheese
```

---

# Example 3: Forming a Committee

People:

```text
A B C D
```

Committee:

```text
A C
```

Same as:

```text
C A
```

No difference.

---

# Example 4: Lottery Numbers

Lottery ticket:

```text
5 12 18 25 41
```

Same ticket as:

```text
41 25 18 12 5
```

Order does not matter.

---

# Key Difference

## Permutation

```text
ABC ≠ BAC
```

---

## Combination

```text
ABC = BAC
```

---

# r-Combination

## Simple Definition

An r-combination means:

```text
Choose r objects
```

from:

```text
n objects
```

without caring about order.

---

# Easy Way to Remember

```text
Choose
NOT
Arrange
```

---

# Example 1

Objects:

```text
A B C D
```

Choose:

```text
2
```

Possible combinations:

```text
AB
AC
AD
BC
BD
CD
```

Total:

```text
6
```

Notice:

```text
AB
```

and

```text
BA
```

count only once.

---

# Example 2

Students:

```text
10 students
```

Choose:

```text
3 representatives
```

Order doesn't matter.

This is an r-combination.

---

# Example 3

Books:

```text
8 books
```

Choose:

```text
4 books to borrow
```

The order of selection is irrelevant.

---

# Example 4

Card Deck

Choose:

```text
5 cards
```

from:

```text
52 cards
```

Order does not matter.

---

# Combination Formula C(n,r)

## Formula

\[
C(n,r)
=
\frac{n!}{r!(n-r)!}
\]

---

## Alternative Notations

\[
\binom{n}{r}
\]

or

\[
{}_nC_r
\]

Both mean:

```text
Choose r objects from n objects
```

---

# Why Does This Formula Work?

Start with permutations:

\[
P(n,r)
=
\frac{n!}{(n-r)!}
\]

---

But combinations ignore order.

Each group of r objects can be arranged in:

\[
r!
\]

different ways.

Therefore divide by:

\[
r!
\]

giving:

\[
C(n,r)
=
\frac{n!}{r!(n-r)!}
\]

---

# Example 1

Choose:

```text
2 from 4
```

\[
C(4,2)
=
\frac{4!}{2!2!}
\]

\[
=
\frac{24}{4}
\]

\[
=6
\]

---

# Example 2

Choose:

```text
3 from 5
```

\[
C(5,3)
=
\frac{5!}{3!2!}
\]

\[
=
\frac{120}{12}
\]

\[
=10
\]

---

# Example 3

Choose:

```text
4 from 7
```

\[
C(7,4)
=
35
\]

---

# Example 4

Choose:

```text
5 from 10
```

\[
C(10,5)
=
252
\]

---

# Factorial Expansion and Simplification

## Simple Definition

Factorial expressions often look large.

Instead of calculating huge factorials directly, we expand them and cancel common terms.

This makes calculations much easier.

---

# Example 1

\[
C(8,3)
=
\frac{8!}{3!5!}
\]

Expand:

\[
=
\frac{8\times7\times6\times5!}
{3\times2\times1\times5!}
\]

Cancel:

\[
5!
\]

Result:

\[
=
\frac{8\times7\times6}
{3\times2\times1}
\]

\[
=
56
\]

---

# Example 2

\[
C(10,2)
=
\frac{10!}{2!8!}
\]

Expand:

\[
=
\frac{10\times9\times8!}
{2\times1\times8!}
\]

Cancel:

\[
8!
\]

Result:

\[
=
\frac{10\times9}{2}
\]

\[
=45
\]

---

# Example 3

\[
C(12,4)
=
\frac{12!}{4!8!}
\]

Expand:

\[
=
\frac{12\times11\times10\times9\times8!}
{4\times3\times2\times1\times8!}
\]

Cancel:

\[
8!
\]

Result:

\[
=
495
\]

---

# Why Simplify?

Without simplification:

```text
12!
=
479,001,600
```

Large numbers become difficult.

Cancellation keeps calculations manageable.

---

# Symmetry of Combinations

## Property

\[
C(n,r)
=
C(n,n-r)
\]

---

# Simple Meaning

Choosing:

```text
r objects
```

is equivalent to leaving behind:

```text
n-r objects
```

---

# Example 1

Suppose:

```text
10 students
```

Choose:

```text
3 students
```

or

Leave behind:

```text
7 students
```

Both count the same selection.

Therefore:

\[
C(10,3)
=
C(10,7)
\]

\[
=120
\]

---

# Example 2

\[
C(8,2)
=
C(8,6)
\]

Both equal:

\[
28
\]

---

# Example 3

\[
C(12,1)
=
C(12,11)
\]

Both equal:

\[
12
\]

---

# Example 4

\[
C(15,4)
=
C(15,11)
\]

Both equal:

\[
1365
\]

---

# Visual Understanding

Choose:

```text
3 people
```

from:

```text
10 people
```

is exactly the same as deciding:

```text
which 7 people stay out.
```

---

# Why Symmetry Helps

Sometimes:

\[
C(100,97)
\]

looks difficult.

Use symmetry:

\[
C(100,97)
=
C(100,3)
\]

Much easier.

---

# Case-Based Counting
## (The Sum Rule)

---

# Simple Definition

Many problems contain phrases like:

```text
At most
```

or

```text
At least
```

In these situations:

1. Break the problem into separate cases.
2. Count each case.
3. Add the results.

---

# Formula

\[
\text{Total}
=
\text{Case 1}
+
\text{Case 2}
+
\text{Case 3}
+\cdots
\]

---

# Example 1: Committee of At Most 2 People

People:

```text
A B C D
```

Choose:

```text
At most 2 people
```

Cases:

### Choose 0

\[
C(4,0)=1
\]

### Choose 1

\[
C(4,1)=4
\]

### Choose 2

\[
C(4,2)=6
\]

Total:

\[
1+4+6
=
11
\]

---

# Example 2: At Least 3 Students

Students:

```text
5
```

Choose:

```text
At least 3
```

Cases:

### Exactly 3

\[
C(5,3)=10
\]

### Exactly 4

\[
C(5,4)=5
\]

### Exactly 5

\[
C(5,5)=1
\]

Total:

\[
10+5+1
=
16
\]

---

# Example 3: Password Length

Allowed lengths:

```text
4
5
6
```

Count:

### Length 4

Count separately.

### Length 5

Count separately.

### Length 6

Count separately.

Add all cases.

---

# Example 4: Choosing Fruits

Available:

```text
Apple
Banana
Orange
Grape
```

Choose:

```text
At most 3 fruits
```

Cases:

\[
C(4,0)
+
C(4,1)
+
C(4,2)
+
C(4,3)
\]

\[
1+4+6+4
=
15
\]

---

# When to Use Case-Based Counting

Look for phrases:

```text
At most
```

```text
At least
```

```text
No more than
```

```text
Between x and y
```

These often require multiple cases.

---

# Permutations vs Combinations

| Feature | Permutation | Combination |
|----------|------------|------------|
| Order Matters? | Yes | No |
| Purpose | Arrange | Select |
| Formula | P(n,r) | C(n,r) |
| ABC vs BAC | Different | Same |
| Example | Race rankings | Committee selection |

---

# Example Comparison

Choose:

```text
2 letters from A,B,C
```

---

## Permutations

```text
AB
BA
AC
CA
BC
CB
```

Total:

```text
6
```

---

## Combinations

```text
AB
AC
BC
```

Total:

```text
3
```

---

# Quick Summary Sheet

## Combination

Selection where:

```text
Order Does Not Matter
```

---

## r-Combination

Choose:

```text
r objects
```

from:

```text
n objects
```

---

## Combination Formula

\[
C(n,r)
=
\frac{n!}{r!(n-r)!}
\]

---

## Factorial Simplification

Expand factorials and cancel common terms.

Example:

\[
C(8,3)
=
\frac{8\times7\times6}
{3\times2\times1}
\]

---

## Symmetry Property

\[
C(n,r)
=
C(n,n-r)
\]

Choosing objects equals leaving objects behind.

---

## Case-Based Counting

Break problem into separate cases and add:

\[
\text{Case 1}
+
\text{Case 2}
+\cdots
\]

---

# Golden Rules

### Order Matters?

Use:

```text
Permutation
```

---

### Order Doesn't Matter?

Use:

```text
Combination
```

---

### Choosing r From n?

Use:

\[
C(n,r)
=
\frac{n!}{r!(n-r)!}
\]

---

### Large Combination?

Use:

```text
Factorial Cancellation
```

---

### See "At Most" or "At Least"?

Use:

```text
Case-Based Counting
```

and add the cases together.

---

### Fast Memory Trick

```text
Permutation = Arrange

Combination = Choose
```

This single idea solves most beginner counting problems correctly.