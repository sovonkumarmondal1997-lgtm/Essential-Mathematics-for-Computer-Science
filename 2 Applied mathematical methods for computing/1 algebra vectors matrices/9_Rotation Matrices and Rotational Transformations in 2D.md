# Rotation Matrices and Rotational Transformations in 2D

---

# Introduction

In previous chapters, we learned:

- Matrices
- Determinants
- Matrix Inverses
- Scaling Matrices
- Reflection Matrices
- Geometric Transformations

Now we study one of the most important transformations in mathematics and computer graphics:

# Rotation

Rotation allows us to turn objects around a fixed point without changing:

- Shape
- Size
- Area
- Distances

Rotations are used in:

- Robotics
- Video Games
- Animation
- Computer Graphics
- Physics
- Aerospace
- Machine Learning Geometry

---

# 1. General Form of a 2D Rotation Matrix

## Simple Definition

A rotation matrix rotates points around the origin by an angle:

\[
\theta
\]

in the counterclockwise direction.

---

## General Formula

\[
R(\theta)
=
\begin{bmatrix}
\cos\theta & -\sin\theta \\
\sin\theta & \cos\theta
\end{bmatrix}
\]

---

## What Does It Mean?

The matrix contains:

- Cosine values
- Sine values

which determine how much the point rotates.

---

## Example 1

Rotate a point by:

\[
45^\circ
\]

The matrix becomes:

\[
\begin{bmatrix}
\cos45^\circ & -\sin45^\circ \\
\sin45^\circ & \cos45^\circ
\end{bmatrix}
\]

---

## Example 2

Rotate a game character.

Original:

```
→
```

After 90° rotation:

```
↑
```

---

## Example 3

Rotate a clock hand.

Every second, the hand rotates by a small angle.

---

## Visual Idea

Before:

```
●
 \
  \
   \
```

After Rotation:

```
      ●
     /
    /
```

---

# Why Rotation Matrices Matter

Instead of manually calculating every point,

one matrix multiplication rotates an entire shape.

---

# 2. Trigonometric Identity (Pythagorean Identity)

## Simple Definition

One of the most important formulas in mathematics:

\[
\cos^2\theta+\sin^2\theta=1
\]

---

## Why Important?

It guarantees that rotations preserve length.

---

## Example 1

\[
\theta=0^\circ
\]

\[
\cos(0^\circ)=1
\]

\[
\sin(0^\circ)=0
\]

Therefore:

\[
1^2+0^2=1
\]

---

## Example 2

\[
\theta=90^\circ
\]

\[
0^2+1^2=1
\]

---

## Example 3

\[
\theta=45^\circ
\]

\[
\left(\frac{\sqrt2}{2}\right)^2
+
\left(\frac{\sqrt2}{2}\right)^2
\]

\[
=
\frac12+\frac12
\]

\[
=1
\]

---

## Real-Life Analogy

Imagine walking around a perfect circle.

No matter where you stand:

\[
x^2+y^2=1
\]

always remains true.

---

# 3. Determinant of a Rotation Matrix

## Formula

For:

\[
R(\theta)
=
\begin{bmatrix}
\cos\theta & -\sin\theta\\
\sin\theta & \cos\theta
\end{bmatrix}
\]

---

Determinant:

\[
det(R)
=
\cos^2\theta+\sin^2\theta
\]

---

Using the Pythagorean Identity:

\[
det(R)=1
\]

---

# Why Is This Important?

Determinant tells us how area changes.

---

If determinant:

\[
=1
\]

then:

- Area unchanged
- Shape unchanged
- Distances unchanged

---

## Example 1

Rotate a square.

Area remains exactly the same.

---

## Example 2

Rotate a triangle.

Area remains unchanged.

---

## Example 3

Rotate a photograph.

Image orientation changes.

Size does not.

---

# Key Observation

Rotation is a rigid transformation.

Rigid means:

```
No stretching
No shrinking
No distortion
```

---

# 4. Rotation by 0° or 360°

## Rotation by 0°

No rotation occurs.

---

Using:

\[
\cos0^\circ=1
\]

\[
\sin0^\circ=0
\]

---

Matrix:

\[
R(0)
=
\begin{bmatrix}
1 & 0\\
0 & 1
\end{bmatrix}
\]

---

This is exactly the:

# Identity Matrix

---

## Rotation by 360°

One complete revolution.

---

After full rotation:

Object returns to original position.

---

Matrix:

\[
R(360^\circ)
=
\begin{bmatrix}
1 & 0\\
0 & 1
\end{bmatrix}
\]

---

## Example 1

Clock hand makes one full turn.

Returns to original position.

---

## Example 2

Spin a coin completely.

Same orientation.

---

## Example 3

Video game character spins once.

Returns to starting direction.

---

# 5. Rotation Matrix for 90°

## Step 1

Use:

\[
\cos90^\circ=0
\]

\[
\sin90^\circ=1
\]

---

## Step 2

Substitute into formula:

\[
R(90^\circ)
=
\begin{bmatrix}
0 & -1\\
1 & 0
\end{bmatrix}
\]

---

## Example 1

Point:

\[
(1,0)
\]

Result:

\[
(0,1)
\]

---

## Example 2

Point:

\[
(2,3)
\]

Result:

\[
(-3,2)
\]

---

## Example 3

Arrow:

```
→
```

becomes:

```
↑
```

---

## Memory Trick

90° Rotation:

\[
(x,y)
\rightarrow
(-y,x)
\]

---

# 6. Rotation Matrix for 180°

## Step 1

Use:

\[
\cos180^\circ=-1
\]

\[
\sin180^\circ=0
\]

---

## Matrix

\[
R(180^\circ)
=
\begin{bmatrix}
-1 & 0\\
0 & -1
\end{bmatrix}
\]

---

## Effect

\[
(x,y)
\rightarrow
(-x,-y)
\]

---

## Example 1

\[
(2,3)
\]

becomes

\[
(-2,-3)
\]

---

## Example 2

\[
(5,-1)
\]

becomes

\[
(-5,1)
\]

---

## Example 3

Turn an arrow upside down.

```
→
```

becomes

```
←
```

---

# Interesting Property

Applying 180° twice:

\[
180^\circ+180^\circ
=
360^\circ
\]

returns original position.

---

# 7. Inverse Rotations / Multiplicative Identity Combinations

## Simple Definition

Some rotations undo others.

---

## Example

Rotate:

\[
90^\circ
\]

then:

\[
270^\circ
\]

---

Total:

\[
360^\circ
\]

---

Result:

Original position.

---

## Example 1

Turn left 90°.

Then right 90°.

Back to original direction.

---

## Example 2

Rotate:

\[
45^\circ
\]

then:

\[
-45^\circ
\]

Back to start.

---

## Example 3

Game character turns and turns back.

---

## Matrix View

\[
R(90^\circ)
R(270^\circ)
=
I
\]

---

# 8. Fixed Point of Rotation (Center of Rotation)

## Simple Definition

A rotation occurs around a specific point.

That point remains fixed.

---

For standard rotation matrices:

\[
(0,0)
\]

is fixed.

---

## Example 1

Point:

\[
(0,0)
\]

After rotation:

\[
(0,0)
\]

unchanged.

---

## Example 2

Compass needle rotates around its center.

---

## Example 3

Ceiling fan blades rotate around the motor.

---

## Visual

```
      ●
    /
  /
O
 \
  \
    ●

```

O stays fixed.

---

# Why Important?

Everything rotates around this center.

---

# 9. Inverse Matrix of a Rotation

## Fundamental Rule

The inverse of a rotation matrix is:

\[
R(-\theta)
\]

---

Meaning:

Rotate by:

\[
\theta
\]

then rotate by:

\[
-\theta
\]

---

Result:

Original position.

---

## Formula

\[
R(\theta)
R(-\theta)
=
I
\]

---

## Example 1

Rotate:

\[
30^\circ
\]

then

\[
-30^\circ
\]

Back to start.

---

## Example 2

Rotate:

\[
90^\circ
\]

then

\[
-90^\circ
\]

Back to start.

---

## Example 3

Rotate:

\[
180^\circ
\]

then

\[
-180^\circ
\]

Back to start.

---

## Real-Life Analogy

Walk 10 steps forward.

Walk 10 steps backward.

Return to starting point.

---

# 10. Even and Odd Trigonometric Functions

## Cosine is Even

### Rule

\[
\cos(-\theta)
=
\cos(\theta)
\]

---

## Example

\[
\cos(60^\circ)
=
0.5
\]

\[
\cos(-60^\circ)
=
0.5
\]

Same value.

---

## Example 2

\[
\cos(45^\circ)
=
0.707
\]

\[
\cos(-45^\circ)
=
0.707
\]

---

# Sine is Odd

### Rule

\[
\sin(-\theta)
=
-\sin(\theta)
\]

---

## Example

\[
\sin(30^\circ)
=
0.5
\]

\[
\sin(-30^\circ)
=
-0.5
\]

---

## Example 2

\[
\sin(90^\circ)
=
1
\]

\[
\sin(-90^\circ)
=
-1
\]

---

# Why Important?

These properties allow us to derive:

\[
R^{-1}
=
R(-\theta)
\]

for rotation matrices.

---

# Complete Big Picture

## General Rotation Matrix

\[
R(\theta)
=
\begin{bmatrix}
\cos\theta & -\sin\theta\\
\sin\theta & \cos\theta
\end{bmatrix}
\]

---

## Pythagorean Identity

\[
\cos^2\theta+\sin^2\theta=1
\]

---

## Determinant

\[
det(R)=1
\]

Area preserved.

---

## Rotation by 0° or 360°

\[
R=
I
\]

No net change.

---

## Rotation by 90°

\[
\begin{bmatrix}
0 & -1\\
1 & 0
\end{bmatrix}
\]

---

## Rotation by 180°

\[
\begin{bmatrix}
-1 & 0\\
0 & -1
\end{bmatrix}
\]

---

## Inverse Rotations

\[
R(\theta)R(-\theta)=I
\]

---

## Fixed Point

The origin:

\[
(0,0)
\]

remains unchanged.

---

## Even/Odd Properties

Cosine:

\[
\cos(-\theta)=\cos(\theta)
\]

Even function.

---

Sine:

\[
\sin(-\theta)=-\sin(\theta)
\]

Odd function.

---

These ideas form the foundation for:

- Computer Graphics
- Animation
- Robotics
- Aerospace
- Physics
- CAD Systems
- Computer Vision
- Machine Learning
- Neural Networks
- Scientific Simulations

where rotations are among the most common geometric transformations used every day.