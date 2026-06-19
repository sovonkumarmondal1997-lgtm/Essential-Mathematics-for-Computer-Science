# Local Maxima, Local Minima, Points of Inflection, and Graph Sketching

---

# Introduction

One of the most powerful applications of differentiation is finding important points on a graph:

- Peaks (Local Maximums)
- Valleys (Local Minimums)
- Flat Points (Points of Inflection)
- Turning Points

These points help us understand the overall shape of a graph without plotting hundreds of coordinates.

The key idea is:

> Turning points occur where the derivative equals zero.

In symbols:

\[
f'(x)=0
\]

These points are called **stationary points**.

---

# 1. Definition of a Local Maximum

---

## What Is a Local Maximum?

A local maximum is a point where the graph reaches a peak before starting to decrease.

---

## Gradient Behavior

Before the peak:

\[
f'(x)>0
\]

The graph is rising.

---

At the peak:

\[
f'(x)=0
\]

The graph becomes flat.

---

After the peak:

\[
f'(x)<0
\]

The graph falls.

---

Pattern:

\[
(+)\rightarrow 0 \rightarrow (-)
\]

---

# Visual Picture

```text
        ▲
       / \
      /   \
-----/-----\-----
```

---

The top point is a local maximum.

---

# Example 1

Consider:

\[
f(x)=-x^2+4
\]

Derivative:

\[
f'(x)=-2x
\]

---

Set derivative equal to zero:

\[
-2x=0
\]

\[
x=0
\]

---

Function value:

\[
f(0)=4
\]

Maximum point:

\[
(0,4)
\]

---

# Example 2

Imagine throwing a ball upward.

The ball rises.

Its velocity becomes zero.

Then it falls.

The highest point is a local maximum.

---

# Real-Life Example

Mountain peak.

You walk uphill.

Reach the summit.

Then walk downhill.

The summit is a local maximum.

---

# Easy Memory Rule

**Maximum = Up → Flat → Down**

---

# 2. Definition of a Local Minimum

---

## What Is a Local Minimum?

A local minimum is a point where the graph reaches a valley before starting to rise.

---

## Gradient Behavior

Before the valley:

\[
f'(x)<0
\]

Graph falls.

---

At the valley:

\[
f'(x)=0
\]

Graph becomes flat.

---

After the valley:

\[
f'(x)>0
\]

Graph rises.

---

Pattern:

\[
(-)\rightarrow 0 \rightarrow (+)
\]

---

# Visual Picture

```text
-----\-----/-----
      \   /
       \ /
        ▼
```

---

The bottom point is a local minimum.

---

# Example 1

Consider:

\[
f(x)=x^2
\]

Derivative:

\[
f'(x)=2x
\]

---

Set derivative equal to zero:

\[
2x=0
\]

\[
x=0
\]

---

Function value:

\[
f(0)=0
\]

Minimum point:

\[
(0,0)
\]

---

# Example 2

A marble rolling inside a bowl.

The marble moves downward.

Stops briefly at the bottom.

Then moves upward.

The bottom point is a local minimum.

---

# Real-Life Example

Lowest point in a valley.

You walk downhill.

Reach the bottom.

Then walk uphill.

---

# Easy Memory Rule

**Minimum = Down → Flat → Up**

---

# 3. Definition of a Point of Inflection

---

## What Is a Point of Inflection?

A point of inflection is a point where the graph flattens but does not turn around.

The graph continues in the same overall direction.

---

# Gradient Behavior

Example:

\[
(+)\rightarrow0\rightarrow(+)
\]

or

\[
(-)\rightarrow0\rightarrow(-)
\]

---

Unlike maxima and minima, the sign does not change.

---

# Visual Picture

```text
      /
     /
----•-----
   /
  /
```

---

The graph flattens briefly.

Then continues.

---

# Example

\[
f(x)=x^3
\]

Derivative:

\[
f'(x)=3x^2
\]

---

Set derivative equal to zero:

\[
3x^2=0
\]

\[
x=0
\]

---

Function value:

\[
f(0)=0
\]

Point:

\[
(0,0)
\]

---

Notice:

Before:

\[
3x^2>0
\]

After:

\[
3x^2>0
\]

Still positive.

---

No turning occurs.

Therefore:

\[
(0,0)
\]

is a stationary point of inflection.

---

# Real-Life Example

A car slowing down slightly but continuing forward.

It never reverses direction.

---

# Easy Memory Rule

**Inflection = Flat but keeps going.**

---

# 4. Calculating the Turning Point of a General Quadratic

---

Consider a quadratic:

\[
f(x)=ax^2+bx+c
\]

---

Differentiate:

\[
f'(x)=2ax+b
\]

---

At a turning point:

\[
f'(x)=0
\]

---

Therefore:

\[
2ax+b=0
\]

---

Solve:

\[
2ax=-b
\]

\[
x=-\frac{b}{2a}
\]

---

# Important Formula

\[
\boxed{
x=-\frac{b}{2a}
}
\]

---

This gives the x-coordinate of the vertex.

---

# Example 1

\[
f(x)=x^2-6x+5
\]

---

Using formula:

\[
x=\frac6{2}
\]

\[
x=3
\]

---

Substitute:

\[
f(3)=9-18+5
\]

\[
=-4
\]

---

Turning point:

\[
(3,-4)
\]

---

# Example 2

\[
f(x)=2x^2+8x+1
\]

---

\[
x=\frac{-8}{4}
\]

\[
=-2
\]

---

Turning point occurs at:

\[
x=-2
\]

---

# Real-Life Example

A projectile follows a quadratic path.

The turning point gives the maximum height.

---

# Easy Memory Rule

**Quadratic vertex x-coordinate = \(-b/(2a)\)**

---

# 5. Corroborating Calculus with Graphic Transformations

---

Consider:

\[
f(x)=(x-3)^2
\]

---

From graph transformations:

\[
y=x^2
\]

shifted right by 3.

---

Therefore minimum should occur at:

\[
x=3
\]

---

# Verify Using Calculus

Expand:

\[
f(x)=x^2-6x+9
\]

---

Differentiate:

\[
f'(x)=2x-6
\]

---

Set equal to zero:

\[
2x-6=0
\]

\[
x=3
\]

---

Exactly the same answer.

---

# Why Is This Important?

Calculus confirms what graph transformations predict.

---

# Another Example

\[
f(x)=(x+2)^2
\]

---

Derivative:

\[
2(x+2)
\]

---

Set equal to zero:

\[
x=-2
\]

---

Matches the transformation rule.

---

# Easy Memory Rule

**Calculus and graph transformations always agree.**

---

# 6. Graphing Using Key Features

---

Instead of plotting many points, we can use important graph features.

---

# Step 1: Determine Overall Shape

Look at the highest power term.

---

## Example

\[
y=x^3
\]

Positive leading coefficient.

Shape rises to the right.

---

## Example

\[
y=-x^3
\]

Negative leading coefficient.

Shape falls to the right.

---

# Step 2: Find Y-Intercept

Set:

\[
x=0
\]

---

Example:

\[
y=x^2-4x+3
\]

---

\[
y=3
\]

Point:

\[
(0,3)
\]

---

# Step 3: Find Turning Points

Differentiate.

Set derivative equal to zero.

Solve.

---

# Example

\[
f(x)=x^2-4x+3
\]

---

Derivative:

\[
2x-4
\]

---

Set equal to zero:

\[
x=2
\]

---

Function value:

\[
f(2)=-1
\]

---

Turning point:

\[
(2,-1)
\]

---

# Step 4: Sketch

Now we know:

- Shape
- Intercept
- Turning point

Enough information for a good sketch.

---

# Real-Life Analogy

Drawing a map.

You don't need every tree.

Just key landmarks.

---

# Easy Memory Rule

**Shape + Intercepts + Turning Points = Graph**

---

# 7. Finding Turning Points of a Cubic Function

---

Consider:

\[
f(x)=x(x-1)(x+1)
\]

---

# Step 1: Expand

First:

\[
(x-1)(x+1)
=
x^2-1
\]

---

Multiply by x:

\[
f(x)=x^3-x
\]

---

# Step 2: Differentiate

\[
f'(x)=3x^2-1
\]

---

# Step 3: Set Equal to Zero

\[
3x^2-1=0
\]

---

\[
3x^2=1
\]

---

\[
x^2=\frac13
\]

---

\[
x=\pm\frac1{\sqrt3}
\]

---

These are the stationary points.

---

# Step 4: Find Coordinates

Substitute back into:

\[
f(x)=x^3-x
\]

---

At:

\[
x=\frac1{\sqrt3}
\]

gives local minimum.

---

At:

\[
x=-\frac1{\sqrt3}
\]

gives local maximum.

---

# Why Does a Cubic Have Two Turning Points?

The derivative:

\[
3x^2-1
\]

is quadratic.

Quadratics can have two roots.

Each root creates a stationary point.

---

# Real-Life Example

Think of a roller coaster.

One hill (maximum).

One valley (minimum).

That is the typical cubic shape.

---

# Easy Memory Rule

**Turning points occur wherever the derivative equals zero.**

---

# Complete Summary

---

## Local Maximum

Gradient pattern:

\[
(+)\rightarrow0\rightarrow(-)
\]

Peak.

---

## Local Minimum

Gradient pattern:

\[
(-)\rightarrow0\rightarrow(+)
\]

Valley.

---

## Point of Inflection

Gradient pattern:

\[
(+)\rightarrow0\rightarrow(+)
\]

or

\[
(-)\rightarrow0\rightarrow(-)
\]

Flattens but does not turn.

---

## Quadratic Turning Point

For:

\[
ax^2+bx+c
\]

\[
\boxed{
x=-\frac{b}{2a}
}
\]

---

## Graph Sketching Method

1. Determine shape.
2. Find intercepts.
3. Find turning points.
4. Sketch.

---

## Cubic Turning Points

Differentiate.

Solve:

\[
f'(x)=0
\]

The roots of the derivative locate maxima and minima.

---

### One-Sentence Memory Rule

**A turning point occurs wherever the derivative becomes zero, and by examining how the derivative changes sign around that point, we can determine whether the graph contains a local maximum, local minimum, or stationary point of inflection.**