# Introduction to Quadratic Functions, Parabolas, Intercepts, and Factorization

---

# Introduction

So far, we have studied **linear equations** such as:

\[
y = 2x + 1
\]

which produce straight lines.

Quadratic equations introduce a new idea:

\[
x^2
\]

This single change transforms the graph from a straight line into a curved shape called a **parabola**.

Quadratics appear everywhere in mathematics, physics, engineering, computer graphics, machine learning, and data science.

---

# 1. Introduction to Quadratics

## What is a Quadratic Equation?

A quadratic equation is an equation that contains:

\[
x^2
\]

as its highest power.

---

# General Form

Every quadratic can be written as:

\[
y = ax^2 + bx + c
\]

where:

- \(a\) controls the curve's direction and steepness
- \(b\) influences the position and tilt
- \(c\) determines the y-intercept

---

# Example 1

\[
y = x^2
\]

---

# Example 2

\[
y = 2x^2 + 3x - 1
\]

---

# Example 3

\[
y = -x^2 + 4
\]

All are quadratic equations because the highest power is:

\[
x^2
\]

---

# Why Are Quadratics Different?

Linear Equation:

\[
y = x
\]

produces:

```text
/
/
/
/
```

a straight line.

---

Quadratic Equation:

\[
y = x^2
\]

produces:

```text
   *
  * *
 *   *
*     *
```

a curved shape.

---

# Example Table for y = x²

| x | y=x² |
|---|---|
| -3 | 9 |
| -2 | 4 |
| -1 | 1 |
| 0 | 0 |
| 1 | 1 |
| 2 | 4 |
| 3 | 9 |

---

# Graph Shape

```text
9 | *         *
8 |
7 |
6 |
5 |
4 |   *     *
3 |
2 |
1 |     * *
0 |       *
  +----------------
   -3 -2 -1 0 1 2 3
```

This U-shaped curve is called a:

```text
Parabola
```

---

# Real-Life Example

Throw a ball into the air.

The path followed by the ball is approximately a quadratic curve.

---

# 2. Immediate Y-Intercept Identification

## What is the Y-Intercept?

The y-intercept is the point where the graph crosses the y-axis.

---

# Key Fact

Every point on the y-axis has:

\[
x = 0
\]

---

# Start with General Form

\[
y=ax^2+bx+c
\]

Substitute:

\[
x=0
\]

---

# Calculation

\[
y=a(0)^2+b(0)+c
\]

Everything disappears except:

\[
y=c
\]

---

# Important Result

For every quadratic:

\[
\boxed{\text{Y-Intercept}=c}
\]

---

# Example 1

\[
y=x^2+5
\]

Here:

\[
c=5
\]

Therefore:

```text
Y-intercept = (0,5)
```

---

# Example 2

\[
y=x^2-3
\]

Here:

\[
c=-3
\]

Therefore:

```text
Y-intercept = (0,-3)
```

---

# Example 3

\[
y=2x^2+4x+7
\]

Here:

\[
c=7
\]

Therefore:

```text
Y-intercept = (0,7)
```

---

# Quick Shortcut

Whenever you see:

\[
y=ax^2+bx+c
\]

immediately read:

```text
Y-intercept = c
```

without doing any calculations.

---

# Real-Life Analogy

Imagine the parabola is a bridge.

The value:

\[
c
\]

tells you where the bridge begins on the vertical axis.

---

# 3. Vertical Translations (Shifting the Curve)

## What is a Translation?

A translation means:

```text
Moving the graph
without changing its shape.
```

---

# Base Curve

Start with:

\[
y=x^2
\]

---

# Graph

```text
   *
  * *
 *   *
*     *
```

---

# Shift Upward

Consider:

\[
y=x^2+2
\]

Every output becomes:

```text
2 units larger
```

---

# Example Values

| x | x² | x²+2 |
|---|---|---|
| -1 | 1 | 3 |
| 0 | 0 | 2 |
| 1 | 1 | 3 |

---

# Result

The entire graph moves upward.

```text
Original

    *
   * *
  *   *

Shifted Up

      *
     * *
    *   *
```

---

# Shift Downward

Consider:

\[
y=x^2-3
\]

Every output becomes:

```text
3 units smaller
```

---

# Example Values

| x | x² | x²−3 |
|---|---|---|
| -1 | 1 | -2 |
| 0 | 0 | -3 |
| 1 | 1 | -2 |

---

# Result

The entire graph moves downward.

```text
Original

   *
  * *
 *   *

Shifted Down

 *   *
  * *
   *
```

---

# Important Observation

Changing:

\[
c
\]

only moves the graph:

```text
Up or Down
```

It does NOT change:

- Width
- Shape
- Steepness

---

# Summary

| Equation | Shift |
|-----------|-----------|
| y=x²+2 | Up 2 |
| y=x²+5 | Up 5 |
| y=x²−3 | Down 3 |
| y=x²−10 | Down 10 |

---

# Real-Life Example

Think of an elevator.

The shape of the elevator remains unchanged.

Only its height changes.

---

# 4. The Power of Factorization (Finding the Roots)

## What is Factorization?

Factorization rewrites a quadratic as a multiplication.

---

# Example

Original:

\[
y=x^2-1
\]

Factored:

\[
y=(x+1)(x-1)
\]

---

# Why Factor?

Factorization makes it easy to find where the graph crosses the x-axis.

---

# What is an X-Intercept?

An x-intercept occurs when:

\[
y=0
\]

---

# Using the Factored Form

Set:

\[
(x+1)(x-1)=0
\]

---

# Zero Product Rule

If two numbers multiply to give zero:

```text
At least one factor must be zero.
```

---

# First Root

\[
x+1=0
\]

\[
x=-1
\]

---

# Second Root

\[
x-1=0
\]

\[
x=1
\]

---

# Result

The graph crosses the x-axis at:

```text
(-1,0)
```

and

```text
(1,0)
```

---

# Visualization

```text
      *
    *   *
---*-----*---
 -1   0   1
```

---

# Why Roots Matter

Roots tell us:

```text
Where the graph touches or crosses the x-axis.
```

This makes graph sketching much easier.

---

# Example 2

Factor:

\[
y=x^2-4
\]

---

# Rewrite

\[
y=(x+2)(x-2)
\]

---

# Find Roots

\[
x=-2
\]

\[
x=2
\]

---

# X-Intercepts

```text
(-2,0)
```

```text
(2,0)
```

---

# Real-Life Example

Imagine a ball thrown upward.

The roots represent the moments when the ball touches the ground.

---

# 5. Parabola Orientation (Positive vs. Negative Curves)

The sign of the \(x^2\) term determines the direction the parabola opens.

---

# Positive Quadratic

Example:

\[
y=x^2
\]

---

# Shape

```text
   *
  * *
 *   *
*     *
```

---

# Description

```text
U-shaped
```

Opens upward.

---

# Why?

As:

\[
x
\]

gets larger:

\[
x^2
\]

gets larger.

---

# Example Values

| x | y |
|---|---|
| -2 | 4 |
| -1 | 1 |
| 0 | 0 |
| 1 | 1 |
| 2 | 4 |

Everything grows upward.

---

# Negative Quadratic

Example:

\[
y=-x^2
\]

---

# Shape

```text
*     *
 *   *
  * *
   *
```

---

# Description

```text
Upside-Down U
```

Opens downward.

---

# Why?

The negative sign flips all outputs.

---

# Example Values

| x | y |
|---|---|
| -2 | -4 |
| -1 | -1 |
| 0 | 0 |
| 1 | -1 |
| 2 | -4 |

All values become negative.

---

# Reflection Interpretation

\[
y=-x^2
\]

is simply:

```text
y=x² reflected across the x-axis
```

---

# Visual Comparison

Positive:

```text
   *
  * *
 *   *
*     *
```

Negative:

```text
*     *
 *   *
  * *
   *
```

---

# Real-Life Example

### Positive Parabola

A satellite dish.

```text
U-shape
```

---

### Negative Parabola

A thrown basketball.

```text
Upside-down U
```

---

# Quick Summary Table

| Feature | Positive x² | Negative x² |
|-----------|-----------|-----------|
| Shape | U-shape | Upside-down U |
| Opens | Upward | Downward |
| Example | y=x² | y=-x² |
| Reflection | No | Reflected across x-axis |

---

# Complete Quadratic Checklist

Given:

\[
y=ax^2+bx+c
\]

Identify:

### Y-Intercept

```text
c
```

---

### Roots

Set:

\[
y=0
\]

Factorize and solve.

---

### Direction

If:

\[
a>0
\]

```text
Opens Up
```

If:

\[
a<0
\]

```text
Opens Down
```

---

# Final Key Idea

Quadratic functions are the next major step beyond straight lines.

Their general form:

\[
y=ax^2+bx+c
\]

creates a curved graph called a **parabola**.

Three of the most important features can be found quickly:

- **Y-Intercept:** The value \(c\)
- **Roots (X-Intercepts):** Found using factorization
- **Orientation:** Determined by the sign of \(a\)

These ideas allow you to sketch quadratic graphs quickly and form the foundation for advanced algebra, calculus, physics, engineering, machine learning, computer graphics, and data science.
