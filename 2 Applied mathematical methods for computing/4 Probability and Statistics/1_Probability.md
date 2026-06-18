# Probability - Complete Beginner's Guide

# Table of Contents

1. Introduction to Probability
2. Probability
3. Impossible Event
4. Certain Event
5. Equally Likely Events (Unbiased Outcomes)
6. Theoretical Probability (Classical Definition)
7. Mutually Exclusive Events
8. Independent Events
9. Dependent Events
10. Sample Space Table (Two Dice Experiment)
11. Complementary Events
12. Quick Summary Sheet

---

# Introduction to Probability

Probability is the branch of mathematics that studies:

```text
Chance
Uncertainty
Likelihood
```

It helps answer questions such as:

- What is the chance of getting a Head?
- What is the chance of rain tomorrow?
- What is the chance of drawing an Ace from a deck?
- What is the chance of rolling a 6?

---

# Probability

## Simple Definition

Probability is a number that measures how likely an event is to happen.

Probability always lies between:

\[
0
\]

and

\[
1
\]

inclusive.

\[
0 \le P(E) \le 1
\]

where:

```text
E = Event
```

---

# Easy Way to Remember

```text
0 → Impossible
```

```text
1 → Certain
```

Everything else falls between them.

---

# Probability Scale

```text
0 -------------------- 1
Impossible         Certain
```

Examples:

```text
0.1 = Unlikely
0.5 = Equal chance
0.9 = Very likely
```

---

# Different Forms of Probability

Probability can be expressed as:

### Fraction

\[
\frac{1}{2}
\]

---

### Decimal

\[
0.5
\]

---

### Percentage

\[
50\%
\]

---

### Irrational Number

\[
0.707106...
\]

---

### Real Number

Any value between:

\[
0
\]

and

\[
1
\]

---

# Example 1

Fair coin:

\[
P(\text{Head})
=
\frac12
\]

---

# Example 2

Fair die:

\[
P(6)
=
\frac16
\]

---

# Example 3

Drawing an Ace:

\[
P(\text{Ace})
=
\frac4{52}
=
\frac1{13}
\]

---

# Impossible Event

## Simple Definition

An impossible event is something that cannot happen.

Its probability is exactly:

\[
0
\]

---

# Formula

\[
P(\text{Impossible Event})=0
\]

---

# Example 1

Roll a standard die.

Event:

```text
Get a 9
```

Possible outcomes:

```text
1,2,3,4,5,6
```

9 does not exist.

\[
P(9)=0
\]

---

# Example 2

Flip a coin.

Event:

```text
Get both Head and Tail on one side
```

Impossible.

\[
P=0
\]

---

# Example 3

Choose a month.

Event:

```text
Month 13
```

Impossible.

\[
P=0
\]

---

# Example 4

Pick a card.

Event:

```text
A card with 20 hearts
```

Impossible.

\[
P=0
\]

---

# Certain Event

## Simple Definition

A certain event is guaranteed to happen.

Its probability is exactly:

\[
1
\]

---

# Formula

\[
P(\text{Certain Event})=1
\]

---

# Example 1

Roll a die.

Event:

```text
Get a number between 1 and 6
```

Guaranteed.

\[
P=1
\]

---

# Example 2

Pick a card.

Event:

```text
Get either a red or black card
```

Always true.

\[
P=1
\]

---

# Example 3

Choose a month.

Event:

```text
Month has at least 28 days
```

Always true.

\[
P=1
\]

---

# Example 4

Flip a coin.

Event:

```text
Head or Tail
```

Guaranteed.

\[
P=1
\]

---

# Equally Likely Events
## (Unbiased Outcomes)

---

# Simple Definition

Outcomes are equally likely when every outcome has the same chance of occurring.

No outcome is favored.

---

# Easy Way to Remember

```text
Fair System
```

means:

```text
Equal Probability
```

---

# Example 1: Fair Coin

Outcomes:

```text
H
T
```

Probabilities:

\[
P(H)=\frac12
\]

\[
P(T)=\frac12
\]

---

# Example 2: Fair Die

Outcomes:

```text
1,2,3,4,5,6
```

Each outcome:

\[
\frac16
\]

---

# Example 3: Lottery Machine

If every ball is identical:

```text
All numbers equally likely.
```

---

# Example 4: Drawing a Card

Each card in a shuffled deck:

```text
Same probability
```

\[
\frac1{52}
\]

---

# Non-Example

Loaded die:

```text
6 appears more often.
```

Not equally likely.

---

# Theoretical Probability
## (Classical Definition)

---

# Simple Definition

Theoretical probability is calculated using:

\[
P(E)
=
\frac{\text{Number of Favorable Outcomes}}
{\text{Total Number of Outcomes}}
\]

---

# Requirements

Works best when outcomes are:

```text
Equally Likely
```

---

# Example 1

Roll a die.

Event:

```text
Get 4
```

Favorable:

```text
1 outcome
```

Total:

```text
6 outcomes
```

\[
P(4)
=
\frac16
\]

---

# Example 2

Roll a die.

Event:

```text
Even number
```

Favorable:

```text
2,4,6
```

Count:

```text
3
```

Total:

```text
6
```

\[
P(\text{Even})
=
\frac36
=
\frac12
\]

---

# Example 3

Deck of cards.

Event:

```text
Heart
```

Favorable:

```text
13
```

Total:

```text
52
```

\[
P(\text{Heart})
=
\frac{13}{52}
=
\frac14
\]

---

# Mutually Exclusive Events

## Simple Definition

Two events are mutually exclusive if they cannot happen simultaneously.

---

# Easy Way to Remember

```text
Either A or B
```

but

```text
Not Both
```

---

# Addition Rule

If A and B are mutually exclusive:

\[
P(A\text{ or }B)
=
P(A)+P(B)
\]

---

# Example 1

Roll a die.

Event A:

```text
Get 2
```

Event B:

```text
Get 5
```

Cannot happen together.

\[
P(2\text{ or }5)
=
\frac16+\frac16
=
\frac13
\]

---

# Example 2

Pick a card.

A:

```text
King
```

B:

```text
Queen
```

Cannot be both.

\[
P
=
\frac4{52}
+
\frac4{52}
=
\frac8{52}
\]

---

# Example 3

Month:

```text
January
```

or

```text
February
```

Cannot be both.

Mutually exclusive.

---

# Independent Events

## Simple Definition

Two events are independent if one does not affect the other.

---

# Easy Way to Remember

```text
First result changes nothing.
```

---

# Multiplication Rule

\[
P(A\text{ and }B)
=
P(A)\times P(B)
\]

---

# Example 1

Flip a coin twice.

A:

```text
Head on first flip
```

B:

```text
Head on second flip
```

Independent.

\[
\frac12\times\frac12
=
\frac14
\]

---

# Example 2

Roll two dice.

A:

```text
First die = 6
```

B:

```text
Second die = 4
```

Independent.

\[
\frac16\times\frac16
=
\frac1{36}
\]

---

# Example 3

Coin and Die

A:

```text
Head
```

B:

```text
Roll 5
```

Independent.

\[
\frac12\times\frac16
=
\frac1{12}
\]

---

# Dependent Events

## Simple Definition

Two events are dependent if one event changes the probability of the other.

---

# Easy Way to Remember

```text
First event affects second event.
```

---

# Example 1

Bag:

```text
3 Red
2 Blue
```

Pick one ball.

Do not replace it.

---

Event A:

```text
First ball is Red
```

Event B:

```text
Second ball is Red
```

Dependent.

The first draw changes the contents of the bag.

---

# Example 2

Deck of cards.

Draw:

```text
Ace
```

without replacement.

The probability of drawing another Ace changes.

Dependent.

---

# Example 3

Weather

Event A:

```text
Month is December
```

Event B:

```text
Sunny Day
```

The month influences weather patterns.

Dependent.

---

# Sample Space Table
## (Two Dice Experiment)

---

# Simple Definition

A sample space table lists every possible outcome systematically.

---

# Two Dice

First die:

```text
1-6
```

Second die:

```text
1-6
```

Total outcomes:

\[
6\times6
=
36
\]

---

# Probability Grid

| D1\D2 | 1 | 2 | 3 | 4 | 5 | 6 |
|--------|---|---|---|---|---|---|
| 1 | (1,1) | (1,2) | (1,3) | (1,4) | (1,5) | (1,6) |
| 2 | (2,1) | (2,2) | (2,3) | (2,4) | (2,5) | (2,6) |
| 3 | (3,1) | (3,2) | (3,3) | (3,4) | (3,5) | (3,6) |
| 4 | (4,1) | (4,2) | (4,3) | (4,4) | (4,5) | (4,6) |
| 5 | (5,1) | (5,2) | (5,3) | (5,4) | (5,5) | (5,6) |
| 6 | (6,1) | (6,2) | (6,3) | (6,4) | (6,5) | (6,6) |

---

# Example

Sum equals:

```text
7
```

Outcomes:

```text
(1,6)
(2,5)
(3,4)
(4,3)
(5,2)
(6,1)
```

Count:

```text
6
```

Probability:

\[
\frac6{36}
=
\frac16
\]

---

# Complementary Events

## Simple Definition

Every event has an opposite event called its complement.

---

# Formula

\[
P(A)+P(A^c)=1
\]

where:

\[
A^c
\]

means:

```text
Not A
```

---

# Easy Way to Remember

```text
Something happens
OR
It doesn't happen
```

Total probability:

```text
1
```

---

# Example 1

Roll a die.

Event:

```text
Odd number
```

\[
P(\text{Odd})
=
\frac36
=
\frac12
\]

Complement:

```text
Even number
```

\[
P(\text{Even})
=
1-\frac12
=
\frac12
\]

---

# Example 2

Coin

\[
P(H)=\frac12
\]

Complement:

\[
P(T)
=
1-\frac12
=
\frac12
\]

---

# Example 3

Card Deck

Event:

```text
Heart
```

\[
P(\text{Heart})
=
\frac14
\]

Complement:

```text
Not Heart
```

\[
1-\frac14
=
\frac34
\]

---

# Example 4

Roll a die.

Event:

```text
Get 6
```

\[
\frac16
\]

Complement:

```text
Not 6
```

\[
1-\frac16
=
\frac56
\]

---

# Why Complements Are Useful

Sometimes:

```text
At least one success
```

is difficult to count directly.

Instead:

1. Count no successes.
2. Subtract from 1.

This is often easier.

---

# Quick Summary Sheet

## Probability

\[
0 \le P(E) \le 1
\]

Measures likelihood.

---

## Impossible Event

\[
P=0
\]

Cannot happen.

---

## Certain Event

\[
P=1
\]

Guaranteed.

---

## Equally Likely Events

Every outcome has the same probability.

Examples:

```text
Fair coin
Fair die
Shuffled deck
```

---

## Theoretical Probability

\[
P(E)
=
\frac{\text{Favorable}}
{\text{Total}}
\]

---

## Mutually Exclusive Events

Cannot happen together.

\[
P(A\text{ or }B)
=
P(A)+P(B)
\]

---

## Independent Events

One event does not affect another.

\[
P(A\text{ and }B)
=
P(A)P(B)
\]

---

## Dependent Events

One event changes the probability of another.

---

## Sample Space Grid

Two dice:

\[
36
\]

possible outcomes.

---

## Complementary Events

\[
P(A)+P(A^c)=1
\]

or

\[
P(A^c)
=
1-P(A)
\]

---

# Golden Rules

### OR

Think:

```text
Addition
```

---

### AND

Think:

```text
Multiplication
```

---

### Impossible

\[
0
\]

---

### Certain

\[
1
\]

---

### Complement

\[
1-P(A)
\]

---

### Probability Formula

\[
\frac{\text{Successful Outcomes}}
{\text{Total Outcomes}}
\]

This single formula is the foundation of most introductory probability problems.