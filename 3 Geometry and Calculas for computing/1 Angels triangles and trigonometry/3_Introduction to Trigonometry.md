# Introduction to Trigonometry: Unit Circle, Sine, Cosine, Tangent, and SOH-CAH-TOA

---

# 1. The Unit Circle

## What is a Unit Circle?

A **Unit Circle** is a circle whose radius is exactly:

```text
r = 1
```

The word "unit" means one unit long.

---

## Visual Representation

```text
          (0,1)
             *
          *     *
       *           *
(-1,0)*     O       *(1,0)
       *           *
          *     *
             *
          (0,-1)
```

Where:

```text
O = Origin (Center)
```

and

```text
Radius = 1
```

---

## Why is the Unit Circle Important?

The unit circle is the foundation of trigonometry because:

- It helps define sine and cosine.
- It allows us to measure angles.
- It connects geometry and algebra.
- It helps describe waves, sound, light, and motion.

---

## Example

Suppose a point moves around the unit circle.

As it moves:

- Its horizontal position changes.
- Its vertical position changes.

These changing positions create the trigonometric functions:

```text
sin(θ)
cos(θ)
```

---

## Real-Life Analogy

Imagine a Ferris wheel with radius:

```text
1 meter
```

As a passenger moves around:

- Their height changes.
- Their left-right position changes.

These changes behave exactly like sine and cosine.

---

# 2. Intuitive Definition of Sine (sinθ)

## What is Sine?

Sine measures the vertical position (height) of a point moving around a circle.

Think of sine as answering:

```text
"How high is the point?"
```

---

## Movement Around the Circle

Start at:

```text
0°
```

```text
(1,0)
```

The point is on the right side of the circle.

Height:

```text
sin(0°) = 0
```

---

### At 90°

```text
      *
      |
      |
      O
```

The point reaches its highest position.

```text
sin(90°) = 1
```

---

### At 180°

The point moves to the left side.

```text
sin(180°) = 0
```

---

### At 270°

The point reaches the lowest position.

```text
sin(270°) = -1
```

---

### At 360°

Returns to starting position.

```text
sin(360°) = 0
```

---

## Summary Table

| Angle | Sine Value |
|---------|---------|
| 0° | 0 |
| 90° | 1 |
| 180° | 0 |
| 270° | -1 |
| 360° | 0 |

---

## Sine Wave Shape

```text
 1 |      *
   |    *   *
 0 | *       *     *
   |           * *
-1 |             *
```

The value smoothly rises and falls.

---

## Geometric Meaning

Consider:

```text
      /|
     / |
    /  | Opposite
   /θ  |
  /____|
```

On the unit circle:

```text
sin(θ)
```

is exactly the vertical height.

---

## Example

At:

```text
θ = 30°
```

```text
sin(30°) = 0.5
```

Meaning:

The point is halfway up the circle.

---

## Real-World Application

### Sound Waves

When you speak:

- Air vibrates.
- The vibration follows sine-wave patterns.

Music, speech, and audio recordings are combinations of many sine waves.

---

### Ocean Waves

The rise and fall of waves often resemble sine curves.

---

### Electricity

Alternating Current (AC) electricity follows sine-wave behavior.

---

# 3. Intuitive Definition of Cosine (cosθ)

## What is Cosine?

Cosine measures the horizontal position of a point moving around the circle.

Think of cosine as answering:

```text
"How far left or right is the point?"
```

---

## Movement Around the Circle

### At 0°

The point starts on the far right.

```text
cos(0°) = 1
```

Maximum value.

---

### At 90°

Point reaches top.

```text
cos(90°) = 0
```

---

### At 180°

Point reaches far left.

```text
cos(180°) = -1
```

---

### At 270°

Point reaches bottom.

```text
cos(270°) = 0
```

---

### At 360°

Returns to starting point.

```text
cos(360°) = 1
```

---

## Summary Table

| Angle | Cosine Value |
|---------|---------|
| 0° | 1 |
| 90° | 0 |
| 180° | -1 |
| 270° | 0 |
| 360° | 1 |

---

## Cosine Wave Shape

```text
 1 | *         *
   |   *     *
 0 |     * *
   |
-1 |       *
```

---

## Geometric Meaning

```text
      /|
     / |
    /  |
   /θ  |
  /____|
 Adjacent
```

On the unit circle:

```text
cos(θ)
```

equals the horizontal distance.

---

## Example

At:

```text
θ = 60°
```

```text
cos(60°) = 0.5
```

Meaning:

The point is halfway across the circle.

---

## Real-Life Example

### Ferris Wheel Position

Cosine can describe:

```text
Left-right movement
```

of a rider as the wheel rotates.

---

# 4. Generalizing Trigonometric Ratios

## Problem

The unit circle has:

```text
Radius = 1
```

But real triangles can be much larger.

Example:

```text
Hypotenuse = 10
```

or

```text
Hypotenuse = 100
```

We need a way to describe angles independent of size.

---

## Solution

Scale everything by dividing by the hypotenuse.

---

# Sine Formula

```text
sin(θ)
=
Opposite / Hypotenuse
```

---

## Example

```text
Opposite = 3
Hypotenuse = 5
```

```text
sin(θ)
=
3/5
=
0.6
```

---

# Cosine Formula

```text
cos(θ)
=
Adjacent / Hypotenuse
```

---

## Example

```text
Adjacent = 4
Hypotenuse = 5
```

```text
cos(θ)
=
4/5
=
0.8
```

---

## Why Values Stay Between -1 and 1

Because:

```text
Side ≤ Hypotenuse
```

the ratio can never exceed:

```text
1
```

or be less than:

```text
-1
```

---

# 5. Tangent (tanθ) and Gradient

## What is Tangent?

Tangent measures steepness or slope.

It answers:

```text
"How steep is the angle?"
```

---

## Gradient Concept

Gradient means:

```text
Rise / Run
```

or

```text
Upward movement
----------------
Horizontal movement
```

---

## Example

A road rises:

```text
4 meters
```

while moving:

```text
8 meters
```

across.

Gradient:

```text
4/8
=
0.5
```

---

# Tangent Formula

```text
tan(θ)
=
Opposite / Adjacent
```

---

## Example

```text
Opposite = 3
Adjacent = 4
```

```text
tan(θ)
=
3/4
=
0.75
```

---

# Relationship with Sine and Cosine

Since:

```text
sin(θ)
=
Opposite / Hypotenuse
```

and

```text
cos(θ)
=
Adjacent / Hypotenuse
```

Dividing them gives:

```text
sin(θ)/cos(θ)

=
(Opposite/Hypotenuse)
/
(Adjacent/Hypotenuse)

=
Opposite/Adjacent
```

Therefore:

```text
tan(θ)
=
sin(θ)/cos(θ)
```

---

## Example

If:

```text
sin(θ)=0.6
```

and

```text
cos(θ)=0.8
```

then

```text
tan(θ)

=
0.6/0.8

=
0.75
```

---

## Real-Life Applications

### Road Slope

Engineers use tangent to measure steepness.

---

### Roof Design

Roof angles use tangent calculations.

---

### Construction

Stairs and ramps use tangent to determine incline.

---

# 6. SOH-CAH-TOA Mnemonic

## What is SOH-CAH-TOA?

SOH-CAH-TOA is a memory trick that helps remember the three main trigonometric ratios.

---

# SOH

```text
S
O
H
```

Means:

```text
Sine
=
Opposite
----------
Hypotenuse
```

---

## Example

```text
Opposite = 6
Hypotenuse = 10
```

```text
sin(θ)
=
6/10

=
0.6
```

---

# CAH

```text
C
A
H
```

Means:

```text
Cosine
=
Adjacent
----------
Hypotenuse
```

---

## Example

```text
Adjacent = 8
Hypotenuse = 10
```

```text
cos(θ)
=
8/10

=
0.8
```

---

# TOA

```text
T
O
A
```

Means:

```text
Tangent
=
Opposite
----------
Adjacent
```

---

## Example

```text
Opposite = 6
Adjacent = 8
```

```text
tan(θ)
=
6/8

=
0.75
```

---

# Complete Example

Consider:

```text
      /|
     / |
 10 /  | 6
   /θ  |
  /____|
     8
```

---

## Sine

```text
sin(θ)
=
6/10

=
0.6
```

---

## Cosine

```text
cos(θ)
=
8/10

=
0.8
```

---

## Tangent

```text
tan(θ)
=
6/8

=
0.75
```

---

# Quick Summary

| Function | Formula | Meaning |
|-----------|-----------|-----------|
| sin(θ) | Opposite / Hypotenuse | Vertical position (height) |
| cos(θ) | Adjacent / Hypotenuse | Horizontal position |
| tan(θ) | Opposite / Adjacent | Slope or steepness |

---

# Unit Circle Values

| Angle | sin(θ) | cos(θ) |
|---------|---------|---------|
| 0° | 0 | 1 |
| 90° | 1 | 0 |
| 180° | 0 | -1 |
| 270° | -1 | 0 |
| 360° | 0 | 1 |

---

# SOH-CAH-TOA Cheat Sheet

```text
SOH
Sine     = Opposite / Hypotenuse

CAH
Cosine   = Adjacent / Hypotenuse

TOA
Tangent  = Opposite / Adjacent
```

---

# Final Key Idea

Think of a point moving around a unit circle:

- **Sine** tells you how high the point is.
- **Cosine** tells you how far left or right the point is.
- **Tangent** tells you how steep the angle is.

These three functions form the foundation of trigonometry, physics, engineering, computer graphics, signal processing, machine learning, and many real-world technologies.
