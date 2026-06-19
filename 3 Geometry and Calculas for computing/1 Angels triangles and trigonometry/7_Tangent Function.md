# Tangent Function: Zero-Crossings, Asymptotes, Limits, and Infinite Discontinuities

---

# Introduction

Unlike sine and cosine, which stay between:

```text
-1 and 1
```

the tangent function behaves very differently.

Recall:

```text
tan(θ)
=
sin(θ)/cos(θ)
```

Because cosine sometimes becomes zero, tangent can become extremely large or extremely small.

This creates:

- Zero-crossing points
- Vertical asymptotes
- Positive infinity
- Negative infinity
- Infinite discontinuities

These ideas are very important in calculus, physics, engineering, computer graphics, and signal processing.

---

# 1. Zero-Crossing Points of Tangent

## What is a Zero-Crossing?

A zero-crossing is a point where a graph passes through:

```text
y = 0
```

For tangent:

```text
tan(θ)=0
```

whenever the slope is perfectly flat.

---

# Why Does This Happen?

Recall:

```text
tan(θ)
=
sin(θ)/cos(θ)
```

For a fraction to equal zero:

```text
Numerator = 0
```

Therefore:

```text
sin(θ)=0
```

---

# When Is Sine Equal to Zero?

At:

```text
0
π
2π
3π
4π
...
```

or generally:

```text
nπ
```

where:

```text
n = 0,1,2,3,...
```

---

# Zero-Crossing Points

Therefore:

```text
tan(0)=0
```

```text
tan(π)=0
```

```text
tan(2π)=0
```

```text
tan(3π)=0
```

and so on.

---

# Visual Representation

```text
      /
     /
----*---------
   /
  /
 /
```

The star (*) shows the graph crossing:

```text
y = 0
```

---

# Example 1

At:

```text
θ = π
```

```text
sin(π)=0
```

```text
cos(π)=-1
```

Therefore:

```text
tan(π)
=
0/(-1)
=
0
```

---

# Example 2

At:

```text
θ = 2π
```

```text
sin(2π)=0
```

```text
cos(2π)=1
```

Thus:

```text
tan(2π)=0
```

---

# Real-Life Analogy

Imagine a road.

When the road becomes perfectly flat:

```text
Slope = 0
```

That is exactly what happens at tangent's zero-crossing points.

---

# Summary

Tangent crosses zero at:

```text
0, π, 2π, 3π, ...
```

or

```text
θ = nπ
```

---

# 2. Asymptotic Behavior (Positive and Negative Infinity)

## What is an Asymptote?

An asymptote is a line that a graph gets closer and closer to but never actually touches.

For tangent:

```text
x = π/2
```

is a vertical asymptote.

---

# Why Does This Happen?

Recall:

```text
tan(θ)
=
sin(θ)/cos(θ)
```

At:

```text
θ = π/2
```

we have:

```text
sin(π/2)=1
```

```text
cos(π/2)=0
```

Thus:

```text
tan(π/2)
=
1/0
```

Division by zero is undefined.

---

# What Happens Near π/2?

As cosine gets closer and closer to zero:

```text
0.1
0.01
0.001
0.0001
```

the fraction becomes enormous.

Example:

```text
1/0.1 = 10
```

```text
1/0.01 = 100
```

```text
1/0.001 = 1000
```

and so on.

---

# Result

The graph shoots upward toward:

```text
+∞
```

or downward toward:

```text
-∞
```

---

# Visual

```text
       |
       |
      /
     /
----|
   /
  /
 /
```

The vertical line is the asymptote.

The graph never touches it.

---

# Difference from Sine and Cosine

Sine:

```text
-1 ≤ sin(θ) ≤ 1
```

Cosine:

```text
-1 ≤ cos(θ) ≤ 1
```

Tangent:

```text
No maximum value
```

```text
No minimum value
```

It can grow forever.

---

# Example

Near:

```text
89°
```

```text
tan(89°)
≈ 57.29
```

Near:

```text
89.9°
```

```text
tan(89.9°)
≈ 572.96
```

Near:

```text
89.99°
```

```text
tan(89.99°)
≈ 5729.58
```

The values explode toward infinity.

---

# 3. Directional Limits and Left-Hand Behavior

## What is a Left-Hand Limit?

A left-hand limit studies what happens when we approach a point from values smaller than that point.

Notation:

```text
lim
x→a⁻
```

The minus sign means:

```text
Approach from the left
```

---

# Example

Consider:

```text
x → π/2
```

from below.

Values:

```text
1.4
1.5
1.56
1.569
1.5707
```

all slightly less than:

```text
π/2 ≈ 1.5708
```

---

# Tangent Values

```text
tan(1.4) ≈ 5.8
```

```text
tan(1.5) ≈ 14.1
```

```text
tan(1.56) ≈ 92.6
```

```text
tan(1.569) ≈ 556
```

The numbers keep increasing.

---

# Left-Hand Limit

Therefore:

```text
lim x→(π/2)⁻ tan(x)
=
+∞
```

---

# Meaning

As we approach:

```text
π/2
```

from the left:

```text
Tangent grows forever upward.
```

---

# Visual

```text
      /
     /
    /
   /
  /
 |
 |
 |
```

The graph rises infinitely.

---

# Real-Life Analogy

Imagine climbing a hill that becomes steeper and steeper.

Near the top:

```text
Slope → ∞
```

The hill becomes almost vertical.

---

# 4. Directional Limits and Right-Hand Behavior

## What is a Right-Hand Limit?

A right-hand limit studies what happens when we approach from values larger than the target.

Notation:

```text
lim
x→a⁺
```

The plus sign means:

```text
Approach from the right
```

---

# Example

Approaching:

```text
π/2
```

from above.

Values:

```text
1.58
1.575
1.571
```

all slightly greater than:

```text
1.5708
```

---

# Tangent Values

```text
tan(1.58) ≈ -108
```

```text
tan(1.575) ≈ -238
```

```text
tan(1.571) ≈ -4900
```

The values become more negative.

---

# Right-Hand Limit

Therefore:

```text
lim x→(π/2)⁺ tan(x)
=
-∞
```

---

# Meaning

Immediately after crossing:

```text
π/2
```

the graph appears to jump from:

```text
+∞
```

to

```text
-∞
```

---

# Visual

```text
|
|
|
 \
  \
   \
    \
```

The graph returns from negative infinity.

---

# Why Does This Happen?

Because:

```text
cos(x)
```

changes sign.

Before π/2:

```text
cos(x) > 0
```

After π/2:

```text
cos(x) < 0
```

The denominator changes from positive to negative.

This flips the sign of tangent.

---

# 5. Infinite Discontinuity at Odd Multiples of π/2

## What is a Discontinuity?

A discontinuity is a break in a graph.

The graph cannot be drawn continuously through that point.

---

# Infinite Discontinuity

For tangent:

```text
x = π/2
```

creates an infinite discontinuity.

The graph breaks apart.

---

# Why?

At:

```text
π/2
```

```text
cos(π/2)=0
```

Therefore:

```text
tan(π/2)
```

is undefined.

---

# Same Problem at 3π/2

At:

```text
3π/2
```

```text
cos(3π/2)=0
```

Again:

```text
tan(3π/2)
```

is undefined.

---

# General Pattern

Discontinuities occur at:

```text
π/2
```

```text
3π/2
```

```text
5π/2
```

```text
7π/2
```

and so on.

---

# General Formula

All odd multiples of:

```text
π/2
```

can be written as:

```text
(2n+1)π/2
```

where:

```text
n = 0,1,2,3,...
```

---

# What Happens Geometrically?

Imagine a line extending from the origin to a point on the unit circle.

At:

```text
90°
```

the line becomes perfectly vertical.

```text
|
|
|
|
```

A vertical line has:

```text
Infinite slope
```

---

# Then It Flips

Immediately after:

```text
90°
```

the slope changes direction.

The graph jumps from:

```text
+∞
```

to

```text
-∞
```

---

# At 270°

The exact same phenomenon occurs.

```text
+∞
```

suddenly switches to:

```text
-∞
```

again.

---

# Tangent Graph Overview

```text
      /|      /|
     / |     / |
    /  |    /  |
---/---|---/---|---
  /    |  /    |
 /     | /     |
/      |/      |
```

Vertical lines represent asymptotes.

The graph never touches them.

---

# Important Tangent Facts

| Angle | tan(θ) |
|---------|---------|
| 0 | 0 |
| π/4 | 1 |
| π/2 | Undefined |
| π | 0 |
| 3π/2 | Undefined |
| 2π | 0 |

---

# Key Limits

### Left-Hand Limit

```text
lim x→(π/2)⁻ tan(x)
=
+∞
```

---

### Right-Hand Limit

```text
lim x→(π/2)⁺ tan(x)
=
-∞
```

---

### Similar Behavior

```text
lim x→(3π/2)⁻ tan(x)
=
+∞
```

```text
lim x→(3π/2)⁺ tan(x)
=
-∞
```

---

# Quick Summary

| Concept | Meaning |
|----------|----------|
| Zero-Crossing | Point where tan(θ)=0 |
| Zero Locations | 0, π, 2π, 3π, ... |
| Asymptote | Vertical line graph approaches |
| Left-Hand Limit | Approach from smaller values |
| Right-Hand Limit | Approach from larger values |
| Positive Infinity | Values grow forever upward |
| Negative Infinity | Values grow forever downward |
| Infinite Discontinuity | Graph breaks at asymptote |
| Tangent Period | π |
| Asymptote Locations | (2n+1)π/2 |

---

# Final Key Idea

The tangent function behaves very differently from sine and cosine:

- **Sine and cosine are bounded** between -1 and 1.
- **Tangent is unbounded** and can grow without limit.
- It crosses zero at:

```text
0, π, 2π, 3π, ...
```

- It has vertical asymptotes at:

```text
π/2, 3π/2, 5π/2, ...
```

- As it approaches these points, it shoots toward:

```text
+∞ or -∞
```

creating **infinite discontinuities** that split the graph into separate repeating sections.
