# Coordinate Axes, Polynomial Behavior, Limits, Asymptotes, and Discontinuities

---

# Introduction

When graphing functions, mathematicians often ask:

```text
What happens far away from the origin?
```

or

```text
What happens near a special point?
```

The mathematical tool used to answer these questions is called a:

```text
Limit
```

Limits help us understand:

- How graphs behave at infinity
- How curves behave near discontinuities
- How polynomials grow
- How rational functions approach asymptotes

This chapter introduces these ideas in a visual and intuitive way.

---

# 1. Defining Coordinate Axes as Line Equations

Most people think of the x-axis and y-axis as lines on a graph.

Mathematically, they are also equations.

---

# The Y-Axis

The y-axis is the vertical line:

\[
x = 0
\]

---

# Why?

Every point on the y-axis has:

```text
x = 0
```

---

# Examples

```text
(0,0)
(0,1)
(0,2)
(0,5)
(0,-3)
```

All have:

```text
x = 0
```

---

# Visualization

```text
      y
      ↑
      |
      |
      |
------|------→ x
      |
      |
      |
```

The vertical line is:

\[
x=0
\]

---

# The X-Axis

The x-axis is the horizontal line:

\[
y = 0
\]

---

# Why?

Every point on the x-axis has:

```text
y = 0
```

---

# Examples

```text
(0,0)
(1,0)
(2,0)
(5,0)
(-3,0)
```

All have:

```text
y = 0
```

---

# Visualization

```text
------------------
        y=0
------------------
```

---

# Real-Life Analogy

Think of:

```text
x-axis = sea level
```

Above it:

```text
positive height
```

Below it:

```text
negative height
```

---

# Summary

| Axis | Equation |
|--------|--------|
| x-axis | y = 0 |
| y-axis | x = 0 |

---

# 2. Fundamental Linear Limits at Infinity

A limit describes what happens as a variable becomes extremely large.

---

# Positive Gradient

Consider:

\[
y=x
\]

---

# Example Values

| x | y |
|---|---|
| 10 | 10 |
| 100 | 100 |
| 1000 | 1000 |

As:

\[
x \to \infty
\]

we see:

\[
y \to \infty
\]

---

# Limit Notation

\[
\lim_{x\to\infty}x
=
\infty
\]

---

# Graph

```text
      /
     /
    /
   /
  /
 /
```

The line keeps rising forever.

---

# Negative Gradient

Consider:

\[
y=-x
\]

---

# Example Values

| x | y |
|---|---|
| 10 | -10 |
| 100 | -100 |
| 1000 | -1000 |

---

As:

\[
x \to \infty
\]

\[
y \to -\infty
\]

---

# Limit Notation

\[
\lim_{x\to\infty}(-x)
=
-\infty
\]

---

# Graph

```text
\
 \
  \
   \
    \
```

The line falls forever.

---

# Key Idea

Positive slope:

```text
Right side goes up
```

Negative slope:

```text
Right side goes down
```

---

# 3. Parabola Behavior and Limits

Quadratic functions behave differently from straight lines.

---

# Positive Parabola

Consider:

\[
y=x^2
\]

---

# Example Values

| x | y |
|---|---|
| 10 | 100 |
| 100 | 10000 |
| -10 | 100 |
| -100 | 10000 |

---

Notice:

```text
Negative numbers become positive when squared.
```

---

# Result

Both ends rise upward.

---

# Limits

\[
\lim_{x\to\infty}x^2
=
\infty
\]

and

\[
\lim_{x\to-\infty}x^2
=
\infty
\]

---

# Graph

```text
*           *
 *         *
  *       *
   *     *
    *   *
     * *
      *
```

---

# Negative Parabola

Consider:

\[
y=-x^2
\]

---

# Example Values

| x | y |
|---|---|
| 10 | -100 |
| -10 | -100 |

---

Both ends go downward.

---

# Limits

\[
\lim_{x\to\infty}(-x^2)
=
-\infty
\]

\[
\lim_{x\to-\infty}(-x^2)
=
-\infty
\]

---

# Graph

```text
      *
     * *
    *   *
   *     *
  *       *
 *         *
```

---

# Summary

| Function | Left End | Right End |
|-----------|-----------|-----------|
| x² | Up | Up |
| -x² | Down | Down |

---

# 4. Higher-Order Polynomials

---

# Cubic Functions

A cubic contains:

\[
x^3
\]

Example:

\[
y=x^3
\]

---

# Important Fact

Negative numbers stay negative:

\[
(-2)^3=-8
\]

---

# Example Values

| x | y |
|---|---|
| -3 | -27 |
| -2 | -8 |
| -1 | -1 |
| 0 | 0 |
| 1 | 1 |
| 2 | 8 |
| 3 | 27 |

---

# Limits

\[
\lim_{x\to\infty}x^3
=
\infty
\]

\[
\lim_{x\to-\infty}x^3
=
-\infty
\]

---

# Shape

```text
      /
     /
    /
---*
  /
 /
/
```

---

# Quartic Functions

A quartic contains:

\[
x^4
\]

---

# Example

\[
y=x^4
\]

---

# Example Values

| x | y |
|---|---|
| -2 | 16 |
| -1 | 1 |
| 0 | 0 |
| 1 | 1 |
| 2 | 16 |

---

# Limits

\[
\lim_{x\to\infty}x^4
=
\infty
\]

\[
\lim_{x\to-\infty}x^4
=
\infty
\]

---

# Shape

Like a steeper quadratic.

```text
*         *
 *       *
  *     *
   *   *
    * *
     *
```

---

# W-Shaped Quartic Example

\[
y=(x^2-1)^2
\]

This quartic has:

```text
Four-direction behavior
```

and resembles:

```text
W
```

---

# Summary

| Function | Left End | Right End |
|-----------|-----------|-----------|
| x³ | Down | Up |
| x⁴ | Up | Up |

---

# 5. Geometry of Repeated Roots (Cuts vs Touches)

Roots tell us where a graph meets the x-axis.

---

# Standard Root (Cuts)

Example:

\[
y=(x-1)
\]

Root:

\[
x=1
\]

---

# Behavior

The graph passes completely through the axis.

---

# Visualization

```text
     /
----*-----
   /
```

Cuts the axis.

---

# Another Example

\[
y=(x-1)(x+2)
\]

Roots:

```text
x=1
x=-2
```

The graph crosses at both locations.

---

# Repeated Root (Touches)

Example:

\[
y=(x-1)^2
\]

---

# Root

\[
x=1
\]

---

# Behavior

The graph touches the axis.

Then turns around.

---

# Visualization

```text
     *
    * *
---*---*---
```

It does not pass through.

---

# Why?

Because:

\[
(x-1)^2
\]

can never become negative.

The graph reaches zero and bounces back.

---

# Summary

| Root Type | Behavior |
|------------|------------|
| Single Root | Cuts through axis |
| Repeated Root | Touches and bounces |

---

# 6. Asymptotic Behavior and Rational Limits

Consider:

\[
y=\frac1x
\]

---

# Large Positive x

\[
\frac1{100}=0.01
\]

\[
\frac1{1000}=0.001
\]

Approaches:

\[
0
\]

---

# Large Negative x

\[
\frac1{-100}=-0.01
\]

\[
\frac1{-1000}=-0.001
\]

Also approaches:

\[
0
\]

---

# Horizontal Asymptote

\[
y=0
\]

---

# Limit

\[
\lim_{x\to\infty}\frac1x=0
\]

\[
\lim_{x\to-\infty}\frac1x=0
\]

---

# Approaching Zero from Right

\[
x\to0^+
\]

Examples:

\[
1/0.1=10
\]

\[
1/0.01=100
\]

\[
1/0.001=1000
\]

---

# Result

\[
\lim_{x\to0^+}\frac1x
=
+\infty
\]

---

# Approaching Zero from Left

\[
x\to0^-
\]

Examples:

\[
1/(-0.1)=-10
\]

\[
1/(-0.01)=-100
\]

---

# Result

\[
\lim_{x\to0^-}\frac1x
=
-\infty
\]

---

# Graph

```text
\       /
 \     /
  \   /
   \ /
   / \
  /   \
 /     \
```

---

# Summary

| Limit | Result |
|---------|---------|
| x→∞ | 0 |
| x→−∞ | 0 |
| x→0⁺ | +∞ |
| x→0⁻ | −∞ |

---

# 7. Dominant Term Analysis for Polynomial Limits

When x becomes very large, the biggest power dominates.

---

# Example

\[
\frac{7x^2-2x}{2x-1}
\]

---

# As x → ∞

Focus on largest powers.

Ignore smaller terms:

\[
\frac{7x^2}{2x}
\]

---

# Simplify

\[
\frac{7x}{2}
\]

---

As:

\[
x\to\infty
\]

\[
\frac{7x}{2}
\to\infty
\]

---

# Conclusion

\[
\lim_{x\to\infty}
\frac{7x^2-2x}{2x-1}
=
\infty
\]

---

# As x → 0

Large powers disappear.

Evaluate:

\[
\frac{-2x}{-1}
=
2x
\]

---

As:

\[
x\to0
\]

\[
2x\to0
\]

---

# Result

\[
\lim_{x\to0}
\frac{7x^2-2x}{2x-1}
=
0
\]

---

# Key Idea

At infinity:

```text
Highest powers dominate.
```

Near zero:

```text
Lowest powers dominate.
```

---

# 8. Removable Discontinuities via Algebraic Cancellation

Sometimes substitution gives:

```text
0/0
```

which is undefined.

---

# Example

\[
\lim_{x\to1}
\frac{x^2-1}{x-1}
\]

---

# Direct Substitution

\[
\frac{1-1}{1-1}
=
\frac00
\]

Undefined.

---

# Factorize

\[
x^2-1
=
(x-1)(x+1)
\]

---

# Substitute

\[
\frac{(x-1)(x+1)}{x-1}
\]

---

# Cancel Common Factor

\[
x+1
\]

---

# New Limit

\[
\lim_{x\to1}(x+1)
\]

---

# Evaluate

\[
1+1=2
\]

---

# Final Answer

\[
\boxed{
\lim_{x\to1}
\frac{x^2-1}{x-1}
=
2
}
\]

---

# Why Is It Called Removable?

The problem existed only because:

```text
(x−1)
```

appeared in both numerator and denominator.

Once cancelled:

```text
Problem disappears.
```

---

# Visualization

Original graph:

```text
---------
    o
---------
```

There is a tiny hole.

After cancellation:

```text
---------
---------
```

The graph becomes smooth.

---

# Complete Summary Table

| Concept | Key Idea |
|----------|----------|
| x-axis | y = 0 |
| y-axis | x = 0 |
| Positive Line | Goes to +∞ |
| Negative Line | Goes to −∞ |
| Positive Parabola | Both ends up |
| Negative Parabola | Both ends down |
| Cubic | Left down, right up |
| Quartic | Both ends up |
| Single Root | Cuts axis |
| Repeated Root | Touches axis |
| y=1/x | Has asymptotes |
| Dominant Term | Largest power controls behavior |
| Removable Discontinuity | Hole removed by cancellation |

---

# Final Key Idea

When studying graphs, limits reveal what happens at the extreme edges of a function and near problematic points.

By understanding:

- Coordinate axes
- Polynomial end behavior
- Repeated roots
- Rational functions
- Asymptotes
- Dominant terms
- Removable discontinuities

you gain the ability to predict the shape and behavior of complex graphs without plotting hundreds of points. These ideas form the foundation of calculus, numerical computing, machine learning, engineering, physics, and advanced mathematical modeling.
