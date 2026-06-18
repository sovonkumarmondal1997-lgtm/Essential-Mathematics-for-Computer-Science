# Sequences and Patterns in Mathematics

---

# Introduction

So far, we have studied:

- Numbers
- Sets
- Functions
- Relations
- Vectors
- Matrices
- Linear Algebra

Now we begin another important topic:

# Sequences

Sequences appear everywhere:

- Mathematics
- Computer Science
- Algorithms
- Data Structures
- Machine Learning
- Finance
- Physics

A sequence is simply a pattern of numbers arranged in a specific order.

Understanding sequences helps us recognize patterns and build mathematical formulas.

---

# 1. Sequence

## Simple Definition

A **Sequence** is an ordered list of numbers or objects that follow a rule.

The order matters.

---

## Example 1

\[
1,2,3,4,5,\dots
\]

Rule:

Add 1 each time.

---

## Example 2

\[
2,4,6,8,10,\dots
\]

Rule:

Add 2 each time.

---

## Example 3

\[
1,4,9,16,25,\dots
\]

Rule:

Square numbers.

---

## Real-Life Example

Days of the week:

```
Monday
Tuesday
Wednesday
Thursday
Friday
```

This is a sequence because order matters.

---

## Another Real-Life Example

Floors in a building:

```
1st
2nd
3rd
4th
5th
```

A sequence.

---

# Why Sequences Matter

Sequences help us:

- Detect patterns
- Predict future values
- Create formulas
- Design algorithms

---

# 2. Term of a Sequence

## Simple Definition

Each individual item in a sequence is called a:

# Term

---

## Example

Sequence:

\[
2,4,6,8,10,\dots
\]

---

Terms:

\[
2
\]

is the first term.

---

\[
4
\]

is the second term.

---

\[
6
\]

is the third term.

---

## Notation

We usually write:

\[
u_1
\]

First term.

---

\[
u_2
\]

Second term.

---

\[
u_3
\]

Third term.

---

## Example

Sequence:

\[
5,10,15,20,\dots
\]

---

\[
u_1=5
\]

\[
u_2=10
\]

\[
u_3=15
\]

---

## Real-Life Example

Class roll numbers:

```
Student 1
Student 2
Student 3
```

Each student corresponds to a term in a sequence.

---

# 3. Natural Numbers

## Simple Definition

Natural numbers are counting numbers.

---

They start at:

\[
1
\]

and continue forever.

---

## Sequence

\[
1,2,3,4,5,6,\dots
\]

---

## Examples

### Example 1

Counting apples:

```
1 apple
2 apples
3 apples
4 apples
```

---

### Example 2

Counting books:

```
1
2
3
4
5
```

---

### Example 3

Classroom attendance:

```
Student 1
Student 2
Student 3
```

---

# Infinite Sequence

Natural numbers never end.

---

\[
1,2,3,4,5,\dots
\]

---

The dots:

\[
\dots
\]

mean:

"Continue forever."

---

# Why Important?

Natural numbers are used as positions in sequences.

---

# 4. Explicit Formula / Term Generator

## Simple Definition

An explicit formula directly calculates any term without needing previous terms.

---

Instead of writing:

\[
2,4,6,8,10,\dots
\]

we write a formula.

---

## General Idea

\[
u_n=f(n)
\]

where:

\[
n
\]

is the position.

---

## Example 1

Even numbers:

\[
u_n=2n
\]

---

Find 10th term:

\[
u_{10}=2(10)
\]

\[
=20
\]

---

## Example 2

Odd numbers:

\[
u_n=2n-1
\]

---

Find 8th term:

\[
u_8=2(8)-1
\]

\[
=15
\]

---

## Example 3

Squares:

\[
u_n=n^2
\]

---

Find 7th term:

\[
u_7=7^2
\]

\[
=49
\]

---

## Why Useful?

You can jump directly to any term.

No need to calculate all previous terms.

---

# 5. Even Numbers Sequence

## Simple Definition

Even numbers are divisible by 2.

---

Sequence:

\[
2,4,6,8,10,\dots
\]

---

## Formula

\[
u_n=2n
\]

---

## Example 1

First term:

\[
u_1=2(1)=2
\]

---

## Example 2

Fourth term:

\[
u_4=2(4)=8
\]

---

## Example 3

Tenth term:

\[
u_{10}=20
\]

---

## Table

| n | \(u_n=2n\) |
|---|---|
|1|2|
|2|4|
|3|6|
|4|8|
|5|10|

---

## Real-Life Example

House numbers on one side of a street:

```
2
4
6
8
10
```

---

# 6. Sequence Indexing / Starting Term Convention

## Simple Definition

Every term has a position number called its index.

---

## Common Convention

We usually start with:

\[
u_1
\]

instead of:

\[
u_0
\]

---

## Example

Sequence:

\[
3,6,9,12,\dots
\]

---

\[
u_1=3
\]

\[
u_2=6
\]

\[
u_3=9
\]

---

## Why Start at 1?

Because sequences traditionally follow natural numbers:

\[
1,2,3,\dots
\]

---

## Example 2

Students in a class:

```
Student 1
Student 2
Student 3
```

not

```
Student 0
```

---

## Example 3

Floors of a building:

```
1st Floor
2nd Floor
3rd Floor
```

---

# Important Note

In computer science:

Arrays often start at:

\[
0
\]

but mathematical sequences usually start at:

\[
1
\]

---

# 7. Odd Numbers Sequence

## Simple Definition

Odd numbers are not divisible by 2.

---

Sequence:

\[
1,3,5,7,9,\dots
\]

---

## Formula

\[
u_n=2n-1
\]

---

## Example 1

\[
u_1=1
\]

---

## Example 2

\[
u_4=7
\]

---

## Example 3

\[
u_{10}=19
\]

---

## Table

| n | \(u_n\) |
|---|---|
|1|1|
|2|3|
|3|5|
|4|7|
|5|9|

---

## Real-Life Example

Odd house numbers:

```
1
3
5
7
9
```

---

# 8. Perfect Squares Sequence

## Simple Definition

Perfect squares are numbers obtained by multiplying a number by itself.

---

## Formula

\[
u_n=n^2
\]

---

## Sequence

\[
1,4,9,16,25,36,\dots
\]

---

## Example 1

\[
u_1=1^2=1
\]

---

## Example 2

\[
u_4=4^2=16
\]

---

## Example 3

\[
u_{10}=10^2=100
\]

---

## Table

| n | \(n^2\) |
|---|---|
|1|1|
|2|4|
|3|9|
|4|16|
|5|25|

---

## Real-Life Example

Square floor tiles.

```
1×1 = 1 tile

2×2 = 4 tiles

3×3 = 9 tiles

4×4 = 16 tiles
```

---

# 9. Sequence of Differences / First Differences

## Simple Definition

First differences show how much a sequence increases between consecutive terms.

---

## Formula

Subtract neighboring terms.

---

# Example 1

Natural Numbers

\[
1,2,3,4,5
\]

Differences:

\[
1,1,1,1
\]

---

## Example 2

Even Numbers

\[
2,4,6,8,10
\]

Differences:

\[
2,2,2,2
\]

---

## Example 3

Odd Numbers

\[
1,3,5,7,9
\]

Differences:

\[
2,2,2,2
\]

---

# Interesting Example

Perfect Squares

\[
1,4,9,16,25
\]

---

Differences:

\[
4-1=3
\]

\[
9-4=5
\]

\[
16-9=7
\]

\[
25-16=9
\]

---

Result:

\[
3,5,7,9
\]

---

Notice:

The differences themselves form a pattern.

---

# Another Example

Sequence:

\[
2,6,12,20,30
\]

---

Differences:

\[
4,6,8,10
\]

---

Again:

Pattern appears.

---

# Why First Differences Matter

They help us:

- Discover formulas
- Predict future terms
- Analyze patterns

---

# Real-Life Example

Daily savings:

```
Day 1 = ₹100
Day 2 = ₹150
Day 3 = ₹200
Day 4 = ₹250
```

Differences:

```
+50
+50
+50
```

This reveals the saving pattern.

---

# Complete Big Picture

## Sequence

An ordered list following a rule.

---

## Term

An individual item in a sequence.

---

## Natural Numbers

\[
1,2,3,4,5,\dots
\]

---

## Explicit Formula

A direct rule:

\[
u_n=f(n)
\]

---

## Even Numbers

\[
u_n=2n
\]

Sequence:

\[
2,4,6,8,\dots
\]

---

## Odd Numbers

\[
u_n=2n-1
\]

Sequence:

\[
1,3,5,7,\dots
\]

---

## Perfect Squares

\[
u_n=n^2
\]

Sequence:

\[
1,4,9,16,\dots
\]

---

## Indexing

Usually begins with:

\[
u_1
\]

---

## First Differences

Measure how much consecutive terms increase.

---

These concepts form the foundation for:

- Arithmetic Sequences
- Geometric Sequences
- Series
- Recurrence Relations
- Algorithm Analysis
- Dynamic Programming
- Machine Learning
- Time-Series Forecasting
- Signal Processing
- Financial Modeling

where identifying patterns in ordered data is critically important.