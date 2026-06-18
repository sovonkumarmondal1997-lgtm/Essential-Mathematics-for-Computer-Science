# The Pigeonhole Principle - Complete Beginner's Guide

# Table of Contents

1. Introduction
2. The Pigeonhole Principle
3. Pigeons (Objects/Elements)
4. Pigeonholes (Containers/Boxes/Sets)
5. The Generalized Pigeonhole Principle
6. The Ceiling Function
7. How to Solve Pigeonhole Problems
8. Real-Life Applications
9. Quick Summary Sheet

---

# Introduction

The **Pigeonhole Principle** is one of the simplest yet most powerful ideas in combinatorics and discrete mathematics.

It helps answer questions like:

- How many people are needed to guarantee two share a birthday month?
- How many socks must be selected to guarantee a matching color?
- How many numbers must be chosen to guarantee two have the same remainder?

The idea is surprisingly simple:

> If there are more objects than containers, some container must hold more than one object.

---

# The Pigeonhole Principle

## Simple Definition

If:

\[
k+1
\]

or more objects are placed into

\[
k
\]

containers,

then at least one container must contain two or more objects.

---

## Easy Way to Remember

Imagine:

```text
4 pigeons
3 pigeonholes
```

Try putting:

```text
1 pigeon in each hole
```

You use:

```text
3 holes
```

But:

```text
1 pigeon remains.
```

Therefore:

```text
One hole must contain at least 2 pigeons.
```

---

# Visual Example

```text
Pigeons:

A
B
C
D

Holes:

1
2
3
```

Possible arrangement:

```text
Hole 1 → A,D
Hole 2 → B
Hole 3 → C
```

Notice:

```text
Hole 1 has two pigeons.
```

---

# Example 1: Birth Months

There are:

```text
13 people
```

Birth months:

```text
12 months
```

Since:

\[
13 > 12
\]

At least two people must share a birth month.

---

# Example 2: Socks

Colors:

```text
Red
Blue
Green
```

Three color categories.

Pick:

```text
4 socks
```

Since:

```text
4 objects
3 categories
```

At least two socks share a color.

---

# Example 3: Students and Grades

Grade categories:

```text
A
B
C
D
```

Four categories.

If:

```text
5 students
```

exist,

then at least two students have the same grade.

---

# Pigeons (Objects/Elements)

## Simple Definition

Pigeons are the items being distributed.

Think:

```text
What am I placing?
```

Those are the pigeons.

---

# Common Pigeons

Examples include:

- Students
- People
- Cards
- Numbers
- Socks
- Balls
- Books
- Passwords

---

# Example 1: Birth Month Problem

Question:

```text
13 people
12 months
```

Pigeons:

```text
People
```

Because people are being assigned to months.

---

# Example 2: Remainder Problem

Question:

```text
6 integers
```

grouped by remainder modulo 5.

Pigeons:

```text
The integers
```

---

# Example 3: Cards

Question:

```text
5 cards
```

grouped by suit.

Pigeons:

```text
The cards
```

---

# Example 4: Students in Classrooms

Question:

```text
100 students
12 classrooms
```

Pigeons:

```text
Students
```

---

# Key Question

Whenever you see a pigeonhole problem, ask:

```text
What is being distributed?
```

That is the pigeon.

---

# Pigeonholes (Containers/Boxes/Sets)

## Simple Definition

Pigeonholes are the categories or containers into which pigeons are placed.

Think:

```text
Where are the objects going?
```

Those are the pigeonholes.

---

# Example 1: Birth Month Problem

People are grouped by:

```text
January
February
...
December
```

Pigeonholes:

```text
12 months
```

---

# Example 2: Card Suits

Cards are grouped by:

```text
Hearts
Diamonds
Clubs
Spades
```

Pigeonholes:

```text
4 suits
```

---

# Example 3: Remainders Modulo 5

Possible remainders:

```text
0
1
2
3
4
```

Pigeonholes:

```text
5 remainder classes
```

---

# Example 4: Hair Colors

Categories:

```text
Black
Brown
Blonde
Red
```

Pigeonholes:

```text
Hair color groups
```

---

# Example 5: Pairs Summing to 12

Numbers:

```text
1 to 11
```

Pairs:

```text
(1,11)
(2,10)
(3,9)
(4,8)
(5,7)
```

Each pair acts as a pigeonhole.

---

# Example 6: Pairs Differing by 2

Numbers:

```text
1,3
2,4
3,5
4,6
```

Each valid pair can be viewed as a category.

---

# Key Question

Ask:

```text
Into what groups am I placing the objects?
```

That is the pigeonhole.

---

# Pigeonhole Problems as a Table

| Situation | Pigeons | Pigeonholes |
|------------|----------|-------------|
| People and months | People | Months |
| Cards and suits | Cards | Suits |
| Integers mod 5 | Integers | Remainders |
| Students and grades | Students | Grades |
| Socks and colors | Socks | Colors |

---

# The Generalized Pigeonhole Principle

## Simple Definition

The ordinary pigeonhole principle guarantees:

```text
A duplicate.
```

The generalized version tells us:

```text
How many duplicates are guaranteed.
```

---

# Formula

If:

\[
N
\]

objects are placed into

\[
k
\]

boxes,

then at least one box contains:

\[
\left\lceil \frac{N}{k} \right\rceil
\]

objects.

---

# Meaning

Spread objects as evenly as possible.

Even then:

```text
One box must reach
Ceiling(N/k)
```

objects.

---

# Example 1: 10 Balls into 3 Boxes

\[
\left\lceil \frac{10}{3} \right\rceil
=
\left\lceil 3.33 \right\rceil
=
4
\]

Therefore:

```text
One box contains at least 4 balls.
```

---

# Example 2: 100 Students into 12 Rooms

\[
\left\lceil \frac{100}{12} \right\rceil
=
\left\lceil 8.33 \right\rceil
=
9
\]

Therefore:

```text
At least one room contains 9 students.
```

---

# Example 3: 50 Cards into 4 Suits

\[
\left\lceil \frac{50}{4} \right\rceil
=
13
\]

Therefore:

```text
At least one suit contains 13 cards.
```

---

# Example 4: 25 Books on 6 Shelves

\[
\left\lceil \frac{25}{6} \right\rceil
=
5
\]

Therefore:

```text
At least one shelf has 5 books.
```

---

# Why Does It Work?

Suppose:

```text
10 balls
3 boxes
```

Try keeping every box below:

```text
4 balls
```

Maximum possible:

```text
3 + 3 + 3 = 9
```

But:

```text
10 balls exist.
```

Impossible.

So one box must contain:

```text
4 or more.
```

---

# The Ceiling Function

## Symbol

\[
\lceil x \rceil
\]

Read as:

```text
Ceiling of x
```

---

# Simple Definition

The ceiling function rounds a number:

```text
UP
```

to the nearest integer.

---

# Examples

## Example 1

\[
\lceil 2.1 \rceil = 3
\]

---

## Example 2

\[
\lceil 4.9 \rceil = 5
\]

---

## Example 3

\[
\lceil 7 \rceil = 7
\]

---

## Example 4

\[
\lceil 8.01 \rceil = 9
\]

---

# Why Ceiling Is Needed

Suppose:

\[
100/12
=
8.33
\]

We cannot have:

```text
8.33 students
```

in a room.

To guarantee enough space:

```text
Round upward
```

Therefore:

\[
\lceil 8.33 \rceil
=
9
\]

---

# More Ceiling Examples

### Example 1

\[
\lceil 11/5 \rceil
=
\lceil 2.2 \rceil
=
3
\]

---

### Example 2

\[
\lceil 20/4 \rceil
=
5
\]

---

### Example 3

\[
\lceil 31/6 \rceil
=
\lceil 5.17 \rceil
=
6
\]

---

### Example 4

\[
\lceil 99/10 \rceil
=
10
\]

---

# How to Solve Pigeonhole Problems

## Step 1

Identify:

```text
What are the pigeons?
```

---

## Step 2

Identify:

```text
What are the pigeonholes?
```

---

## Step 3

Count:

```text
Number of pigeons
```

and

```text
Number of holes
```

---

## Step 4

Apply:

### Basic Principle

\[
k+1
\]

objects into

\[
k
\]

holes.

---

### Generalized Principle

\[
\left\lceil \frac{N}{k} \right\rceil
\]

---

# Real-Life Applications

## Birthdays

Guaranteeing shared birthday months.

---

## Computer Science

Hash table collisions.

---

## Networking

Packet distribution.

---

## Data Engineering

Data partition balancing.

---

## Database Sharding

Ensuring minimum records per shard.

---

## Scheduling

Assigning employees to shifts.

---

## Load Balancing

Distributing requests among servers.

---

# Quick Summary Sheet

## Pigeonhole Principle

If:

\[
k+1
\]

objects go into

\[
k
\]

boxes,

then one box contains at least:

```text
2 objects.
```

---

## Pigeons

The objects being distributed.

Examples:

```text
People
Cards
Numbers
Students
Books
```

---

## Pigeonholes

The categories receiving the objects.

Examples:

```text
Months
Suits
Remainders
Colors
Shelves
```

---

## Generalized Pigeonhole Principle

If:

\[
N
\]

objects go into

\[
k
\]

boxes,

then some box contains at least:

\[
\left\lceil \frac{N}{k} \right\rceil
\]

objects.

---

## Ceiling Function

\[
\lceil x \rceil
\]

means:

```text
Round Up
```

Examples:

```text
⌈2.1⌉ = 3
⌈7.8⌉ = 8
⌈9⌉ = 9
```

---

# Golden Rules

### More Objects Than Boxes

Use:

```text
Basic Pigeonhole Principle
```

---

### Need Minimum Guaranteed Occupancy

Use:

\[
\left\lceil \frac{N}{k} \right\rceil
\]

---

### Always Ask

```text
What are the pigeons?
```

and

```text
What are the pigeonholes?
```

before solving the problem.

Once those are identified, most pigeonhole problems become straightforward.