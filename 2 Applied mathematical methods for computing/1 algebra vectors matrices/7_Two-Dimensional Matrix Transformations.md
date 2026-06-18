# Two-Dimensional Matrix Transformations

---

# Introduction

So far, we have learned:

- Vectors
- Matrices
- Matrix Multiplication
- Determinants
- Matrix Inverses

Now we will learn one of the most practical applications of matrices:

# Geometric Transformations

Matrices can:

- Move objects
- Rotate objects
- Reflect objects
- Stretch objects
- Shrink objects
- Slant objects

These transformations are used everywhere:

- Computer Graphics
- Video Games
- Animation
- Robotics
- Computer Vision
- CAD Software
- Machine Learning

---

# 1. Geometric Transformations via Two-Dimensional Matrices

## Simple Definition

A geometric transformation changes:

- Position
- Shape
- Size
- Orientation

of an object.

---

## The Big Idea

Suppose we have a point:

\[
P=
\begin{bmatrix}
x\\
y
\end{bmatrix}
\]

We multiply it by a matrix:

\[
A
\]

to get a new point:

\[
P'
=
AP
\]

---

## Visual Idea

Before:

```
     ●
    (2,3)
```

Apply matrix.

After:

```
         ●
       (4,6)
```

The point moves.

---

## Example 1

Original point:

\[
(2,3)
\]

Transformation matrix:

\[
\begin{bmatrix}
2 & 0\\
0 & 2
\end{bmatrix}
\]

Result:

\[
(4,6)
\]

Everything doubles.

---

## Example 2

Video Game Character

Original:

\[
(5,2)
\]

Transformation matrix rotates character.

New position:

\[
(-2,5)
\]

---

## Example 3

Robot Arm

Matrix transformations determine:

- Position
- Rotation
- Orientation

---

# Why Matrices?

Without matrices:

Every point must be transformed individually.

With matrices:

One operation transforms an entire shape.

---

# 2. Reflection

## Simple Definition

Reflection creates a mirror image.

---

## Reflection Across x-axis

Matrix:

\[
\begin{bmatrix}
1 & 0\\
0 & -1
\end{bmatrix}
\]

---

### Example

Point:

\[
(2,3)
\]

Multiply:

\[
\begin{bmatrix}
1 & 0\\
0 & -1
\end{bmatrix}
\begin{bmatrix}
2\\
3
\end{bmatrix}
=
\begin{bmatrix}
2\\
-3
\end{bmatrix}
\]

---

Result:

\[
(2,-3)
\]

---

## Visual

Before:

```
      ●
      (2,3)

------------- x-axis

```

After:

```
------------- x-axis

      ●
      (2,-3)

```

---

# Reflection Across y-axis

Matrix:

\[
\begin{bmatrix}
-1 & 0\\
0 & 1
\end{bmatrix}
\]

---

## Example

Point:

\[
(4,2)
\]

Result:

\[
(-4,2)
\]

---

# Real-Life Example

Looking into a mirror.

Your left and right appear reversed.

---

# Example 2

Logo design software.

Mirror effect uses reflection matrices.

---

# Example 3

Computer graphics.

Character facing left becomes facing right.

---

# 3. Rotation

## Simple Definition

Rotation means turning an object around a fixed point.

Usually around:

\[
(0,0)
\]

called the origin.

---

# Rotation Matrix

For angle \(\theta\):

\[
R=
\begin{bmatrix}
\cos\theta & -\sin\theta\\
\sin\theta & \cos\theta
\end{bmatrix}
\]

---

# Example 1

Rotate by:

\[
90^\circ
\]

Matrix becomes:

\[
\begin{bmatrix}
0 & -1\\
1 & 0
\end{bmatrix}
\]

---

Point:

\[
(1,0)
\]

Result:

\[
(0,1)
\]

---

## Visual

Before

```
● (1,0)

```

After

```
     ● (0,1)

```

---

# Example 2

Clock Hand

Every second:

rotation occurs.

---

# Example 3

Video Games

Character turning.

Car steering.

Camera rotation.

All use rotation matrices.

---

# Important Observation

Rotation changes:

- Direction

but not:

- Shape
- Area
- Size

---

# 4. Shearing

## Simple Definition

Shearing means slanting an object.

Imagine pushing the top of a rectangle sideways.

---

## Visual

Before:

```
|      |
|      |
|      |
|______|

```

After:

```
   /|
  / |
 /  |
/___|

```

---

# Horizontal Shear Matrix

\[
\begin{bmatrix}
1 & k\\
0 & 1
\end{bmatrix}
\]

---

## Example

Let:

\[
k=2
\]

Matrix:

\[
\begin{bmatrix}
1 & 2\\
0 & 1
\end{bmatrix}
\]

---

Point:

\[
(1,1)
\]

Result:

\[
(3,1)
\]

---

# Example 2

Italic text.

Text editors create italic effects using shearing.

---

# Example 3

Perspective effects in graphics.

---

# Important Observation

Shearing changes:

- Angles

but often preserves:

- Area

---

# 5. Enlargement / Scaling

## Simple Definition

Scaling changes the size of an object.

---

Two possibilities:

### Enlargement

Make larger.

### Reduction

Make smaller.

---

# Example 1

Double Size

Matrix:

\[
\begin{bmatrix}
2 & 0\\
0 & 2
\end{bmatrix}
\]

---

Point:

\[
(3,4)
\]

Result:

\[
(6,8)
\]

---

# Example 2

Shrink

Matrix:

\[
\begin{bmatrix}
0.5 & 0\\
0 & 0.5
\end{bmatrix}
\]

---

Point:

\[
(6,8)
\]

Result:

\[
(3,4)
\]

---

# Example 3

Stretch Only Horizontally

Matrix:

\[
\begin{bmatrix}
3 & 0\\
0 & 1
\end{bmatrix}
\]

---

Point:

\[
(2,5)
\]

Result:

\[
(6,5)
\]

---

# Real-Life Examples

- Zooming images
- Resizing photos
- Enlarging maps
- Video game scaling

---

# 6. Geometric Matrix Representation of Shapes

## Simple Definition

A shape can be represented as a matrix.

Each column stores one vertex.

---

# Example

Triangle vertices:

\[
(0,0)
\]

\[
(2,0)
\]

\[
(1,2)
\]

---

Matrix form:

\[
T=
\begin{bmatrix}
0 & 2 & 1\\
0 & 0 & 2
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
(2,0)
\]

Column 3:

\[
(1,2)
\]

---

# Why Useful?

One matrix multiplication transforms the entire shape.

---

Instead of:

```
Transform point 1
Transform point 2
Transform point 3
```

We do:

\[
AT
\]

once.

---

# Example 2

Square represented by four columns.

---

# Example 3

3D models in games.

Thousands of vertices stored in matrices.

---

# 7. General Form of a Scaling Matrix

## Simple Definition

General scaling matrix:

\[
S=
\begin{bmatrix}
s_x & 0\\
0 & s_y
\end{bmatrix}
\]

---

Where:

\[
s_x
\]

controls horizontal scaling.

---

\[
s_y
\]

controls vertical scaling.

---

# Example 1

\[
s_x=2
\]

\[
s_y=3
\]

---

Matrix:

\[
\begin{bmatrix}
2 & 0\\
0 & 3
\end{bmatrix}
\]

---

Point:

\[
(1,2)
\]

Result:

\[
(2,6)
\]

---

# Example 2

\[
s_x=1
\]

\[
s_y=4
\]

Only vertical stretching.

---

# Example 3

\[
s_x=0.5
\]

\[
s_y=0.5
\]

Uniform shrinking.

---

# Special Cases

## Uniform Scaling

\[
s_x=s_y
\]

Shape remains similar.

---

## Non-Uniform Scaling

\[
s_x\ne s_y
\]

Shape becomes distorted.

---

# 8. Determinant as an Area Scale Factor

## Simple Definition

The determinant tells us how area changes after transformation.

---

## Rule

If

\[
det(A)=k
\]

then:

\[
\text{New Area}
=
k\times
\text{Original Area}
\]

---

# Example 1

Scaling Matrix

\[
\begin{bmatrix}
2 & 0\\
0 & 3
\end{bmatrix}
\]

---

Determinant:

\[
2\times3
=
6
\]

---

Interpretation:

Area becomes:

\[
6
\]

times larger.

---

# Example 2

Matrix

\[
\begin{bmatrix}
0.5 & 0\\
0 & 0.5
\end{bmatrix}
\]

---

Determinant:

\[
0.25
\]

---

Area becomes:

25%

of original.

---

# Example 3

Reflection Matrix

\[
\begin{bmatrix}
1 & 0\\
0 & -1
\end{bmatrix}
\]

---

Determinant:

\[
-1
\]

---

Meaning:

Area unchanged.

Orientation reversed.

---

# Important Interpretations

### Determinant > 1

Area increases.

---

### Determinant between 0 and 1

Area decreases.

---

### Determinant = 1

Area unchanged.

---

### Determinant = 0

Area collapses.

Shape becomes a line or point.

---

### Determinant < 0

Orientation flips.

Reflection occurs.

---

# Complete Big Picture

## Geometric Transformations

Matrices can transform shapes mathematically.

---

## Reflection

Mirror image transformation.

Examples:

- Mirrors
- Graphics
- Symmetry

---

## Rotation

Turns an object around a fixed point.

Examples:

- Wheels
- Clocks
- Camera movement

---

## Shearing

Slants an object.

Examples:

- Italic text
- Perspective effects

---

## Scaling

Changes size.

Examples:

- Zooming
- Resizing images
- Enlarging maps

---

## Shape Representation

Vertices stored as columns inside a matrix.

Allows entire shapes to be transformed with one matrix multiplication.

---

## General Scaling Matrix

\[
\begin{bmatrix}
s_x & 0\\
0 & s_y
\end{bmatrix}
\]

---

## Determinant

Measures area scaling.

\[
det(A)
=
\text{Area Scale Factor}
\]

---

These ideas form the mathematical foundation for:

- Computer Graphics
- Animation
- Robotics
- Computer Vision
- CAD Software
- Game Engines
- Augmented Reality (AR)
- Virtual Reality (VR)
- Machine Learning
- Neural Networks
- Large Language Models (LLMs)

where matrices continuously transform vectors and geometric spaces.