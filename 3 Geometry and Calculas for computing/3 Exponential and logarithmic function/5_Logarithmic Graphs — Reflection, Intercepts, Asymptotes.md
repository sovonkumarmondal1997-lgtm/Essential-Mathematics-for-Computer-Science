# Logarithmic Graphs — Reflection, Intercepts, Asymptotes, and Real-World Meaning

---

# 1. Graphing via Exponential Reflection

## The Big Idea

A logarithmic function and its corresponding exponential function are inverse functions.

Because they are inverses, their graphs are mirror images of each other across the line:

\[
y=x
\]

This line is often called the **line of symmetry for inverse functions**.

---

# Why Does This Happen?

Suppose:

\[
y=2^x
\]

and

\[
y=\log_2 x
\]

These functions undo each other.

If:

\[
2^3=8
\]

then:

\[
\log_2(8)=3
\]

Notice what happened:

The coordinates changed from

\[
(3,8)
\]

to

\[
(8,3)
\]

The x-coordinate and y-coordinate swap places.

This is exactly what reflection across

\[
y=x
\]

does.

---

# Example 1

Exponential Function:

\[
y=2^x
\]

Contains point:

\[
(2,4)
\]

because:

\[
2^2=4
\]

---

Logarithmic Reflection:

\[
y=\log_2 x
\]

Contains point:

\[
(4,2)
\]

because:

\[
\log_2(4)=2
\]

---

# Example 2

Exponential:

\[
3^2=9
\]

Point:

\[
(2,9)
\]

---

Logarithmic:

\[
\log_3(9)=2
\]

Point:

\[
(9,2)
\]

---

# Example 3

Exponential:

\[
10^3=1000
\]

Point:

\[
(3,1000)
\]

---

Logarithmic:

\[
\log_{10}(1000)=3
\]

Point:

\[
(1000,3)
\]

---

# Visual Analogy

Imagine standing in front of a mirror.

Your left hand appears as your right hand.

Similarly:

\[
(x,y)
\]

becomes

\[
(y,x)
\]

This creates the reflected logarithmic graph.

---

# Key Memory Rule

For inverse functions:

\[
(x,y)
\]

becomes

\[
(y,x)
\]

---

# 2. Universal Reference Points

---

## Point 1: \((1,0)\)

Every logarithmic graph passes through:

\[
(1,0)
\]

because:

\[
\log_a(1)=0
\]

---

# Why?

Remember:

\[
a^0=1
\]

Therefore:

\[
\log_a(1)=0
\]

for every valid base.

---

# Examples

### Base 2

\[
\log_2(1)=0
\]

Point:

\[
(1,0)
\]

---

### Base 3

\[
\log_3(1)=0
\]

Point:

\[
(1,0)
\]

---

### Base 10

\[
\log_{10}(1)=0
\]

Point:

\[
(1,0)
\]

---

# Point 2: \((a,1)\)

Every logarithmic graph passes through:

\[
(a,1)
\]

because:

\[
\log_a(a)=1
\]

---

# Examples

### Base 2

\[
\log_2(2)=1
\]

Point:

\[
(2,1)
\]

---

### Base 3

\[
\log_3(3)=1
\]

Point:

\[
(3,1)
\]

---

### Base 5

\[
\log_5(5)=1
\]

Point:

\[
(5,1)
\]

---

# Quick Summary Table

| Function | Universal Point |
|-----------|-----------|
| \(y=\log_a x\) | (1,0) |
| \(y=\log_a x\) | (a,1) |

---

# Easy Memory Trick

For logarithms:

\[
(1,0)
\]

always comes first.

Then:

\[
(a,1)
\]

---

# 3. The Boundary of Logarithms

---

# Important Rule

You cannot calculate:

\[
\log_a(0)
\]

or

\[
\log_a(\text{negative number})
\]

---

# Why Not?

A logarithm asks:

> "What exponent gives this number?"

---

## Example

Can any power of 2 produce:

\[
-5?
\]

Let's test:

\[
2^1=2
\]

\[
2^2=4
\]

\[
2^3=8
\]

\[
2^{-1}=\frac12
\]

All answers remain positive.

---

Therefore:

\[
\log_2(-5)
\]

does not exist.

---

# What About Zero?

Can any power of 2 equal zero?

\[
2^{-100}
=
\frac1{2^{100}}
\]

Very small.

But not zero.

---

Therefore:

\[
\log_2(0)
\]

does not exist.

---

# Graphical Consequence

The graph only exists for:

\[
x>0
\]

---

# Domain

\[
(0,\infty)
\]

---

# Visual Interpretation

The entire graph stays to the right of the y-axis.

It never crosses:

\[
x=0
\]

---

# Real-Life Analogy

Suppose x represents:

- Population
- Money
- Number of users

You cannot have:

- Negative population
- Negative users
- Exactly zero inside a logarithm model

So logarithms naturally stay in the positive region.

---

# 4. Asymptotes of a Standard Log Graph (\(a>1\))

---

Consider:

\[
y=\log_2 x
\]

---

# What Happens Near Zero?

Take positive values getting closer to zero.

---

## Example

\[
\log_2(1)=0
\]

\[
\log_2(0.5)=-1
\]

\[
\log_2(0.25)=-2
\]

\[
\log_2(0.125)=-3
\]

---

Notice:

The y-values become more negative.

---

As:

\[
x\to0^+
\]

we get:

\[
y\to-\infty
\]

---

# Vertical Asymptote

The graph approaches:

\[
x=0
\]

but never touches it.

---

Thus:

\[
x=0
\]

is a vertical asymptote.

---

# Real-Life Analogy

Imagine walking toward a wall.

You get closer and closer.

But never actually touch it.

The graph behaves similarly near:

\[
x=0
\]

---

# 5. Slow Growth and Algorithmic Complexity

---

# What Happens as \(x\) Gets Large?

For:

\[
y=\log_2 x
\]

the graph rises forever.

But very slowly.

---

# Example Table

| x | \(\log_2 x\) |
|---|---|
| 2 | 1 |
| 4 | 2 |
| 8 | 3 |
| 16 | 4 |
| 32 | 5 |
| 64 | 6 |
| 1024 | 10 |

---

Notice:

To increase y by only 1,

x must double.

---

# Visual Observation

The graph rises.

But it rises extremely slowly.

---

# Real-Life Example: Searching a Phone Book

Suppose a phone book has:

1000 names.

You open near the middle.

Half the book is eliminated.

Open middle again.

Half eliminated again.

This is logarithmic behavior.

---

# Connection to Computer Science

Many efficient algorithms run in:

\[
O(\log n)
\]

time.

---

# Example: Binary Search

Searching:

1 million records.

Instead of checking all records:

\[
1,000,000
\]

checks,

binary search requires only about:

\[
20
\]

checks.

---

Why?

Because:

\[
\log_2(1,000,000)\approx20
\]

---

# Why Programmers Love Logarithms

Because:

\[
O(\log n)
\]

grows very slowly.

---

# Example

| Data Size | Log Steps |
|------------|-----------|
| 1000 | 10 |
| 1,000,000 | 20 |
| 1,000,000,000 | 30 |

Huge data increase.

Tiny work increase.

---

# 6. Behavior of Fractional Log Graphs (\(0<a<1\))

---

Consider:

\[
y=\log_{0.5}x
\]

---

# What Happens Near Zero?

Let's calculate.

---

\[
\log_{0.5}(1)=0
\]

\[
\log_{0.5}(0.5)=1
\]

\[
\log_{0.5}(0.25)=2
\]

\[
\log_{0.5}(0.125)=3
\]

---

Notice:

As x approaches zero,

y becomes larger.

---

Therefore:

\[
x\to0^+
\]

implies

\[
y\to\infty
\]

---

# What Happens for Large x?

---

\[
\log_{0.5}(2)=-1
\]

\[
\log_{0.5}(4)=-2
\]

\[
\log_{0.5}(8)=-3
\]

---

The graph drops downward.

---

Thus:

\[
x\to\infty
\]

implies

\[
y\to-\infty
\]

---

# Comparison with Normal Logarithms

### Standard Log

\[
y=\log_2 x
\]

- Up on the right
- Down near zero

---

### Fractional Log

\[
y=\log_{0.5}x
\]

- Down on the right
- Up near zero

---

The graph is flipped.

---

# Real-Life Example

Suppose a quantity halves every hour.

| Hour | Amount |
|--------|--------|
| 0 | 100 |
| 1 | 50 |
| 2 | 25 |
| 3 | 12.5 |

To find how many hours produced a certain amount, logarithms with base 0.5 naturally appear.

---

# Complete Summary

---

## Reflection Property

\[
y=a^x
\]

and

\[
y=\log_a x
\]

are mirror images across:

\[
y=x
\]

---

## Universal Logarithmic Points

Every logarithmic graph passes through:

\[
(1,0)
\]

and

\[
(a,1)
\]

---

## Logarithm Boundary

Valid inputs:

\[
x>0
\]

Invalid:

\[
x\le0
\]

---

## Standard Logarithms (\(a>1\))

As:

\[
x\to0^+
\]

\[
y\to-\infty
\]

As:

\[
x\to\infty
\]

\[
y\to\infty
\]

slowly.

---

## Fractional Logarithms (\(0<a<1\))

As:

\[
x\to0^+
\]

\[
y\to\infty
\]

As:

\[
x\to\infty
\]

\[
y\to-\infty
\]

---

## Computer Science Connection

Logarithmic growth:

\[
O(\log n)
\]

is extremely efficient because the output grows very slowly even when the input becomes enormous.

---

### One-Sentence Memory Rule

**A logarithmic graph is the mirror image of its exponential partner across \(y=x\), always passes through \((1,0)\), exists only for positive inputs, and grows so slowly that it becomes one of the most important concepts in computer science and algorithm design.**