# Homogeneous Coordinates and Composite Transformations

---

# Introduction

In previous chapters, we learned:

- Vectors
- Matrices
- Scaling
- Reflection
- Rotation
- Shearing
- Translation Limitations of 2×2 Matrices

We discovered an important problem:

> Ordinary 2×2 matrices cannot perform translations.

To solve this problem, mathematicians and computer graphics engineers introduced:

# Homogeneous Coordinates

This concept is one of the most important ideas in:

- Computer Graphics
- Game Engines
- CAD Software
- Robotics
- Computer Vision
- Augmented Reality
- Virtual Reality

---

# 1. Homogeneous Coordinates

## Simple Definition

Homogeneous Coordinates are a way of representing a 2D point using three numbers instead of two.

Instead of writing:

\[
(x,y)
\]

we write:

\[
(x,y,1)
\]

---

## Why Add an Extra Coordinate?

The extra coordinate allows:

- Translation
- Rotation
- Scaling
- Reflection
- Shearing

to all be performed using matrix multiplication.

---

# Example 1

Ordinary Point:

\[
(2,3)
\]

Homogeneous Form:

\[
\begin{bmatrix}
2\\
3\\
1
\end{bmatrix}
\]

---

# Example 2

Point:

\[
(5,8)
\]

Homogeneous Form:

\[
\begin{bmatrix}
5\\
8\\
1
\end{bmatrix}
\]

---

# Example 3

Origin:

\[
(0,0)
\]

becomes

\[
\begin{bmatrix}
0\\
0\\
1
\end{bmatrix}
\]

---

# Real-Life Analogy

Think of adding a "special passport stamp" to every point.

Normal point:

```
(x,y)
```

Homogeneous point:

```
(x,y,1)
```

The extra coordinate allows the point to travel through transformations that were previously impossible.

---

# Why Computer Graphics Uses It

Every object in:

- Games
- Movies
- CAD software

is usually transformed using homogeneous coordinates.

---

# 2. Fixed Origin Limitation of Linear Transformations

## Simple Definition

Every ordinary:

\[
2\times2
\]

matrix leaves the origin fixed.

---

# Why?

Suppose:

\[
A=
\begin{bmatrix}
a & b\\
c & d
\end{bmatrix}
\]

---

Multiply by origin:

\[
\begin{bmatrix}
0\\
0
\end{bmatrix}
\]

---

Result:

\[
A
\begin{bmatrix}
0\\
0
\end{bmatrix}
=
\begin{bmatrix}
0\\
0
\end{bmatrix}
\]

---

Always.

---

# Example 1

Scaling

\[
\begin{bmatrix}
2 & 0\\
0 & 2
\end{bmatrix}
\]

Origin remains:

\[
(0,0)
\]

---

# Example 2

Rotation

Origin remains:

\[
(0,0)
\]

---

# Example 3

Reflection

Origin remains:

\[
(0,0)
\]

---

# Why Is This a Problem?

Suppose we want:

\[
(0,0)
\rightarrow
(5,2)
\]

A 2×2 matrix cannot do it.

---

# Important Conclusion

Translation is impossible using only standard linear transformations.

---

# 3. Translation via 3×3 Matrices

## Simple Definition

By moving to:

\[
3\times3
\]

matrices,

translation becomes possible.

---

# General Translation Matrix

\[
T=
\begin{bmatrix}
1 & 0 & t_x\\
0 & 1 & t_y\\
0 & 0 & 1
\end{bmatrix}
\]

---

where

\[
t_x
\]

is horizontal movement.

---

\[
t_y
\]

is vertical movement.

---

# Example 1

Move:

- 5 units right
- 2 units up

Matrix:

\[
\begin{bmatrix}
1 & 0 & 5\\
0 & 1 & 2\\
0 & 0 & 1
\end{bmatrix}
\]

---

Point:

\[
\begin{bmatrix}
1\\
3\\
1
\end{bmatrix}
\]

---

Result:

\[
\begin{bmatrix}
6\\
5\\
1
\end{bmatrix}
\]

---

# Example 2

Move:

\[
(-3,+4)
\]

---

Point:

\[
(10,2)
\]

becomes:

\[
(7,6)
\]

---

# Example 3

Video Game Character

Current Position:

\[
(50,20)
\]

Move right:

\[
10
\]

Result:

\[
(60,20)
\]

---

# Why It Works

The extra coordinate allows addition to be hidden inside matrix multiplication.

---

# 4. Homogeneous Transformation Matrix Structure

## Simple Definition

Every valid 2D homogeneous transformation matrix has a fixed bottom row:

\[
\begin{bmatrix}
0 & 0 & 1
\end{bmatrix}
\]

---

# General Structure

\[
\begin{bmatrix}
a & b & t_x\\
c & d & t_y\\
0 & 0 & 1
\end{bmatrix}
\]

---

The top-left part:

\[
\begin{bmatrix}
a & b\\
c & d
\end{bmatrix}
\]

controls:

- Scaling
- Rotation
- Reflection
- Shearing

---

The last column controls:

- Translation

---

# Example 1

Pure Translation

\[
\begin{bmatrix}
1 & 0 & 5\\
0 & 1 & 2\\
0 & 0 & 1
\end{bmatrix}
\]

---

# Example 2

Scaling + Translation

\[
\begin{bmatrix}
2 & 0 & 3\\
0 & 2 & 1\\
0 & 0 & 1
\end{bmatrix}
\]

---

# Example 3

Rotation + Translation

\[
\begin{bmatrix}
0 & -1 & 5\\
1 & 0 & 2\\
0 & 0 & 1
\end{bmatrix}
\]

---

# Memory Trick

Bottom row never changes:

\[
(0,0,1)
\]

---

# 5. Multiple / Composite Transformations

## Simple Definition

Real-world graphics rarely use one transformation.

Usually multiple transformations occur together.

---

Example:

1. Enlarge
2. Rotate
3. Translate

---

Instead of performing three separate operations,

we combine them into one matrix.

---

# Example 1

Scale then Translate.

---

# Example 2

Rotate then Translate.

---

# Example 3

Scale then Rotate then Translate.

---

# Real-Life Example

Video Game Character

```
Scale Character
Rotate Character
Move Character
```

All combined into one matrix.

---

# Why Useful?

Faster computations.

Graphics cards do this millions of times per second.

---

# 6. Order of Matrix Composition

## Very Important Rule

Suppose:

Transformation B happens first.

Then:

Transformation A.

---

Combined matrix:

\[
AB
\]

---

The transformation nearest the point happens first.

---

# Example

Point:

\[
P
\]

Apply:

1. Scale
2. Rotate

---

Result:

\[
RP
\]

after scaling becomes:

\[
R(SP)
\]

---

Using associativity:

\[
(RS)P
\]

---

Combined matrix:

\[
RS
\]

---

# Memory Trick

Read right to left.

```
ABP
```

First:

```
P
```

Then:

```
B
```

Then:

```
A
```

---

# Example 2

Wear:

1. Socks
2. Shoes

Order matters.

---

# Example 3

Paint wall then build wall.

Different from:

Build wall then paint wall.

---

# 7. Associative Property of Matrix Multiplication

## Rule

\[
(AB)C
=
A(BC)
\]

---

## What Does This Mean?

Grouping does not matter.

Order still matters.

---

# Example

\[
(AB)C
\]

and

\[
A(BC)
\]

produce the same result.

---

# Important

Associative:

✔ True

---

Commutative:

✘ Usually False

---

# Example 1

Numbers:

\[
(2\times3)\times4
=
2\times(3\times4)
\]

---

# Example 2

Graphics Pipeline

Scale

Rotate

Translate

can be grouped efficiently.

---

# Example 3

Game Engine

Precompute transformation matrix once.

Use repeatedly.

---

# Why Important?

Allows composite transformations to be built efficiently.

---

# 8. Inverse of a Composite Transformation

("Socks-and-Shoes Property")

---

## Fundamental Rule

\[
(AB)^{-1}
=
B^{-1}A^{-1}
\]

---

Notice:

Order reverses.

---

# Why?

Because we must undo operations backwards.

---

# Real-Life Example

Putting on:

1. Socks
2. Shoes

---

To remove:

1. Shoes
2. Socks

---

Reverse order.

---

# Example 1

Scale then Translate.

Undo:

Translate Back

Then Scale Back

---

# Example 2

Rotate then Translate.

Undo:

Translate Back

Then Rotate Back

---

# Example 3

Open Door

Walk Through

To reverse:

Walk Back

Close Door

---

# Memory Trick

```
Forward:
A then B

Reverse:
B⁻¹ then A⁻¹
```

---

# 9. Inverse Translation

## Simple Definition

Undo a translation by moving the exact opposite distance.

---

# Example 1

Move:

\[
(+5,+2)
\]

Inverse:

\[
(-5,-2)
\]

---

# Example 2

Move:

\[
(+10,0)
\]

Inverse:

\[
(-10,0)
\]

---

# Example 3

Walk:

10 steps East.

Undo:

10 steps West.

---

# Translation Matrix

\[
\begin{bmatrix}
1 & 0 & 5\\
0 & 1 & 2\\
0 & 0 & 1
\end{bmatrix}
\]

---

Inverse:

\[
\begin{bmatrix}
1 & 0 & -5\\
0 & 1 & -2\\
0 & 0 & 1
\end{bmatrix}
\]

---

# 10. Inverse Enlargement / Fractional Scaling

## Simple Definition

Scaling is undone using reciprocals.

---

# Example 1

Scale by:

\[
2
\]

Inverse:

\[
\frac12
\]

---

Result:

Original size restored.

---

# Example 2

Scale by:

\[
3
\]

Inverse:

\[
\frac13
\]

---

# Example 3

Scale by:

\[
0.25
\]

Inverse:

\[
4
\]

---

# Scaling Matrix

\[
\begin{bmatrix}
2 & 0\\
0 & 2
\end{bmatrix}
\]

---

Inverse:

\[
\begin{bmatrix}
1/2 & 0\\
0 & 1/2
\end{bmatrix}
\]

---

# Real-Life Analogy

Photocopy at:

200%

Then photocopy at:

50%

Original size returns.

---

# Complete Big Picture

## Homogeneous Coordinates

Represent:

\[
(x,y)
\]

as

\[
(x,y,1)
\]

---

## Fixed-Origin Limitation

Every:

\[
2\times2
\]

matrix keeps:

\[
(0,0)
\]

fixed.

---

## Translation

Achieved using:

\[
3\times3
\]

homogeneous matrices.

---

## Homogeneous Matrix Structure

\[
\begin{bmatrix}
a & b & t_x\\
c & d & t_y\\
0 & 0 & 1
\end{bmatrix}
\]

---

## Composite Transformations

Multiple transformations combined into one matrix.

---

## Order Rule

If:

B first

then A

Combined matrix:

\[
AB
\]

---

## Associativity

\[
(AB)C=A(BC)
\]

---

## Composite Inverse

\[
(AB)^{-1}
=
B^{-1}A^{-1}
\]

---

## Inverse Translation

Move opposite distance.

---

## Inverse Scaling

Multiply by reciprocal.

---

These ideas form the mathematical foundation of:

- Computer Graphics
- OpenGL
- DirectX
- CAD Software
- Robotics
- Animation
- Computer Vision
- AR/VR Systems
- Scientific Visualization
- Game Engines

where complex transformation pipelines are built from simple matrix operations.