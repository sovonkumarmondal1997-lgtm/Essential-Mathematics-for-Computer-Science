# Trigonometric Relationships, Pythagorean Identity, and the Special 45° Triangle

---

# 1. Relating Triangle Sides to Trigonometric Ratios

Before learning advanced trigonometry, it is important to understand how triangle side lengths and trigonometric ratios are connected.

Consider a right-angled triangle:

```text
        /|
       / |
      /  | Opposite (o)
   h /θ  |
    /____|
 Adjacent(a)
```

Where:

- θ = Reference angle
- o = Opposite side
- a = Adjacent side
- h = Hypotenuse

---

# Review of Sine and Cosine

We know:

```text
sin(θ) = Opposite / Hypotenuse
```

and

```text
cos(θ) = Adjacent / Hypotenuse
```

These formulas tell us the ratio of side lengths.

---

# Finding the Opposite Side

Starting with:

```text
sin(θ) = Opposite / Hypotenuse
```

Multiply both sides by the hypotenuse:

```text
Hypotenuse × sin(θ)
=
Opposite
```

or

```text
Opposite = Hypotenuse × sin(θ)
```

---

## Example 1

Suppose:

```text
Hypotenuse = 10
θ = 30°
```

Since:

```text
sin(30°) = 0.5
```

then:

```text
Opposite
=
10 × 0.5
=
5
```

Answer:

```text
Opposite Side = 5
```

---

# Finding the Adjacent Side

Starting with:

```text
cos(θ)
=
Adjacent / Hypotenuse
```

Multiply both sides by the hypotenuse:

```text
Adjacent
=
Hypotenuse × cos(θ)
```

---

## Example 2

Suppose:

```text
Hypotenuse = 10
θ = 60°
```

Since:

```text
cos(60°) = 0.5
```

then:

```text
Adjacent
=
10 × 0.5
=
5
```

Answer:

```text
Adjacent Side = 5
```

---

# Why This Is Useful

These formulas allow us to calculate missing side lengths without directly using Pythagoras' theorem.

Engineers, architects, surveyors, and game developers use these relationships constantly.

---

# Real-Life Example

Imagine a ladder leaning against a wall.

```text
Wall
 |
 |\
 | \
 |  \
 |   \ Ladder
 |____\
 Ground
```

If:

```text
Ladder Length = 8 m
Angle = 60°
```

Height reached:

```text
8 × sin(60°)

≈ 8 × 0.866

≈ 6.93 m
```

---

# 2. Derivation of the Pythagorean Trigonometric Identity

One of the most important formulas in trigonometry is:

```text
sin²(θ) + cos²(θ) = 1
```

Let's see where it comes from.

---

# Step 1: Start with Pythagoras' Theorem

For every right triangle:

```text
o² + a² = h²
```

---

# Step 2: Substitute Trigonometric Expressions

We already know:

```text
o = h sin(θ)
```

and

```text
a = h cos(θ)
```

Substitute into Pythagoras:

```text
(h sin(θ))² + (h cos(θ))² = h²
```

---

# Step 3: Expand Squares

```text
h²sin²(θ)
+
h²cos²(θ)
=
h²
```

---

# Step 4: Factor Out h²

```text
h²[sin²(θ)+cos²(θ)]
=
h²
```

---

# Step 5: Divide Both Sides by h²

```text
sin²(θ)+cos²(θ)
=
1
```

This gives:

```text
sin²(θ) + cos²(θ) = 1
```

---

# Why Is This Important?

This identity works for:

```text
0°
30°
45°
60°
90°
180°
270°
360°
```

and every angle in between.

It is one of the most frequently used formulas in mathematics, physics, and engineering.

---

# Example

Suppose:

```text
sin(θ)=0.6
```

Find cos(θ).

Using:

```text
sin²(θ)+cos²(θ)=1
```

Substitute:

```text
0.6² + cos²(θ)=1
```

```text
0.36 + cos²(θ)=1
```

```text
cos²(θ)=0.64
```

```text
cos(θ)=0.8
```

---

# 3. Geometric Assumption of Positive Values

When solving geometry problems, side lengths represent physical distances.

Distances cannot be negative.

---

## Example

Suppose:

```text
x² = 25
```

Mathematically:

```text
x = +5
or
x = -5
```

---

## Geometry Interpretation

If x represents:

```text
Length of a wall
```

then:

```text
x = -5 meters
```

does not make physical sense.

Therefore:

```text
x = 5 meters
```

is used.

---

# Why Negative Values Are Ignored

Geometry deals with:

- Length
- Width
- Height
- Distance

These quantities are treated as positive magnitudes.

---

## Example

Suppose:

```text
h² = 100
```

Then:

```text
h = ±10
```

But since h is a side length:

```text
h = 10
```

---

# Real-Life Example

A carpenter measures a plank.

The plank can be:

```text
2 m long
```

but not:

```text
-2 m long
```

---

# 4. Analysis of a Right-Angled Isosceles Triangle

Now let's examine a very special triangle.

---

# What is an Isosceles Triangle?

An isosceles triangle has:

```text
Two equal sides
```

---

# Right-Angled Isosceles Triangle

```text
      /|
     / |
    /  |
   /   |
  /____|
```

where:

```text
Adjacent = Opposite
```

or

```text
a = o
```

---

# Determining the Angles

Every triangle has:

```text
180°
```

total angle sum.

One angle is:

```text
90°
```

Therefore:

```text
180° - 90° = 90°
```

remain.

---

Since the other two sides are equal:

```text
Remaining angles are equal
```

Thus:

```text
90° ÷ 2 = 45°
```

So the angles are:

```text
45°
45°
90°
```

---

# Visual Representation

```text
      /|
     / |
    /  |
   /45°|
  /____|
   45°
```

---

# Real-Life Example

Many square floor tiles are cut diagonally.

The resulting pieces form:

```text
45°-45°-90°
```

triangles.

---

# 5. Exact Trigonometric Values for 45°

Consider:

```text
      /|
     / |
    /o |
 h /45°|
  /____|
    o
```

Since:

```text
Adjacent = Opposite = o
```

---

# Apply Pythagoras

```text
o² + o² = h²
```

Combine terms:

```text
2o² = h²
```

---

# Solve for o

Divide by 2:

```text
o² = h²/2
```

Take square root:

```text
o = h/√2
```

---

# Find Sine

Using:

```text
sin(45°)
=
Opposite / Hypotenuse
```

Substitute:

```text
sin(45°)
=
(h/√2)/h
```

Cancel h:

```text
sin(45°)
=
1/√2
```

---

# Find Cosine

Using:

```text
cos(45°)
=
Adjacent / Hypotenuse
```

Substitute:

```text
cos(45°)
=
(h/√2)/h
```

Therefore:

```text
cos(45°)
=
1/√2
```

---

# Exact Values

```text
sin(45°)
=
1/√2
```

```text
cos(45°)
=
1/√2
```

---

# Decimal Approximation

Since:

```text
√2 ≈ 1.414
```

then:

```text
1/√2 ≈ 0.7071
```

Therefore:

```text
sin(45°)
≈ 0.7071
```

```text
cos(45°)
≈ 0.7071
```

---

# Why Are They Equal?

Because:

```text
Adjacent = Opposite
```

Both ratios use the same numerator.

Therefore:

```text
sin(45°)
=
cos(45°)
```

---

# 6. Verification Using the Pythagorean Identity

Now let's verify our answer.

---

# Identity

```text
sin²(θ)+cos²(θ)=1
```

Substitute:

```text
sin(45°)=1/√2
```

and

```text
cos(45°)=1/√2
```

---

# Compute

```text
(1/√2)² + (1/√2)²
```

---

Square each term:

```text
1/2 + 1/2
```

---

Add:

```text
1
```

Therefore:

```text
(1/√2)² + (1/√2)² = 1
```

Perfectly correct.

---

# What Does This Show?

This demonstrates that:

- Geometry is consistent.
- Pythagoras' theorem is consistent.
- Trigonometric ratios are consistent.
- Algebra agrees with geometry.

Everything connects together.

---

# Complete 45° Triangle Summary

```text
Angles:
45°
45°
90°
```

---

```text
Sides:
o = a
```

---

```text
Pythagoras:
2o² = h²
```

---

```text
o = h/√2
```

---

```text
sin(45°)
=
1/√2
≈ 0.7071
```

---

```text
cos(45°)
=
1/√2
≈ 0.7071
```

---

```text
tan(45°)
=
1
```

because:

```text
Opposite = Adjacent
```

---

# Quick Formula Sheet

## Side Relationships

```text
Opposite = Hypotenuse × sin(θ)
```

```text
Adjacent = Hypotenuse × cos(θ)
```

---

## Pythagorean Identity

```text
sin²(θ)+cos²(θ)=1
```

---

## 45° Triangle

```text
sin(45°)=1/√2
```

```text
cos(45°)=1/√2
```

```text
tan(45°)=1
```

---

# Final Key Idea

A right-angled isosceles triangle (45°-45°-90° triangle) is one of the most important shapes in trigonometry. By combining:

- Pythagoras' theorem
- Sine and cosine definitions
- Algebraic manipulation

we discover the fundamental identity:

```text
sin²(θ)+cos²(θ)=1
```

and the exact trigonometric values:

```text
sin(45°)=cos(45°)=1/√2
```

which appear throughout mathematics, physics, computer graphics, engineering, and machine learning.
