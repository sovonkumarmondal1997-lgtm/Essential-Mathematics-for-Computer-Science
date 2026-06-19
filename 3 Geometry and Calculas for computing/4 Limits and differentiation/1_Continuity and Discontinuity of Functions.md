# Continuity and Discontinuity of Functions — Simple Notes with Examples

---

# Introduction

Before learning differentiation, one of the most important ideas in calculus is **continuity**.

Why?

Because differentiation studies how a function changes at a point, and this only makes sense when the graph behaves properly around that point.

Think of continuity as checking whether a road is smooth enough before measuring the speed of a car traveling on it.

---

# 1. The Requirement for Differentiation

## What Is Differentiation?

Differentiation measures:

- Rate of change
- Slope of a curve
- Instantaneous speed
- Gradient of a graph

---

## Why Does Continuity Matter?

To calculate a slope at a point, the graph must actually exist around that point.

If the graph suddenly breaks, jumps, or disappears, there is no smooth curve to measure.

---

## Road Analogy

Imagine driving a car.

### Continuous Road

```
-------------------
```

You can measure speed anywhere.

---

### Broken Road

```
-------     -------
```

At the gap, speed becomes meaningless because the road does not exist.

---

The same idea applies to differentiation.

---

# Example 1: Continuous Curve

\[
y=x^2
\]

The graph is smooth everywhere.

Therefore:

- Continuous everywhere
- Differentiable everywhere

---

# Example 2: Broken Curve

\[
y=\frac1x
\]

At:

\[
x=0
\]

the graph breaks.

Differentiation is impossible there.

---

# Easy Memory Rule

**No continuous curve → No derivative at that point.**

---

# 2. Geometric Concept of Continuity

---

## What Does Continuous Mean Visually?

A graph is continuous if you can draw it without lifting your pencil from the paper.

---

## Characteristics

A continuous graph has:

- No gaps
- No holes
- No breaks
- No sudden jumps

---

# Example 1

\[
y=x
\]

Straight line.

You can draw it in one motion.

Continuous.

---

# Example 2

\[
y=x^2
\]

Smooth parabola.

Continuous.

---

# Example 3

\[
y=\sin x
\]

Smooth wave.

Continuous.

---

# Example of a Non-Continuous Graph

```
----     ----
```

Gap in the graph.

Not continuous.

---

# Real-Life Analogy

Imagine a railway track.

### Continuous Track

Train moves smoothly.

---

### Broken Track

Train cannot continue.

The track is discontinuous.

---

# Easy Memory Rule

Continuous means:

**"No pencil lifting."**

---

# 3. Algebraic Definition of Continuity

---

Visual intuition is useful, but mathematics needs a precise definition.

---

# Definition

A function is continuous at a point \(x=a\) if:

\[
\lim_{x\to a^-}f(x)
=
\lim_{x\to a^+}f(x)
=
f(a)
\]

---

This means:

1. Left-hand limit exists
2. Right-hand limit exists
3. Both are equal
4. They equal the actual function value

---

# Example

Consider:

\[
f(x)=x^2
\]

Check continuity at:

\[
x=2
\]

---

From the left:

\[
\lim_{x\to2^-}x^2=4
\]

---

From the right:

\[
\lim_{x\to2^+}x^2=4
\]

---

Actual value:

\[
f(2)=4
\]

---

All are equal.

Therefore:

\[
f(x)
\]

is continuous at \(x=2\).

---

# Real-Life Analogy

Imagine two roads approaching a bridge.

If both roads meet perfectly at the bridge, traffic flows smoothly.

If they don't meet, there is a discontinuity.

---

# Easy Memory Rule

Continuity means:

Left = Right = Function Value

---

# 4. Example of a Continuous Function

---

Consider:

\[
y=x^2
\]

---

Check near:

\[
x=2
\]

---

Values from the left:

| x | y |
|---|---|
|1.9|3.61|
|1.99|3.9601|
|1.999|3.996001|

Approaching:

\[
4
\]

---

Values from the right:

| x | y |
|---|---|
|2.1|4.41|
|2.01|4.0401|
|2.001|4.004001|

Approaching:

\[
4
\]

---

Function value:

\[
f(2)=4
\]

---

Therefore:

\[
\lim_{x\to2^-}x^2
=
\lim_{x\to2^+}x^2
=
4
\]

Continuous.

---

# More Continuous Examples

---

## Example

\[
y=x^3
\]

Continuous everywhere.

---

## Example

\[
y=e^x
\]

Continuous everywhere.

---

## Example

\[
y=\sin x
\]

Continuous everywhere.

---

# Easy Memory Rule

Most standard curves are continuous unless a denominator, logarithm, or piecewise rule creates a problem.

---

# 5. Essential Discontinuity via \(1/x\)

---

Consider:

\[
y=\frac1x
\]

---

# What Happens Near Zero?

---

Approach from the right:

\[
x=0.1
\]

\[
y=10
\]

---

\[
x=0.01
\]

\[
y=100
\]

---

\[
x=0.001
\]

\[
y=1000
\]

---

Thus:

\[
x\to0^+
\]

gives:

\[
y\to+\infty
\]

---

Approach from the left:

\[
x=-0.1
\]

\[
y=-10
\]

---

\[
x=-0.01
\]

\[
y=-100
\]

---

\[
x=-0.001
\]

\[
y=-1000
\]

---

Thus:

\[
x\to0^-
\]

gives:

\[
y\to-\infty
\]

---

# Problem

Left side:

\[
-\infty
\]

Right side:

\[
+\infty
\]

Not equal.

---

Therefore:

\[
\lim_{x\to0}\frac1x
\]

does not exist.

---

This is called an **essential discontinuity**.

---

# Visual Picture

```
    |
   /
  /
 |
 |
 |
  \
   \
    |
```

The graph splits into two separate branches.

---

# 6. Essential Discontinuity via \(\tan x\)

---

Consider:

\[
y=\tan x
\]

---

Remember:

\[
\tan x
=
\frac{\sin x}{\cos x}
\]

---

At:

\[
x=\frac{\pi}{2}
\]

we have:

\[
\cos\left(\frac{\pi}{2}\right)=0
\]

Division by zero occurs.

---

# Approaching From the Left

\[
\tan x
\to+\infty
\]

---

# Approaching From the Right

\[
\tan x
\to-\infty
\]

---

The graph shoots in opposite directions.

---

Therefore:

\[
x=\frac{\pi}{2}
\]

is an essential discontinuity.

---

# Real-Life Analogy

Imagine an elevator.

One side shoots upward forever.

The other side shoots downward forever.

They never meet.

---

# 7. Jump Discontinuity

---

## What Is a Jump?

A jump discontinuity occurs when the graph suddenly jumps from one value to another.

---

# Example

Define:

\[
f(x)=
\begin{cases}
1 & x<0\\
5 & x\ge0
\end{cases}
\]

---

Approaching from left:

\[
1
\]

Approaching from right:

\[
5
\]

---

The graph looks like:

```
5 ────────●
|
|
|
1 ●────────
```

---

The graph instantly jumps.

---

Since:

\[
1 \ne 5
\]

the limits are different.

Therefore discontinuous.

---

# Real-Life Example

Imagine a staircase.

You move smoothly.

Suddenly:

Step up.

That sudden jump is a jump discontinuity.

---

# More Examples

### Tax Brackets

Income ₹49,999

Tax = 5%

Income ₹50,000

Tax = 10%

Sudden jump.

---

### Shipping Charges

Below 5 kg:

₹100

Above 5 kg:

₹300

Instant jump.

---

# 8. Removable Singularity

---

## What Is It?

A removable singularity is a tiny hole in an otherwise perfect graph.

The graph is almost continuous.

Only one point is missing or misplaced.

---

# Example

Consider:

\[
f(x)=\frac{x^2-4}{x-2}
\]

---

Factor:

\[
=
\frac{(x-2)(x+2)}{x-2}
\]

---

Cancel:

\[
=x+2
\]

---

But:

\[
x=2
\]

is not allowed in the original formula.

---

# What Happens?

The graph behaves exactly like:

\[
y=x+2
\]

except one point is missing.

---

The missing point would be:

\[
(2,4)
\]

---

Graph:

```
      ○
-----/-----
```

Small hole.

---

# Why Is It Called Removable?

Simply define:

\[
f(2)=4
\]

The hole disappears.

Continuity is restored.

---

# Real-Life Analogy

Imagine a perfectly smooth road with one missing brick.

Replace the brick.

Problem solved.

---

# Another Example

\[
f(x)=\frac{x^2-1}{x-1}
\]

---

Simplify:

\[
=x+1
\]

except at:

\[
x=1
\]

---

Hole occurs at:

\[
(1,2)
\]

---

Again, a removable singularity.

---

# Complete Summary

---

## Continuity Requirement

A function must be continuous at a point before differentiation can be meaningfully performed there.

---

## Geometric Continuity

Continuous graph:

- No breaks
- No holes
- No jumps

Draw without lifting your pencil.

---

## Algebraic Continuity

A function is continuous when:

\[
\lim_{x\to a^-}f(x)
=
\lim_{x\to a^+}f(x)
=
f(a)
\]

---

## Continuous Example

\[
y=x^2
\]

Continuous everywhere.

---

## Essential Discontinuity

Examples:

\[
y=\frac1x
\]

at \(x=0\)

and

\[
y=\tan x
\]

at \(x=\frac{\pi}{2}\)

---

## Jump Discontinuity

Graph suddenly leaps from one value to another.

Example:

Piecewise functions.

---

## Removable Singularity

Graph is perfect except for one missing point.

Example:

\[
\frac{x^2-4}{x-2}
\]

has a hole at:

\[
(2,4)
\]

---

## Types of Discontinuities

| Type | Description |
|--------|--------|
| Essential | Infinite break |
| Jump | Sudden leap |
| Removable | Missing point |

---

### One-Sentence Memory Rule

**A function is continuous when the left side, right side, and actual function value all meet perfectly; if they fail to meet because of infinity, jumps, or holes, the function becomes discontinuous.**