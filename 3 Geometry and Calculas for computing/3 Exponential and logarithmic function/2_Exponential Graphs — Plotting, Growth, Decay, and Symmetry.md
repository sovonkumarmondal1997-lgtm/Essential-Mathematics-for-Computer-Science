# Exponential Graphs — Plotting, Growth, Decay, and Symmetry

---

# 1. Plotting Exponential Graphs by Point Testing

## What is Point Testing?

Point testing means:

1. Choose values of \(x\)
2. Substitute them into the function
3. Calculate \(y\)
4. Plot the resulting points
5. Join the points smoothly

This is one of the easiest ways to draw exponential graphs.

---

# Example 1: Graph of \(y = 2^x\)

Let's calculate values from \(x=-3\) to \(x=3\).

| x | \(y=2^x\) |
|---|---|
| -3 | \(1/8\) |
| -2 | \(1/4\) |
| -1 | \(1/2\) |
| 0 | 1 |
| 1 | 2 |
| 2 | 4 |
| 3 | 8 |

---

## How Were Negative Powers Calculated?

Remember:

\[
a^{-n}=\frac{1}{a^n}
\]

Example:

\[
2^{-3}
=
\frac{1}{2^3}
=
\frac{1}{8}
\]

---

## Observing the Pattern

Moving right:

\[
1 \rightarrow 2 \rightarrow 4 \rightarrow 8
\]

The values double each step.

Moving left:

\[
1 \rightarrow \frac12 \rightarrow \frac14 \rightarrow \frac18
\]

The values become smaller and approach zero.

---

# Example 2: Graph of \(y = 3^x\)

| x | \(y=3^x\) |
|---|---|
| -3 | \(1/27\) |
| -2 | \(1/9\) |
| -1 | \(1/3\) |
| 0 | 1 |
| 1 | 3 |
| 2 | 9 |
| 3 | 27 |

---

## Observing the Pattern

Positive side:

\[
1 \rightarrow 3 \rightarrow 9 \rightarrow 27
\]

Growth is much faster than \(2^x\).

Negative side:

\[
1 \rightarrow \frac13 \rightarrow \frac19 \rightarrow \frac1{27}
\]

Values shrink faster toward zero.

---

# Example 3: Graph of \(y=\left(\frac12\right)^x\)

| x | \(y=(1/2)^x\) |
|---|---|
| -3 | 8 |
| -2 | 4 |
| -1 | 2 |
| 0 | 1 |
| 1 | \(1/2\) |
| 2 | \(1/4\) |
| 3 | \(1/8\) |

---

## Why Do Negative Values Become Large?

Example:

\[
\left(\frac12\right)^{-3}
=
\frac1{(1/2)^3}
=
\frac1{1/8}
=
8
\]

Negative exponents flip fractions upside down.

---

## Observing the Pattern

Moving right:

\[
1,\frac12,\frac14,\frac18
\]

Graph decreases.

Moving left:

\[
1,2,4,8
\]

Graph increases.

This is called exponential decay.

---

# Quick Comparison

| x | \(2^x\) | \(3^x\) | \((1/2)^x\) |
|---|---|---|---|
| -3 | 1/8 | 1/27 | 8 |
| -2 | 1/4 | 1/9 | 4 |
| -1 | 1/2 | 1/3 | 2 |
| 0 | 1 | 1 | 1 |
| 1 | 2 | 3 | 1/2 |
| 2 | 4 | 9 | 1/4 |
| 3 | 8 | 27 | 1/8 |

---

# 2. Universal Points Shared by All Exponential Graphs

No matter what positive base is used, every exponential graph shares two important points.

---

# Universal Point 1: The Y-Intercept

Set:

\[
x=0
\]

Then:

\[
y=a^0
\]

Since:

\[
a^0=1
\]

Every exponential graph passes through:

\[
(0,1)
\]

---

## Examples

### \(y=2^x\)

\[
2^0=1
\]

Point:

\[
(0,1)
\]

---

### \(y=3^x\)

\[
3^0=1
\]

Point:

\[
(0,1)
\]

---

### \(y=0.5^x\)

\[
(0.5)^0=1
\]

Point:

\[
(0,1)
\]

---

# Universal Point 2: The Point \((1,a)\)

Set:

\[
x=1
\]

Then:

\[
y=a^1=a
\]

Therefore:

\[
(1,a)
\]

---

## Examples

### \(y=2^x\)

\[
(1,2)
\]

---

### \(y=3^x\)

\[
(1,3)
\]

---

### \(y=5^x\)

\[
(1,5)
\]

---

### \(y=0.5^x\)

\[
(1,0.5)
\]

---

# Easy Memory Trick

Every exponential graph always passes through:

\[
(0,1)
\]

and

\[
(1,a)
\]

---

# 3. Behavior of Growth Curves (Base \(a>1\))

Examples:

\[
y=2^x
\]

\[
y=3^x
\]

\[
y=5^x
\]

These are called exponential growth functions.

---

# What Happens When \(x\) Gets Very Large?

Example:

\[
y=2^x
\]

| x | y |
|---|---|
| 5 | 32 |
| 10 | 1024 |
| 20 | 1,048,576 |

The graph rises extremely fast.

---

Mathematically:

\[
x\to\infty
\]

implies

\[
y\to\infty
\]

---

# What Happens When \(x\) Becomes Very Negative?

Example:

\[
2^{-5}
=
\frac1{32}
\]

\[
2^{-10}
=
\frac1{1024}
\]

\[
2^{-20}
=
\frac1{1048576}
\]

The values become extremely small.

---

Mathematically:

\[
x\to-\infty
\]

implies

\[
y\to0
\]

---

# Horizontal Asymptote

The graph gets closer and closer to zero.

But it never touches zero.

The line:

\[
y=0
\]

is called a horizontal asymptote.

---

# Real-Life Example: Population Growth

A bacteria colony doubles every hour.

| Hour | Population |
|---|---|
| 0 | 100 |
| 1 | 200 |
| 2 | 400 |
| 3 | 800 |
| 4 | 1600 |

Growth becomes explosive.

---

# 4. The Impact of a Larger Base

Compare:

\[
y=2^x
\]

\[
y=3^x
\]

\[
y=5^x
\]

---

# At \(x=3\)

\[
2^3=8
\]

\[
3^3=27
\]

\[
5^3=125
\]

---

## Observation

Larger base = faster growth.

---

# At \(x=-3\)

\[
2^{-3}
=
\frac18
\]

\[
3^{-3}
=
\frac1{27}
\]

\[
5^{-3}
=
\frac1{125}
\]

---

## Observation

Larger base approaches zero much faster.

---

# Visual Understanding

Think of three rockets.

- Rocket 2 rises steadily.
- Rocket 3 rises faster.
- Rocket 5 shoots upward dramatically.

Larger base = steeper graph.

---

# Real-Life Example

Imagine investments:

### Plan A

Money doubles each year.

\[
2^x
\]

---

### Plan B

Money triples each year.

\[
3^x
\]

---

### Plan C

Money becomes five times larger each year.

\[
5^x
\]

Plan C grows much faster.

---

# 5. Behavior of Decay Curves (\(0<a<1\))

Examples:

\[
y=(1/2)^x
\]

\[
y=(1/3)^x
\]

\[
y=(0.8)^x
\]

These are called exponential decay functions.

---

# What Happens When \(x\) Gets Larger?

Example:

\[
(1/2)^1=\frac12
\]

\[
(1/2)^2=\frac14
\]

\[
(1/2)^3=\frac18
\]

\[
(1/2)^{10}=\frac1{1024}
\]

Values move toward zero.

---

Mathematically:

\[
x\to\infty
\]

implies

\[
y\to0
\]

---

# What Happens When \(x\) Becomes Very Negative?

Example:

\[
(1/2)^{-1}=2
\]

\[
(1/2)^{-2}=4
\]

\[
(1/2)^{-3}=8
\]

\[
(1/2)^{-10}=1024
\]

Values become huge.

---

Mathematically:

\[
x\to-\infty
\]

implies

\[
y\to\infty
\]

---

# Real-Life Example: Medicine in the Body

Suppose a medicine loses half its amount every hour.

| Hour | Amount |
|---|---|
| 0 | 100 mg |
| 1 | 50 mg |
| 2 | 25 mg |
| 3 | 12.5 mg |

This follows:

\[
100\left(\frac12\right)^x
\]

This is exponential decay.

---

# 6. Graphical Symmetry and Reflection

One of the most beautiful properties of exponential graphs is symmetry.

---

# Compare These Functions

\[
y=2^x
\]

and

\[
y=(1/2)^x
\]

---

Notice:

\[
(1/2)^x
=
2^{-x}
\]

---

# Test Values

| x | \(2^x\) | \((1/2)^x\) |
|---|---|---|
| -3 | 1/8 | 8 |
| -2 | 1/4 | 4 |
| -1 | 1/2 | 2 |
| 0 | 1 | 1 |
| 1 | 2 | 1/2 |
| 2 | 4 | 1/4 |
| 3 | 8 | 1/8 |

---

# What Do You Notice?

The values swap positions.

For example:

\[
2^3=8
\]

and

\[
(1/2)^{-3}=8
\]

---

# Mirror Reflection

The graph of:

\[
y=(1/2)^x
\]

is the mirror image of:

\[
y=2^x
\]

across the y-axis.

---

# Why?

Replacing \(x\) by \(-x\) reflects a graph across the y-axis.

Since:

\[
(1/2)^x=2^{-x}
\]

the two graphs are reflections.

---

# Real-Life Analogy

Imagine looking at a mountain in a mirror.

One side rises.

The reflected side falls.

The two shapes are identical but reversed.

That is exactly what happens with:

\[
2^x
\]

and

\[
(1/2)^x
\]

---

# Final Summary

## Growth Curves (\(a>1\))

Examples:

\[
2^x,\;3^x,\;5^x
\]

Properties:

- Rise to infinity on the right
- Approach zero on the left
- Larger base = steeper graph

---

## Decay Curves (\(0<a<1\))

Examples:

\[
(1/2)^x,\;(1/3)^x
\]

Properties:

- Approach zero on the right
- Rise to infinity on the left

---

## Universal Points

Every exponential graph passes through:

\[
(0,1)
\]

and

\[
(1,a)
\]

---

## Horizontal Asymptote

Every standard exponential graph approaches:

\[
y=0
\]

but never touches it.

---

## Reflection Property

\[
(1/2)^x=2^{-x}
\]

Therefore:

- \(2^x\) and \((1/2)^x\) are mirror images.
- Reflection occurs across the y-axis.

---

### One-Sentence Memory Rule

**If the base is greater than 1, the graph grows; if the base is between 0 and 1, the graph decays; and every exponential graph always passes through (0,1) while approaching the horizontal asymptote \(y=0\).**