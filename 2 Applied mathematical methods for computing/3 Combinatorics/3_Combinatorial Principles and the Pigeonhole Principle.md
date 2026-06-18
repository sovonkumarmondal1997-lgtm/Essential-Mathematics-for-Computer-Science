# Combinatorial Principles and the Pigeonhole Principle

# Table of Contents

1. Combinatorial Principle
2. Pigeonhole Principle (Dirichlet's Box Principle)
3. Card Suit Distribution
4. Generalized Pigeonhole Principle
5. Proof by Contradiction
6. Quick Summary Sheet

---

# Combinatorial Principle

## Simple Definition

A **Combinatorial Principle** is a basic rule or theorem used to solve problems involving:

- Counting
- Arranging
- Selecting
- Distributing objects

Instead of listing every possibility, combinatorial principles help us calculate answers efficiently.

---

## Why Are Combinatorial Principles Important?

Suppose you want to know:

```text
How many passwords can be created?
```

or

```text
How many ways can students sit in a row?
```

or

```text
How many ways can cards be dealt?
```

Listing every possibility would take forever.

Combinatorial principles provide shortcuts.

---

# Common Combinatorial Principles

Some important principles are:

1. Product Rule
2. Sum Rule
3. Complement Counting Principle
4. Inclusion-Exclusion Principle
5. Pigeonhole Principle

---

# Example 1: Product Rule

You have:

```text
3 shirts
4 pants
```

Number of outfits:

\[
3 \times 4 = 12
\]

---

# Example 2: Sum Rule

Choose:

```text
5 juices
OR
3 soft drinks
```

Total:

\[
5+3=8
\]

---

# Example 3: Complement Counting

How many 4-digit codes contain at least one 5?

Total:

\[
10^4
\]

No 5:

\[
9^4
\]

Desired:

\[
10^4-9^4
\]

---

## Key Idea

Combinatorial principles help answer:

```text
How many?
```

without manually counting.

---

# Pigeonhole Principle
## (Dirichlet's Box Principle)

---

## Simple Definition

The Pigeonhole Principle states:

> If more objects than boxes are distributed into the boxes, then at least one box must contain more than one object.

Mathematically:

If:

\[
k+1
\]

or more objects are placed into

\[
k
\]

boxes,

then at least one box contains at least two objects.

---

# Why Is It Called Pigeonhole?

Imagine:

```text
4 pigeons
3 pigeonholes
```

Trying to place:

```text
1 pigeon per hole
```

uses:

```text
3 holes
```

But there is still:

```text
1 extra pigeon
```

Therefore:

```text
Some hole must contain at least 2 pigeons.
```

---

# Visual Example

Boxes:

```text
Box A
Box B
Box C
```

Objects:

```text
1
2
3
4
```

Possible arrangement:

```text
A → 1,4
B → 2
C → 3
```

Notice:

```text
Box A contains 2 objects.
```

---

# Example 1: Students and Birth Months

There are:

```text
13 students
```

Birth months:

```text
12 months
```

Since:

\[
13 > 12
\]

At least two students must share a birth month.

### Answer

```text
At least two students have birthdays in the same month.
```

---

# Example 2: Socks

You own:

```text
5 pairs of socks
```

Colors:

```text
Red
Blue
Black
White
Green
```

Suppose you randomly pick:

```text
6 socks
```

Since:

```text
6 socks
5 color categories
```

At least one color must appear twice.

---

# Example 3: People and Days of the Week

There are:

```text
8 people
```

Days:

```text
Monday-Sunday
```

which gives:

```text
7 days
```

Since:

\[
8 > 7
\]

At least two people were born on the same day of the week.

---

# Card Suit Distribution

## Simple Definition

A deck of cards has four suits:

- Hearts
- Diamonds
- Clubs
- Spades

These suits can act as "boxes" in a pigeonhole problem.

---

# Standard Deck

Total cards:

```text
52
```

Suits:

```text
Hearts
Diamonds
Clubs
Spades
```

Each suit:

```text
13 cards
```

---

# Visual Representation

```text
Hearts    → Box 1
Diamonds  → Box 2
Clubs     → Box 3
Spades    → Box 4
```

---

# Example 1: Five Cards

Suppose you draw:

```text
5 cards
```

There are:

```text
4 suits
```

Using the Pigeonhole Principle:

\[
5 > 4
\]

Therefore:

```text
At least two cards belong to the same suit.
```

---

# Example 2: Nine Cards

Draw:

```text
9 cards
```

Suit boxes:

```text
4
```

Using the generalized version:

\[
\lceil 9/4 \rceil = 3
\]

At least one suit contains:

```text
3 cards
```

---

# Example 3: Thirteen Cards

Draw:

```text
13 cards
```

Suits:

```text
4
```

\[
\lceil 13/4 \rceil = 4
\]

Therefore:

```text
At least one suit appears at least 4 times.
```

---

# Generalized Pigeonhole Principle

## Simple Definition

The ordinary pigeonhole principle says:

```text
More objects than boxes
```

forces repetition.

The generalized version tells us:

```text
How much repetition must occur.
```

---

# Formula

If:

\[
n
\]

objects are placed into

\[
k
\]

boxes,

then at least one box contains:

\[
\left\lceil \frac{n}{k} \right\rceil
\]

objects.

---

## What Is Ceiling?

The symbol:

\[
\lceil x \rceil
\]

means:

```text
Round upward
```

Examples:

\[
\lceil 2.1 \rceil = 3
\]

\[
\lceil 4.8 \rceil = 5
\]

---

# Example 1: 10 Balls into 3 Boxes

\[
\left\lceil \frac{10}{3} \right\rceil
=
\left\lceil 3.33 \right\rceil
=
4
\]

### Answer

At least one box contains:

```text
4 balls
```

---

# Example 2: 25 Students into 4 Groups

\[
\left\lceil \frac{25}{4} \right\rceil
=
\left\lceil 6.25 \right\rceil
=
7
\]

### Answer

At least one group contains:

```text
7 students
```

---

# Example 3: 100 Books on 9 Shelves

\[
\left\lceil \frac{100}{9} \right\rceil
=
12
\]

### Answer

At least one shelf contains:

```text
12 books
```

---

# Example 4: 50 Cards into 4 Suits

\[
\left\lceil \frac{50}{4} \right\rceil
=
13
\]

### Answer

At least one suit contains:

```text
13 cards
```

---

# Why Does the Formula Work?

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

Therefore:

```text
One box must contain 4 balls.
```

---

# Proof by Contradiction

## Simple Definition

Proof by contradiction is a method where:

1. Assume the opposite of what we want to prove.
2. Follow the consequences.
3. Reach an impossible result.
4. Conclude the original statement must be true.

---

# Everyday Example

Claim:

```text
There is at least one student in class.
```

Suppose the opposite:

```text
No students are in class.
```

You look inside and see:

```text
20 students.
```

Contradiction.

Therefore:

```text
The assumption was wrong.
```

---

# Example 1: Proving the Basic Pigeonhole Principle

Claim:

```text
4 objects
3 boxes
```

must produce a repeated box.

---

## Assume Opposite

Suppose:

```text
No box contains more than one object.
```

Then each box can contain at most:

```text
1 object
```

Maximum capacity:

```text
3 boxes × 1
=
3 objects
```

But:

```text
4 objects exist.
```

Impossible.

Contradiction.

Therefore:

```text
At least one box contains two objects.
```

---

# Example 2: Generalized Principle

Claim:

```text
10 balls
3 boxes
```

At least one box contains:

```text
4 balls.
```

---

## Assume Opposite

Suppose:

```text
Every box has at most 3 balls.
```

Maximum balls:

\[
3+3+3=9
\]

But:

```text
10 balls exist.
```

Contradiction.

Therefore:

```text
One box must contain at least 4 balls.
```

---

# Example 3: Birth Month Problem

Claim:

```text
13 students
12 months
```

At least two students share a birth month.

---

## Assume Opposite

Suppose:

```text
No month contains more than one student.
```

Then maximum students:

```text
12
```

But:

```text
13 students exist.
```

Contradiction.

Therefore:

```text
At least two students share a birth month.
```

---

# Quick Summary Sheet

## Combinatorial Principle

General counting rules used to solve:

```text
Counting
Selecting
Arranging
Distributing
```

problems.

---

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

then at least one box contains:

```text
2 or more objects
```

---

## Card Suit Distribution

Treat suits as boxes:

```text
Hearts
Diamonds
Clubs
Spades
```

Use pigeonhole reasoning to determine suit repetitions.

---

## Generalized Pigeonhole Principle

If:

\[
n
\]

objects go into

\[
k
\]

boxes,

then at least one box contains:

\[
\left\lceil \frac{n}{k} \right\rceil
\]

objects.

---

## Proof by Contradiction

Steps:

1. Assume the opposite.
2. Derive consequences.
3. Reach an impossibility.
4. Reject the assumption.
5. Original statement is true.

---

# Golden Rules

### More Objects Than Boxes

Use:

```text
Pigeonhole Principle
```

---

### Need Minimum Guaranteed Repetition

Use:

\[
\left\lceil \frac{n}{k} \right\rceil
\]

---

### Card Suit Problems

Treat:

```text
4 suits = 4 boxes
```

---

### Formal Proof

Use:

```text
Proof by Contradiction
```

The contradiction usually comes from showing that the boxes cannot hold all the objects under the opposite assumption.