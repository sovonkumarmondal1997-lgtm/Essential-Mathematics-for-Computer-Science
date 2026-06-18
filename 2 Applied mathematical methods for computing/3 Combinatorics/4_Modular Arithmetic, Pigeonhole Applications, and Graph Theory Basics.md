# Modular Arithmetic, Pigeonhole Applications, and Graph Theory Basics

# Table of Contents

1. Modular Arithmetic Remainders
2. Pigeonhole Principle Application to Remainders
3. Worst-Case Scenario Counting (Guarantee Thresholds)
4. Generalized Pigeonhole Principle via Ceiling Function
5. Complementary Pairing (Target Sum Subsets)
6. Simple Graph Degree Properties (Friendship Logic)
7. Identical Degrees in a Graph
8. Quick Summary Sheet

---

# Modular Arithmetic Remainders

## Simple Definition

When we divide a number by another number, we get:

- Quotient
- Remainder

Modular arithmetic focuses on the remainder.

Example:

\[
17 \div 5
\]

\[
17 = 5 \times 3 + 2
\]

Remainder:

\[
2
\]

Therefore:

\[
17 \equiv 2 \pmod 5
\]

Read as:

```text
17 is congruent to 2 modulo 5
```

---

# Why Is This Useful?

Instead of thinking about infinitely many integers:

```text
..., -10, -9, -8, ...
```

we can group them into a small number of remainder classes.

For modulus 5, there are only:

```text
0
1
2
3
4
```

possible remainders.

These become our "boxes."

---

# Example 1: Modulo 3

Possible remainders:

```text
0
1
2
```

Group numbers:

### Remainder 0

```text
0,3,6,9,12,15,...
```

### Remainder 1

```text
1,4,7,10,13,16,...
```

### Remainder 2

```text
2,5,8,11,14,17,...
```

---

# Example 2: Modulo 4

Possible remainders:

```text
0,1,2,3
```

Examples:

```text
8 mod 4 = 0
13 mod 4 = 1
18 mod 4 = 2
23 mod 4 = 3
```

---

# Example 3: Modulo 10

Possible remainder classes:

```text
0,1,2,3,4,5,6,7,8,9
```

Examples:

```text
37 mod 10 = 7
84 mod 10 = 4
123 mod 10 = 3
```

Notice:

```text
The last digit determines the remainder modulo 10.
```

---

# Key Idea

For modulus k:

Possible remainders are:

\[
0,1,2,\dots,k-1
\]

Exactly:

\[
k
\]

remainder classes exist.

---

# Pigeonhole Principle Application to Remainders

## Simple Definition

Suppose numbers are grouped according to their remainders modulo k.

There are only:

\[
k
\]

possible remainder classes.

If we choose:

\[
k+1
\]

numbers, then at least two numbers must fall into the same remainder class.

This follows directly from the Pigeonhole Principle.

---

# Formula

For modulus:

\[
k
\]

There are:

\[
k
\]

boxes (remainder classes).

Selecting:

\[
k+1
\]

numbers guarantees two numbers with the same remainder.

---

# Example 1: Modulo 5

Possible remainders:

```text
0,1,2,3,4
```

Total boxes:

```text
5
```

Choose:

```text
6 numbers
```

By the Pigeonhole Principle:

```text
At least two numbers have the same remainder modulo 5.
```

---

# Example 2: Modulo 10

Possible remainders:

```text
0-9
```

10 remainder classes.

Choose:

```text
11 integers
```

Guaranteed:

```text
Two integers share the same last digit.
```

---

# Example 3: Modulo 3

Possible remainders:

```text
0
1
2
```

Choose:

```text
4 numbers
```

Guaranteed:

```text
At least two numbers have the same remainder when divided by 3.
```

---

# Real Example

Numbers:

```text
11
17
24
31
```

Modulo 3:

```text
11 mod 3 = 2
17 mod 3 = 2
24 mod 3 = 0
31 mod 3 = 1
```

Notice:

```text
11 and 17 share remainder 2.
```

---

# Worst-Case Scenario Counting
## (Guarantee Thresholds)

---

## Simple Definition

Many counting problems ask:

```text
How many items must I select
to guarantee a certain outcome?
```

The key word is:

```text
Guarantee
```

We do NOT assume luck.

Instead we assume the worst possible arrangement.

---

# Why Worst Case?

Suppose a drawer contains:

```text
5 red socks
5 blue socks
```

Question:

```text
How many socks must I take
to guarantee a matching pair?
```

---

## Wrong Thinking

Maybe:

```text
2 socks
```

Not guaranteed.

You could get:

```text
1 red
1 blue
```

---

## Worst Case

Take:

```text
1 red
1 blue
```

No pair yet.

Next sock:

```text
Must match one color.
```

Total needed:

```text
3 socks
```

---

# Example 1: Birth Months

Months:

```text
12
```

To guarantee two people share a birth month:

Worst case:

```text
1 person per month
```

\[
12
\]

people.

One more person forces repetition.

Answer:

\[
13
\]

---

# Example 2: Suit Matching

Card suits:

```text
4
```

Worst case:

```text
1 card from each suit
```

Need:

\[
4+1=5
\]

cards.

---

# Example 3: Remainders Modulo 7

Remainders:

```text
0,1,2,3,4,5,6
```

7 boxes.

Worst case:

```text
One number in each class.
```

Need:

\[
8
\]

numbers to guarantee a duplicate remainder.

---

# Generalized Pigeonhole Principle via Ceiling Function

## Formula

If:

\[
n
\]

objects go into

\[
k
\]

boxes,

then some box contains at least:

\[
\left\lceil \frac{n}{k} \right\rceil
\]

objects.

---

# What Does This Mean?

Imagine distributing objects as evenly as possible.

Even then, at least one box reaches:

\[
\left\lceil \frac{n}{k} \right\rceil
\]

---

# Example 1: 20 Balls into 6 Boxes

\[
\left\lceil \frac{20}{6} \right\rceil
=
\left\lceil 3.33 \right\rceil
=
4
\]

Guaranteed:

```text
One box has at least 4 balls.
```

---

# Example 2: 100 Students into 9 Rooms

\[
\left\lceil \frac{100}{9} \right\rceil
=
12
\]

Guaranteed:

```text
One room contains at least 12 students.
```

---

# Example 3: 50 Cards into 4 Suits

\[
\left\lceil \frac{50}{4} \right\rceil
=
13
\]

Guaranteed:

```text
One suit contains at least 13 cards.
```

---

# Using It to Find Thresholds

Suppose we want:

```text
At least 5 objects
in one box.
```

Boxes:

```text
8
```

Question:

```text
How many objects are needed?
```

---

## Worst Case

Keep every box at:

```text
4
```

objects.

Maximum:

\[
8 \times 4
=
32
\]

One more object forces:

```text
5 in some box.
```

Answer:

\[
33
\]

---

# Complementary Pairing
## (Target Sum Subsets)

---

## Simple Definition

Sometimes numbers can be grouped into pairs that add to a specific target.

Example target:

\[
9
\]

Pairs:

```text
0 + 9
1 + 8
2 + 7
3 + 6
4 + 5
```

These are called complementary pairs.

---

# Why Is This Useful?

Many Pigeonhole problems use these pairs as boxes.

---

# Example 1: Numbers 0-9

Target:

\[
9
\]

Pairs:

```text
(0,9)
(1,8)
(2,7)
(3,6)
(4,5)
```

Total boxes:

```text
5
```

Choose:

```text
6 numbers
```

Guaranteed:

```text
Some pair sums to 9.
```

---

# Example 2: Numbers 1-10

Target:

\[
11
\]

Pairs:

```text
(1,10)
(2,9)
(3,8)
(4,7)
(5,6)
```

Choose:

```text
6 numbers
```

Guaranteed:

```text
Two selected numbers sum to 11.
```

---

# Example 3: Numbers 1-20

Target:

\[
21
\]

Pairs:

```text
(1,20)
(2,19)
(3,18)
...
(10,11)
```

There are:

```text
10 complementary pairs.
```

Selecting:

```text
11 numbers
```

guarantees a pair summing to 21.

---

# Simple Graph Degree Properties
## (Friendship Logic)

---

# What Is a Graph?

A graph contains:

- Vertices (people)
- Edges (friendships)

Example:

```text
Alice ----- Bob
     \
      \
      Charlie
```

---

# Degree

The degree of a vertex means:

```text
Number of connections
```

or

```text
Number of friends
```

---

# Example

Suppose:

```text
Alice knows Bob and Charlie
```

Degree:

\[
2
\]

---

# Friendship Logic

Suppose there are:

\[
n
\]

people.

Can someone have:

\[
n
\]

friends?

No.

Why?

Because:

```text
You cannot be your own friend.
```

Maximum friends:

\[
n-1
\]

---

# Example 1

5 people:

```text
A
B
C
D
E
```

Maximum friends for any person:

\[
5-1=4
\]

---

# Example 2

100 people.

Maximum friends:

\[
99
\]

---

# Example 3

20 people.

Maximum friends:

\[
19
\]

---

# Key Rule

Possible degrees:

\[
0,1,2,\dots,n-1
\]

---

# Identical Degrees in a Graph

## Theorem

In every simple graph with:

\[
n
\]

vertices,

at least two vertices have exactly the same degree.

---

# Why Is This True?

Possible degrees:

\[
0,1,2,\dots,n-1
\]

Looks like:

\[
n
\]

choices.

But:

```text
Degree 0 and Degree n−1
cannot occur simultaneously.
```

---

# Why?

If someone has degree:

\[
n-1
\]

they know everyone.

Therefore:

```text
Nobody has degree 0.
```

---

# So Only n−1 Degree Values Exist

Instead of:

\[
n
\]

possible degrees,

we effectively have:

\[
n-1
\]

degree categories.

---

# Apply Pigeonhole Principle

Vertices:

\[
n
\]

Degree categories:

\[
n-1
\]

Therefore:

```text
At least two vertices
share the same degree.
```

---

# Example 1: 4 People

Possible degrees:

```text
0,1,2,3
```

But:

```text
0 and 3 cannot both occur.
```

Only:

```text
3 degree categories.
```

Four people:

```text
4 people
3 categories
```

Therefore:

```text
Two people have the same degree.
```

---

# Example 2: 5 People

People:

```text
5
```

Possible degree categories:

```text
0,1,2,3,4
```

Again:

```text
0 and 4 cannot both exist.
```

Only:

```text
4 categories.
```

Five people:

```text
5 people
4 categories
```

Guaranteed duplicate degree.

---

# Example 3: Friendship Network

Friend counts:

```text
1
2
2
4
5
```

Notice:

```text
Two people have degree 2.
```

The theorem is satisfied.

---

# Quick Summary Sheet

## Modular Arithmetic

Groups integers by remainders.

For modulus k:

\[
0,1,2,\dots,k-1
\]

---

## Pigeonhole on Remainders

Choose:

\[
k+1
\]

integers.

Guaranteed:

```text
Two share the same remainder modulo k.
```

---

## Worst-Case Counting

To guarantee an outcome:

1. Avoid success as long as possible.
2. Count that maximum.
3. Add one more.

---

## Generalized Pigeonhole Principle

\[
\left\lceil \frac{n}{k} \right\rceil
\]

gives the minimum guaranteed occupancy.

---

## Complementary Pairing

Group numbers into target-sum pairs.

Examples:

```text
(1,10)
(2,9)
(3,8)
```

Useful as pigeonhole categories.

---

## Graph Degree Rule

In a group of n people:

Maximum friends:

\[
n-1
\]

---

## Identical Degree Theorem

Every simple graph with n vertices contains:

```text
At least two vertices
with the same degree.
```

This follows from the Pigeonhole Principle.

---

# Golden Rules

### Remainders → Boxes

Modulo k gives:

\[
k
\]

boxes.

---

### Guarantee Problems

Think:

```text
Worst Case First
```

---

### Target Sum Problems

Use:

```text
Complementary Pairs
```

---

### Friendship Problems

Maximum friends:

\[
n-1
\]

---

### Graph Degree Proofs

Use:

```text
Pigeonhole Principle
+
Degree Categories
```

to show duplicate degrees must exist.