# Exponential Functions: Symmetry, Reflections, and Reciprocal Bases

---

# 1. Visual-Algebraic Connection

## What Does "Visual-Algebraic Connection" Mean?

In mathematics, every graph has an equation, and every equation creates a graph.

The visual-algebraic connection means:

- The graph (visual picture) shows what the equation is doing.
- The equation (algebra) explains why the graph looks that way.

When you understand both together, mathematics becomes much easier.

---

## Simple Analogy

Think about a car.

### Visual View

You see the car moving faster and faster.

### Algebra View

The speedometer tells you the exact speed.

Both describe the same thing in different ways.

Graphs and equations work the same way.

---

# Example 1: Growth Function

Consider:

\[
y = 2^x
\]

Table:

| x | y |
|---|---|
| 0 | 1 |
| 1 | 2 |
| 2 | 4 |
| 3 | 8 |

---

## Algebra Says

Each increase of 1 in \(x\):

\[
y \times 2
\]

The value doubles.

---

## Graph Says

The curve rises upward faster and faster.

---

### Connection

The graph rises because the algebra keeps multiplying by 2.

---

# Example 2: Decay Function

Consider:

\[
y = \left(\frac12\right)^x
\]

Table:

| x | y |
|---|---|
| 0 | 1 |
| 1 | 1/2 |
| 2 | 1/4 |
| 3 | 1/8 |

---

## Algebra Says

Each step multiplies by:

\[
\frac12
\]

---

## Graph Says

The curve falls toward zero.

---

### Connection

The graph falls because the algebra keeps dividing by 2.

---

# Why Is This Important?

In real-world data:

- Population growth
- Stock prices
- Compound interest
- Radioactive decay
- Machine learning

You often see a graph first.

Understanding the algebra helps explain the graph.

Understanding the graph helps predict future behavior.

---

# Real-Life Example: YouTube Subscribers

Suppose a channel doubles subscribers every month.

| Month | Subscribers |
|---------|---------|
| 0 | 100 |
| 1 | 200 |
| 2 | 400 |
| 3 | 800 |

Equation:

\[
y = 100(2)^x
\]

The graph rises rapidly because the equation doubles repeatedly.

---

# 2. Geometric Symmetry Across the \(y\)-Axis

---

## What Is Symmetry?

Symmetry means one side looks exactly like the mirror image of the other side.

---

## Example

Consider:

\[
y = 2^x
\]

and

\[
y = \left(\frac12\right)^x
\]

---

### Values of \(2^x\)

| x | \(2^x\) |
|---|---|
| -3 | 1/8 |
| -2 | 1/4 |
| -1 | 1/2 |
| 0 | 1 |
| 1 | 2 |
| 2 | 4 |
| 3 | 8 |

---

### Values of \((1/2)^x\)

| x | \((1/2)^x\) |
|---|---|
| -3 | 8 |
| -2 | 4 |
| -1 | 2 |
| 0 | 1 |
| 1 | 1/2 |
| 2 | 1/4 |
| 3 | 1/8 |

---

## Observation

Notice:

| \(2^x\) | \((1/2)^x\) |
|----------|----------|
| 8 | 1/8 |
| 4 | 1/4 |
| 2 | 1/2 |
| 1 | 1 |
| 1/2 | 2 |
| 1/4 | 4 |
| 1/8 | 8 |

The values swap places.

---

## Visual Meaning

The graph of:

\[
y=2^x
\]

rises upward.

The graph of:

\[
y=\left(\frac12\right)^x
\]

falls downward.

They are mirror reflections across:

\[
x=0
\]

which is the y-axis.

---

## Real-Life Mirror Example

Imagine standing in front of a mirror.

Raise your right hand.

The reflection raises its left hand.

Same shape.

Opposite direction.

This is exactly how these two exponential graphs behave.

---

# 3. Function Notation of Reflections

---

## Reflection Rule

Suppose we have two functions:

\[
f_1(x)
\]

and

\[
f_2(x)
\]

If:

\[
f_1(x)=f_2(-x)
\]

then one graph is the reflection of the other across the y-axis.

---

## Why Does Replacing \(x\) With \(-x\) Create Reflection?

Positive values become negative.

Negative values become positive.

Every point moves to the opposite side of the y-axis.

---

# Example

Original function:

\[
f(x)=x^2+1
\]

Replace \(x\) by \(-x\):

\[
f(-x)=(-x)^2+1
\]

\[
=x^2+1
\]

This graph stays the same because it is already symmetric.

---

# Exponential Example

Let:

\[
f_1(x)=\left(\frac12\right)^x
\]

\[
f_2(x)=2^x
\]

Then:

\[
f_1(x)=f_2(-x)
\]

and

\[
f_2(x)=f_1(-x)
\]

Therefore the graphs are reflections.

---

# Easy Memory Trick

Changing:

\[
x
\]

to

\[
-x
\]

means:

"Look in a mirror placed on the y-axis."

---

# 4. Algebraic Proof of the Mirror Identity

---

We want to prove:

\[
f_1(-x)=2^x
\]

where

\[
f_1(x)=\left(\frac12\right)^x
\]

---

## Step 1

Substitute \(-x\) for \(x\):

\[
f_1(-x)
=
\left(\frac12\right)^{-x}
\]

---

## Step 2

Use the negative exponent rule:

\[
a^{-n}
=
\frac1{a^n}
\]

Therefore:

\[
\left(\frac12\right)^{-x}
=
\frac1{\left(\frac12\right)^x}
\]

---

## Step 3

Divide by a fraction

Remember:

\[
\frac1{\frac12}=2
\]

Therefore:

\[
\frac1{\left(\frac12\right)^x}
=
2^x
\]

---

## Final Result

\[
\left(\frac12\right)^{-x}
=
2^x
\]

Proved.

---

# Numerical Proof

Take:

\[
x=3
\]

Left side:

\[
\left(\frac12\right)^{-3}
\]

\[
=8
\]

Right side:

\[
2^3
\]

\[
=8
\]

Both sides are equal.

---

# Another Example

Take:

\[
x=5
\]

Left side:

\[
\left(\frac12\right)^{-5}
\]

\[
=32
\]

Right side:

\[
2^5
\]

\[
=32
\]

Again equal.

---

# Why Does This Create Mirror Graphs?

Because:

\[
f_1(-x)=f_2(x)
\]

Every point on one graph appears at the reflected location on the other graph.

---

# 5. Universal Rule of Reciprocal Bases

---

## The Rule

For any positive base \(a\):

\[
\left(\frac1a\right)^{-x}
=
a^x
\]

---

## Meaning

Two things happen:

### Step 1

Negative exponent flips the expression.

### Step 2

Reciprocal base flips again.

The two flips cancel each other.

Result:

\[
a^x
\]

---

# Example 1

\[
\left(\frac13\right)^{-2}
\]

Using the rule:

\[
=3^2
\]

\[
=9
\]

---

# Example 2

\[
\left(\frac15\right)^{-3}
\]

Using the rule:

\[
=5^3
\]

\[
=125
\]

---

# Example 3

\[
\left(\frac1{10}\right)^{-4}
\]

Using the rule:

\[
=10^4
\]

\[
=10000
\]

---

# Example 4

\[
\left(\frac14\right)^{-5}
\]

Using the rule:

\[
=4^5
\]

\[
=1024
\]

---

# Real-Life Analogy

Imagine a light switch.

### First Flip

Turns OFF.

### Second Flip

Turns ON again.

Two flips return to the original state.

Similarly:

- Reciprocal flips once.
- Negative exponent flips again.

Result:

\[
a^x
\]

---

# Connection to Graph Reflections

Growth Function:

\[
y=a^x
\]

Decay Function:

\[
y=\left(\frac1a\right)^x
\]

These two graphs are mirror images because:

\[
\left(\frac1a\right)^{-x}=a^x
\]

---

# Complete Summary

## Visual-Algebraic Connection

- Equations explain graphs.
- Graphs visualize equations.
- Understanding both improves mathematical modeling.

---

## Symmetry Across the Y-Axis

\[
2^x
\]

and

\[
\left(\frac12\right)^x
\]

are mirror images across:

\[
x=0
\]

---

## Reflection Rule

If:

\[
f_1(x)=f_2(-x)
\]

then the graphs are reflections across the y-axis.

---

## Mirror Identity

\[
\left(\frac12\right)^{-x}
=
2^x
\]

This proves the reflection algebraically.

---

## Universal Reciprocal Rule

\[
\left(\frac1a\right)^{-x}
=
a^x
\]

for every positive base \(a\).

---

## One-Sentence Memory Rule

**A growth curve \(a^x\) and its decay curve \((1/a)^x\) are mirror images across the y-axis because replacing \(x\) with \(-x\) converts one function into the other through the rule \((1/a)^{-x}=a^x\).**