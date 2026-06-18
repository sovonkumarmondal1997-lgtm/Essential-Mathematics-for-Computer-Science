# Shearing, Translation, and Introduction to Homogeneous Coordinates

---

# Introduction

So far, we have studied several important geometric transformations:

- Scaling
- Reflection
- Rotation

All of these transformations can be performed using ordinary:

\[
2\times2
\]

matrices.

Now we will learn:

- Shearing
- Translation
- Why Translation cannot be performed with ordinary 2×2 matrices
- Why mathematicians introduce Homogeneous Coordinates

These concepts are fundamental in:

- Computer Graphics
- Animation
- CAD Software
- Robotics
- Computer Vision
- Video Games
- Augmented Reality (AR)
- Virtual Reality (VR)

---

# 1. Shearing / Shear Transformation

## Simple Definition

A **Shear Transformation** slants a shape.

Instead of making the shape larger or rotating it,

shearing pushes one part of the shape sideways while keeping another part fixed.

---

## Visual Idea

Original Rectangle

```
+------+
|      |
|      |
|      |
+------+
```

---

After Shearing

```
   +------+
  /      /
 /      /
/______/
```

Notice:

- Shape is slanted
- Area remains the same
- Angles change

---

## Real-Life Example 1

Italic Text

Normal text:

```
HELLO
```

Italic text:

```
/HELLO/
```

This is essentially a shear transformation.

---

## Real-Life Example 2

Strong Wind

Imagine a tall building.

A strong wind pushes the top sideways.

The building appears sheared.

---

## Real-Life Example 3

Stack of Cards

Push the top of a card stack sideways.

The stack becomes slanted.

---

# What Changes?

### Changes

- Angles
- Shape appearance

### Does Not Change

- Area
- Parallel lines

---

# 2. Shearing Matrix Structure

There are two common types:

---

# X-Shear

## Matrix

\[
S_x=
\begin{bmatrix}
1 & s_x\\
0 & 1
\end{bmatrix}
\]

---

## Meaning

The x-coordinate changes.

The y-coordinate stays unchanged.

---

### Transformation Rule

\[
x' = x+s_xy
\]

\[
y' = y
\]

---

## Example 1

Let:

\[
s_x=2
\]

Matrix:

\[
\begin{bmatrix}
1 & 2\\
0 & 1
\end{bmatrix}
\]

Point:

\[
(1,1)
\]

Result:

\[
(3,1)
\]

---

## Example 2

Point:

\[
(2,3)
\]

Result:

\[
(8,3)
\]

---

# Y-Shear

## Matrix

\[
S_y=
\begin{bmatrix}
1 & 0\\
s_y & 1
\end{bmatrix}
\]

---

## Meaning

The y-coordinate changes.

The x-coordinate remains unchanged.

---

### Transformation Rule

\[
x'=x
\]

\[
y'=s_yx+y
\]

---

## Example 1

Let:

\[
s_y=2
\]

Point:

\[
(1,1)
\]

Result:

\[
(1,3)
\]

---

## Example 2

Point:

\[
(3,2)
\]

Result:

\[
(3,8)
\]

---

# Why Ones on the Main Diagonal?

Notice:

\[
\begin{bmatrix}
1 & s_x\\
0 & 1
\end{bmatrix}
\]

and

\[
\begin{bmatrix}
1 & 0\\
s_y & 1
\end{bmatrix}
\]

Both contain:

\[
1
\]

on the leading diagonal.

These ones preserve the original coordinate while adding a slanting effect.

---

# 3. Area Preservation in Shearing

## Simple Definition

Shearing changes shape,

but not area.

---

## Why?

Because the determinant equals:

\[
1
\]

---

# Example: X-Shear

\[
\begin{bmatrix}
1 & s_x\\
0 & 1
\end{bmatrix}
\]

Determinant:

\[
(1)(1)-(s_x)(0)
\]

\[
=1
\]

---

# Example: Y-Shear

\[
\begin{bmatrix}
1 & 0\\
s_y & 1
\end{bmatrix}
\]

Determinant:

\[
(1)(1)-(0)(s_y)
\]

\[
=1
\]

---

# Geometric Meaning

If area before transformation is:

\[
10
\]

then after shearing:

\[
10\times1
=
10
\]

Area remains unchanged.

---

## Example 1

Rectangle area:

\[
20
\]

After shearing:

\[
20
\]

---

## Example 2

Triangle area:

\[
12
\]

After shearing:

\[
12
\]

---

## Example 3

Square area:

\[
25
\]

After shearing:

\[
25
\]

---

# Important Observation

### Rotation

Preserves area.

### Reflection

Preserves area.

### Shearing

Preserves area.

---

All have determinant magnitude:

\[
1
\]

---

# 4. Unit Square Matrix Representation

## Simple Definition

A shape can be represented as a matrix.

---

# Unit Square

Vertices:

\[
(0,0)
\]

\[
(1,0)
\]

\[
(1,1)
\]

\[
(0,1)
\]

---

## Coordinate Matrix

\[
Q=
\begin{bmatrix}
0 & 1 & 1 & 0\\
0 & 0 & 1 & 1
\end{bmatrix}
\]

---

## Meaning

Column 1:

\[
(0,0)
\]

Column 2:

\[
(1,0)
\]

Column 3:

\[
(1,1)
\]

Column 4:

\[
(0,1)
\]

---

# Why Useful?

Instead of transforming each point separately:

```
Transform Point 1
Transform Point 2
Transform Point 3
Transform Point 4
```

we transform the entire square at once.

---

## Example

Apply shear matrix:

\[
S_xQ
\]

Entire square becomes sheared.

---

# 5. Fixed Origin Limitation of 2D Linear Transformations

## Simple Definition

Every ordinary:

\[
2\times2
\]

matrix has a limitation.

The origin:

\[
(0,0)
\]

always stays fixed.

---

# Why?

Take any matrix:

\[
A=
\begin{bmatrix}
a & b\\
c & d
\end{bmatrix}
\]

Multiply:

\[
A
\begin{bmatrix}
0\\
0
\end{bmatrix}
\]

---

Result:

\[
\begin{bmatrix}
0\\
0
\end{bmatrix}
\]

---

Always.

---

# Example 1

Rotation

Origin remains fixed.

---

# Example 2

Reflection

Origin remains fixed.

---

# Example 3

Scaling

Origin remains fixed.

---

# Important Conclusion

Using only:

\[
2\times2
\]

matrices,

we can never move the origin.

---

# 6. Translation

## Simple Definition

Translation means moving a shape from one location to another.

---

## Visual

Before:

```
□
```

After:

```
        □
```

Shape unchanged.

Location changed.

---

# Example 1

Move point:

\[
(2,3)
\]

by:

\[
(+5,+2)
\]

Result:

\[
(7,5)
\]

---

# Example 2

Move a car on a map.

---

# Example 3

Move a game character.

---

# Important Observation

Translation changes:

- Position

but not:

- Shape
- Size
- Area

---

# Why Can't 2×2 Matrices Perform Translation?

Suppose:

\[
(0,0)
\]

must become:

\[
(5,2)
\]

---

But every 2×2 matrix sends:

\[
(0,0)
\]

back to:

\[
(0,0)
\]

---

Impossible.

---

# Therefore

Translation is NOT a standard linear transformation.

---

# 7. 3D Matrix Transformations for 2D Space

## The Solution

Mathematicians add an extra coordinate.

---

Instead of:

\[
(x,y)
\]

we use:

\[
(x,y,1)
\]

---

Now points live in:

\[
3D
\]

even though the shape remains 2D.

---

# Example

Point:

\[
(2,3)
\]

becomes:

\[
(2,3,1)
\]

---

# Translation Matrix

\[
T=
\begin{bmatrix}
1 & 0 & t_x\\
0 & 1 & t_y\\
0 & 0 & 1
\end{bmatrix}
\]

---

Suppose:

\[
t_x=5
\]

\[
t_y=2
\]

---

Matrix:

\[
\begin{bmatrix}
1 & 0 & 5\\
0 & 1 & 2\\
0 & 0 & 1
\end{bmatrix}
\]

---

Apply to:

\[
\begin{bmatrix}
2\\
3\\
1
\end{bmatrix}
\]

---

Result:

\[
\begin{bmatrix}
7\\
5\\
1
\end{bmatrix}
\]

---

Translation achieved.

---

# Why Important?

Now we can perform:

- Translation
- Rotation
- Scaling
- Reflection

using one unified framework.

---

# 8. Homogeneous Coordinates / Homogeneous Equations

## Simple Definition

Homogeneous coordinates add one extra coordinate.

---

Instead of:

\[
(x,y)
\]

we use:

\[
(x,y,1)
\]

---

This extra coordinate allows translation to be expressed using matrix multiplication.

---

# Example 1

Ordinary coordinate:

\[
(3,4)
\]

Homogeneous form:

\[
(3,4,1)
\]

---

# Example 2

Point:

\[
(0,0)
\]

Homogeneous:

\[
(0,0,1)
\]

---

# Example 3

Entire triangle:

\[
\begin{bmatrix}
x_1 & x_2 & x_3\\
y_1 & y_2 & y_3\\
1 & 1 & 1
\end{bmatrix}
\]

---

# Why Introduced?

To combine all transformations into matrix multiplication.

Without homogeneous coordinates:

```
Rotation → Matrix

Scaling → Matrix

Reflection → Matrix

Translation → Special Case
```

---

With homogeneous coordinates:

```
Rotation → Matrix

Scaling → Matrix

Reflection → Matrix

Translation → Matrix
```

Everything becomes unified.

---

# Complete Big Picture

## Shearing

Slants a shape.

---

## X-Shear Matrix

\[
\begin{bmatrix}
1 & s_x\\
0 & 1
\end{bmatrix}
\]

---

## Y-Shear Matrix

\[
\begin{bmatrix}
1 & 0\\
s_y & 1
\end{bmatrix}
\]

---

## Area Preservation

\[
det=1
\]

Area unchanged.

---

## Unit Square Matrix

\[
\begin{bmatrix}
0 & 1 & 1 & 0\\
0 & 0 & 1 & 1
\end{bmatrix}
\]

Represents a square algebraically.

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

Moves a shape.

Cannot be achieved using ordinary:

\[
2\times2
\]

matrices.

---

## 3×3 Transformations

Add an extra coordinate:

\[
(x,y,1)
\]

to allow translation.

---

## Homogeneous Coordinates

Provide a unified mathematical framework for:

- Translation
- Rotation
- Reflection
- Scaling
- Shearing

using matrix multiplication.

---

These ideas form the mathematical foundation of:

- Computer Graphics
- OpenGL
- DirectX
- CAD Systems
- Robotics
- Computer Vision
- Animation
- Video Games
- Virtual Reality
- Augmented Reality

where millions of geometric transformations are computed every second.