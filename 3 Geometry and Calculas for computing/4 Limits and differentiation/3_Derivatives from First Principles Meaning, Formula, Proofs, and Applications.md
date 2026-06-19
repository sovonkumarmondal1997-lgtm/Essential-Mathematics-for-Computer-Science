# Derivatives from First Principles — Meaning, Formula, Proofs, and Applications

---

# Introduction

One of the most important ideas in calculus is the **derivative**.

A derivative tells us:

- How fast something changes.
- The steepness of a graph.
- The gradient of a curve.
- Instantaneous speed.

The derivative is the mathematical tool that allows us to measure change at an exact point.

---

# 1. Core Purpose of a Derivative

## What Does a Function Tell Us?

A normal function:

\[
f(x)
\]

tells us the height of a graph.

---

## Example

Consider:

\[
f(x)=x^2
\]

If:

\[
x=3
\]

then:

\[
f(3)=9
\]

The function tells us:

> The point is located at height 9.

---

# What Does the Derivative Tell Us?

The derivative:

\[
f'(x)
\]

does not tell us the height.

Instead, it tells us:

> How steep the graph is at that point.

---

# Example

For:

\[
f(x)=x^2
\]

the derivative is:

\[
f'(x)=2x
\]

At:

\[
x=3
\]

the slope is:

\[
f'(3)=6
\]

---

# Comparison

| Question | Function | Derivative |
|-----------|-----------|-----------|
| Height? | Yes | No |
| Slope? | No | Yes |
| Position? | Yes | No |
| Rate of Change? | No | Yes |

---

# Real-Life Example: Driving a Car

Suppose:

\[
f(t)
\]

represents distance traveled.

---

The function tells you:

> Where the car is.

---

The derivative tells you:

> How fast the car is moving.

---

Example:

Distance:

\[
100\ km
\]

Speed:

\[
80\ km/h
\]

The function gives position.

The derivative gives speed.

---

# Easy Memory Rule

**A function tells you where you are. A derivative tells you how fast you are changing.**

---

# 2. Geometric Basis of First Principles

---

# Starting with a Straight Line

The slope of a straight line is:

\[
\text{Slope}
=
\frac{\Delta y}{\Delta x}
\]

which means:

\[
\frac{\text{Vertical Change}}{\text{Horizontal Change}}
\]

---

# Example

Points:

\[
(2,3)
\]

and

\[
(4,7)
\]

---

Vertical change:

\[
\Delta y=7-3=4
\]

---

Horizontal change:

\[
\Delta x=4-2=2
\]

---

Slope:

\[
\frac{\Delta y}{\Delta x}
=
\frac4 2
=
2
\]

---

# Problem with Curves

For a curve, the slope keeps changing.

---

Example:

\[
y=x^2
\]

At different points:

| x | Slope |
|---|---|
|1|2|
|2|4|
|3|6|

---

We need the slope at one exact point.

---

# Solution

Take two points:

- Point A
- Point B

Move Point B closer and closer to Point A.

---

Eventually:

\[
\Delta x
\rightarrow 0
\]

---

The average slope becomes the exact slope.

---

This idea creates the derivative.

---

# Real-Life Analogy

Imagine measuring the speed of a car.

---

Average speed over 1 hour:

\[
\frac{\text{Distance}}{\text{Time}}
\]

---

Average speed over 1 minute:

More accurate.

---

Average speed over 1 second:

Even more accurate.

---

Average speed over an infinitely tiny time interval:

Instantaneous speed.

This is exactly what derivatives do.

---

# Easy Memory Rule

**Derivative = Average slope with points squeezed infinitely close together.**

---

# 3. The Limit Definition Formula

---

# Official Definition

The derivative from first principles is:

\[
f'(x)
=
\lim_{\Delta x\to0}
\frac{
f(x+\Delta x)-f(x)
}
{\Delta x}
\]

---

# What Does Each Part Mean?

---

## \(\Delta x\)

Tiny movement in x.

---

## \(f(x+\Delta x)\)

New height after moving slightly.

---

## \(f(x)\)

Original height.

---

## Numerator

\[
f(x+\Delta x)-f(x)
\]

Change in height.

---

## Denominator

\[
\Delta x
\]

Change in position.

---

Thus:

\[
\frac{\Delta y}{\Delta x}
\]

which is slope.

---

## Limit

\[
\Delta x\to0
\]

Move the points infinitely close together.

---

# Simple Interpretation

The derivative equals:

\[
\text{Instantaneous Slope}
=
\lim
\left(
\text{Average Slope}
\right)
\]

---

# Easy Memory Rule

**Derivative = Tiny change in y divided by tiny change in x.**

---

# 4. Proof for \(f(x)=x^2\)

---

We will use the first-principles formula.

---

# Step 1

Start with:

\[
f(x)=x^2
\]

---

Substitute into formula:

\[
f'(x)
=
\lim_{\Delta x\to0}
\frac{
(x+\Delta x)^2-x^2
}
{\Delta x}
\]

---

# Step 2

Expand using the binomial theorem

\[
(x+\Delta x)^2
=
x^2
+
2x\Delta x
+
(\Delta x)^2
\]

---

Substitute:

\[
=
\lim_{\Delta x\to0}
\frac{
x^2
+
2x\Delta x
+
(\Delta x)^2
-
x^2
}
{\Delta x}
\]

---

# Step 3

Cancel \(x^2\)

\[
=
\lim_{\Delta x\to0}
\frac{
2x\Delta x
+
(\Delta x)^2
}
{\Delta x}
\]

---

# Step 4

Factor out \(\Delta x\)

\[
=
\lim_{\Delta x\to0}
\frac{
\Delta x(2x+\Delta x)
}
{\Delta x}
\]

---

Cancel:

\[
=
\lim_{\Delta x\to0}
(2x+\Delta x)
\]

---

# Step 5

Apply the limit

\[
\Delta x\to0
\]

---

Result:

\[
f'(x)=2x
\]

---

# Final Answer

\[
\boxed{
\frac{d}{dx}(x^2)=2x
}
\]

---

# Numerical Verification

At:

\[
x=3
\]

Derivative:

\[
2(3)=6
\]

Slope equals 6.

---

# 5. Practical Application of a Derivative

---

# Example

Consider:

\[
y=x^2
\]

Derivative:

\[
y'=2x
\]

---

Find slope at:

\[
(3,9)
\]

---

Substitute:

\[
x=3
\]

---

\[
y'=2(3)
\]

---

\[
=6
\]

---

Therefore:

The tangent line at:

\[
(3,9)
\]

has slope:

\[
6
\]

---

# Another Example

At:

\[
x=5
\]

---

\[
y'=2(5)
\]

---

\[
=10
\]

---

The graph is steeper.

---

# Real-Life Example

Suppose:

\[
s(t)=t^2
\]

represents distance traveled.

Derivative:

\[
v(t)=2t
\]

represents velocity.

---

At:

\[
t=3
\]

velocity:

\[
6
\]

units/sec.

---

At:

\[
t=10
\]

velocity:

\[
20
\]

units/sec.

---

The derivative tells us the exact speed at a particular instant.

---

# Easy Memory Rule

**Plug a value into the derivative to find the slope at that point.**

---

# 6. Proof for \(f(x)=x^3\)

---

Start with:

\[
f(x)=x^3
\]

---

# Step 1

Apply first principles:

\[
f'(x)
=
\lim_{\Delta x\to0}
\frac{
(x+\Delta x)^3-x^3
}
{\Delta x}
\]

---

# Step 2

Expand using:

\[
(a+b)^3
=
a^3+3a^2b+3ab^2+b^3
\]

---

Thus:

\[
(x+\Delta x)^3
=
x^3
+
3x^2\Delta x
+
3x(\Delta x)^2
+
(\Delta x)^3
\]

---

Substitute:

\[
=
\lim_{\Delta x\to0}
\frac{
x^3
+
3x^2\Delta x
+
3x(\Delta x)^2
+
(\Delta x)^3
-
x^3
}
{\Delta x}
\]

---

# Step 3

Cancel \(x^3\)

\[
=
\lim_{\Delta x\to0}
\frac{
3x^2\Delta x
+
3x(\Delta x)^2
+
(\Delta x)^3
}
{\Delta x}
\]

---

# Step 4

Factor out \(\Delta x\)

\[
=
\lim_{\Delta x\to0}
\frac{
\Delta x
\left(
3x^2
+
3x\Delta x
+
(\Delta x)^2
\right)
}
{\Delta x}
\]

---

Cancel:

\[
=
\lim_{\Delta x\to0}
\left(
3x^2
+
3x\Delta x
+
(\Delta x)^2
\right)
\]

---

# Step 5

Apply limit

\[
\Delta x\to0
\]

---

Terms disappear:

\[
3x\Delta x\to0
\]

\[
(\Delta x)^2\to0
\]

---

Result:

\[
f'(x)=3x^2
\]

---

# Final Answer

\[
\boxed{
\frac{d}{dx}(x^3)=3x^2
}
\]

---

# Numerical Example

At:

\[
x=2
\]

---

Slope:

\[
3(2)^2
\]

---

\[
=12
\]

---

At:

\[
x=4
\]

---

Slope:

\[
3(4)^2
\]

---

\[
=48
\]

---

Notice how rapidly the slope increases.

---

# Complete Summary

---

## Function vs Derivative

Function:

\[
f(x)
\]

gives height.

Derivative:

\[
f'(x)
\]

gives slope.

---

## First Principles Formula

\[
f'(x)
=
\lim_{\Delta x\to0}
\frac{
f(x+\Delta x)-f(x)
}
{\Delta x}
\]

---

## Derivative of \(x^2\)

\[
\boxed{
\frac{d}{dx}(x^2)=2x
}
\]

---

## Derivative of \(x^3\)

\[
\boxed{
\frac{d}{dx}(x^3)=3x^2
}
\]

---

## Practical Meaning

Evaluate the derivative at a point to find the exact slope of the graph at that location.

---

## Real-World Meaning

If a function represents position, its derivative represents speed.

If a function represents profit, its derivative represents profit growth.

If a function represents population, its derivative represents population growth rate.

---

### One-Sentence Memory Rule

**A derivative measures the exact slope of a curve at a point by taking the limit of average slopes as two points move infinitely close together, leading to results such as \(\frac{d}{dx}(x^2)=2x\) and \(\frac{d}{dx}(x^3)=3x^2\).**