# Permutations - Complete Beginner's Guide

# Table of Contents

1. Introduction to Permutations
2. Permutation
3. Factorial (n!)
4. r-Permutation
5. Permutation Formula P(n,r)
6. Block Permutation (String/Block Binding)
7. Permutation with Insertion (Gaps Method)
8. Quick Summary Sheet

---

# Introduction to Permutations

One of the most important topics in combinatorics is:

```text
Permutation
```

A permutation deals with:

```text
Arranging objects in order.
```

The most important idea is:

> Order Matters

---

# Permutation

## Simple Definition

A **Permutation** is an ordered arrangement of objects.

When the order changes, the arrangement changes.

---

## Easy Way to Remember

```text
Permutation = Position Matters
```

If two arrangements contain the same objects but in different positions, they are considered different permutations.

---

# Example 1: Three Students

Students:

```text
A
B
C
```

Possible arrangements:

```text
ABC
ACB
BAC
BCA
CAB
CBA
```

Total:

```text
6 arrangements
```

Notice:

```text
ABC ≠ BAC
```

because positions are different.

---

# Example 2: Gold, Silver, Bronze

Suppose:

```text
Alice
Bob
Charlie
```

compete in a race.

Arrangement:

```text
Alice
Bob
Charlie
```

means:

```text
Gold   = Alice
Silver = Bob
Bronze = Charlie
```

---

Arrangement:

```text
Bob
Alice
Charlie
```

means:

```text
Gold   = Bob
Silver = Alice
Bronze = Charlie
```

Different outcome.

Therefore:

```text
Order matters.
```

---

# Example 3: Password

Characters:

```text
A
B
C
```

Passwords:

```text
ABC
BAC
CAB
```

All are different.

---

# Example 4: Seating Arrangement

People:

```text
Tom
Jerry
Mike
```

Seats:

```text
1
2
3
```

Changing seats creates a different arrangement.

---

# Key Difference

## Permutation

```text
ABC
BAC
```

Different.

---

## Combination

```text
ABC
BAC
```

Same group.

---

Therefore:

```text
Permutation → Order Matters
Combination → Order Does Not Matter
```

---

# Factorial (n!)

## Simple Definition

Factorial is the mathematical operation used to count arrangements of all distinct objects.

Symbol:

\[
n!
\]

Read as:

```text
n factorial
```

---

# Formula

\[
n! = n \times (n-1) \times (n-2) \times \cdots \times 2 \times 1
\]

---

# Examples

## Example 1

\[
3!
\]

\[
=3\times2\times1
\]

\[
=6
\]

---

## Example 2

\[
4!
\]

\[
=4\times3\times2\times1
\]

\[
=24
\]

---

## Example 3

\[
5!
\]

\[
=5\times4\times3\times2\times1
\]

\[
=120
\]

---

## Example 4

\[
6!
\]

\[
=720
\]

---

# Why Factorial Works

Suppose:

```text
A B C
```

Three positions.

---

First position:

```text
3 choices
```

Second position:

```text
2 choices
```

Third position:

```text
1 choice
```

Using Product Rule:

\[
3\times2\times1
\]

\[
=6
\]

which is:

\[
3!
\]

---

# Important Special Case

\[
0! = 1
\]

This is defined by convention.

---

# Factorial Table

| n | n! |
|---|---|
| 0 | 1 |
| 1 | 1 |
| 2 | 2 |
| 3 | 6 |
| 4 | 24 |
| 5 | 120 |
| 6 | 720 |
| 7 | 5040 |
| 8 | 40320 |

---

# r-Permutation

## Simple Definition

Sometimes we do not arrange all objects.

We arrange only:

```text
r objects
```

chosen from:

```text
n objects
```

This is called an:

```text
r-Permutation
```

---

# Easy Way to Remember

```text
Choose r objects
AND
Arrange them
```

Order still matters.

---

# Example 1

Objects:

```text
A B C D
```

Choose:

```text
2 objects
```

Possible arrangements:

```text
AB
BA
AC
CA
AD
DA
BC
CB
BD
DB
CD
DC
```

Total:

```text
12
```

---

# Example 2

Students:

```text
5 students
```

Positions:

```text
President
Vice President
```

Order matters.

This is an r-permutation problem.

---

# Example 3

Digits:

```text
1 2 3 4 5
```

Create:

```text
3-digit numbers
```

without repetition.

This is also an r-permutation.

---

# Permutation Formula P(n,r)

## Formula

\[
P(n,r)
=
\frac{n!}{(n-r)!}
\]

---

## Alternative Form

\[
P(n,r)
=
n(n-1)(n-2)\cdots(n-r+1)
\]

---

# Why Does It Work?

For:

```text
r positions
```

we need only the first:

```text
r factors
```

of n!.

---

# Example 1

Choose and arrange:

```text
2 objects from 4
```

\[
P(4,2)
=
\frac{4!}{2!}
\]

\[
=
\frac{24}{2}
\]

\[
=12
\]

---

# Example 2

Choose and arrange:

```text
3 objects from 5
```

\[
P(5,3)
=
\frac{5!}{2!}
\]

\[
=
\frac{120}{2}
\]

\[
=60
\]

---

# Example 3

Choose and arrange:

```text
4 objects from 7
```

\[
P(7,4)
=
\frac{7!}{3!}
\]

\[
=
840
\]

---

# Shortcut Method

Instead of factorials:

\[
P(7,4)
=
7\times6\times5\times4
\]

\[
=840
\]

Same answer.

---

# Block Permutation
## (String / Block Binding)

---

# Simple Definition

Sometimes certain letters or objects must stay together.

Treat them as one single object.

This is called:

```text
Block Permutation
```

or

```text
Block Binding
```

---

# Example 1: Word BAD Must Stay Together

Letters:

```text
B A D C E
```

Requirement:

```text
BAD must stay together
```

Treat:

```text
BAD
```

as one object.

Now objects become:

```text
[BAD]
C
E
```

Total objects:

```text
3
```

Arrange:

\[
3!
\]

\[
=6
\]

---

# Example 2: Two Friends Sit Together

People:

```text
A B C D
```

Requirement:

```text
A and B sit together
```

Treat:

```text
AB
```

as one block.

Objects:

```text
[AB]
C
D
```

Arrange:

\[
3!
\]

\[
=6
\]

Inside block:

```text
AB
BA
```

2 possibilities.

Total:

\[
3!\times2
\]

\[
=12
\]

---

# Example 3: Word MATH

Requirement:

```text
AT stays together
```

Treat:

```text
[AT]
M
H
```

Arrange:

\[
3!
\]

Internal arrangement:

```text
AT
TA
```

Total:

\[
3!\times2
\]

\[
=12
\]

---

# Block Permutation Strategy

Step 1:

```text
Create block
```

Step 2:

```text
Treat block as one object
```

Step 3:

```text
Arrange objects
```

Step 4:

```text
Multiply by internal arrangements
```

---

# Permutation with Insertion
## (Gaps Method)

---

# Simple Definition

Sometimes a block must be inserted into the spaces around other objects.

Instead of arranging the block first, we:

1. Arrange the remaining objects.
2. Count available gaps.
3. Insert the block.

---

# Example 1: Insert X into ABC

Arrange:

```text
ABC
```

Available gaps:

```text
_ A _ B _ C _
```

Number of gaps:

```text
4
```

Insert X:

```text
XABC
AXBC
ABXC
ABCX
```

Total:

```text
4 ways
```

---

# Example 2: Insert BAD into CE

Arrange:

```text
C E
```

Gaps:

```text
_ C _ E _
```

Number of gaps:

```text
3
```

Insert BAD:

```text
BADCE
CBADE
CEBAD
```

Total:

```text
3 ways
```

---

# Example 3: Three People and One Couple

People:

```text
A
B
C
```

Couple:

```text
D,E
```

must stay together.

---

Arrange:

```text
A B C
```

\[
3! = 6
\]

For any arrangement:

```text
_ A _ B _ C _
```

Number of gaps:

```text
4
```

Insert block:

```text
(DE)
```

or

```text
(ED)
```

2 possibilities.

Total:

\[
3!\times4\times2
\]

\[
48
\]

---

# When to Use Gaps Method

Use when:

```text
A block must stay together
```

and it is easier to:

```text
Arrange others first
```

then

```text
Insert the block.
```

---

# Quick Summary Sheet

## Permutation

Ordered arrangement.

Remember:

```text
Order Matters
```

---

## Factorial

\[
n!
=
n(n-1)(n-2)\cdots1
\]

Used for arranging:

```text
All n objects
```

---

## r-Permutation

Arrange:

```text
r objects
```

from:

```text
n objects
```

---

## Permutation Formula

\[
P(n,r)
=
\frac{n!}{(n-r)!}
\]

---

## Block Permutation

When objects must stay together:

```text
Treat them as one block.
```

---

## Gaps Method

1. Arrange other objects.
2. Count gaps.
3. Insert block.

---

# Golden Rules

### Order Matters?

Use:

```text
Permutation
```

---

### Arrange All Objects?

Use:

\[
n!
\]

---

### Arrange Only r Objects?

Use:

\[
P(n,r)
=
\frac{n!}{(n-r)!}
\]

---

### Elements Must Stay Together?

Use:

```text
Block Permutation
```

or

```text
Gaps Method
```

---

### Quick Memory Trick

```text
Permutation = Position Matters

Combination = Position Doesn't Matter
```

This is the single most important idea to remember when studying permutations.