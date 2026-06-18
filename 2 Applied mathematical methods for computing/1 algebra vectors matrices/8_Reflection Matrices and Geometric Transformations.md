# Reflection Matrices and Geometric Transformations

---

# Introduction

In previous chapters, we learned:

- Vectors
- Matrices
- Matrix Multiplication
- Determinants
- Matrix Inverses
- Scaling
- Rotation
- Shearing

Now we will study one of the most important geometric transformations:

# Reflection

Reflection creates a mirror image of an object.

Reflection matrices are widely used in:

- Computer Graphics
- Video Games
- Animation
- Robotics
- CAD Software
- Computer Vision
- Image Processing

---

# 1. Reflection Matrices

## Simple Definition

A **Reflection Matrix** is a special matrix that flips points across a line.

Think of a mirror.

Whatever is on one side appears symmetrically on the other side.

---

## General Idea

Original Point:

\[
P=
\begin{bmatrix}
x\\
y
\end{bmatrix}
\]

Reflection Matrix:

\[
R
\]

New Point:

\[
P'
=
RP
\]

---

## Visual Example

Before Reflection:

```
        ●
      (3,2)

|
|
| Mirror Line
|
|

```

After Reflection:

```
●
(-3,2)

|
|
| Mirror Line
|
|

```

---

## Real-Life Examples

### Example 1

Looking into a mirror.

---

### Example 2

Image editing software.

"Flip Horizontally"

---

### Example 3

Video game character turns from:

```
→
```

to

```
←
```

using reflection.

---

# Why Reflection Matrices Matter

They allow computers to:

- Flip images
- Create symmetry
- Build animations
- Perform geometric calculations

using simple matrix multiplication.

---

# 2. Reflection in the Y-Axis

## Reflection Matrix

\[
R_y=
\begin{bmatrix}
-1 & 0\\
0 & 1
\end{bmatrix}
\]

---

## What Happens?

Only x-coordinate changes sign.

\[
(x,y)
\rightarrow
(-x,y)
\]

---

## Example 1

Point:

\[
(3,2)
\]

Apply matrix:

\[
\begin{bmatrix}
-1 & 0\\
0 & 1
\end{bmatrix}
\begin{bmatrix}
3\\
2
\end{bmatrix}
=
\begin{bmatrix}
-3\\
2
\end{bmatrix}
\]

---

## Example 2

\[
(5,-4)
\]

becomes

\[
(-5,-4)
\]

---

## Example 3

\[
(-2,7)
\]

becomes

\[
(2,7)
\]

---

## Visual

Before:

```
      ● (3,2)

----------- y-axis -----------

```

After:

```
● (-3,2)

----------- y-axis -----------

```

---

## Memory Trick

Reflection in y-axis:

```
Change x
Keep y
```

---

# 3. Reflection in the X-Axis

## Reflection Matrix

\[
R_x=
\begin{bmatrix}
1 & 0\\
0 & -1
\end{bmatrix}
\]

---

## What Happens?

Only y-coordinate changes sign.

\[
(x,y)
\rightarrow
(x,-y)
\]

---

## Example 1

\[
(3,2)
\]

becomes

\[
(3,-2)
\]

---

## Example 2

\[
(-4,5)
\]

becomes

\[
(-4,-5)
\]

---

## Example 3

\[
(7,-3)
\]

becomes

\[
(7,3)
\]

---

## Visual

Before:

```
      ● (3,2)

---------------- x-axis

```

After:

```
---------------- x-axis

      ● (3,-2)

```

---

## Memory Trick

Reflection in x-axis:

```
Keep x
Change y
```

---

# 4. Reflection in the Line y = x

## Reflection Matrix

\[
R=
\begin{bmatrix}
0 & 1\\
1 & 0
\end{bmatrix}
\]

---

## What Happens?

Coordinates swap places.

\[
(x,y)
\rightarrow
(y,x)
\]

---

## Example 1

\[
(2,5)
\]

becomes

\[
(5,2)
\]

---

## Example 2

\[
(7,1)
\]

becomes

\[
(1,7)
\]

---

## Example 3

\[
(-3,4)
\]

becomes

\[
(4,-3)
\]

---

## Visual

Line:

\[
y=x
\]

```
       /
      /
     /
    /
   /

```

Reflection swaps horizontal and vertical distances.

---

## Memory Trick

Reflection across \(y=x\):

```
Swap x and y
```

---

# 5. Reflection in the Line y = -x

## Reflection Matrix

\[
R=
\begin{bmatrix}
0 & -1\\
-1 & 0
\end{bmatrix}
\]

---

## What Happens?

Swap coordinates.

Then change both signs.

\[
(x,y)
\rightarrow
(-y,-x)
\]

---

## Example 1

\[
(2,5)
\]

becomes

\[
(-5,-2)
\]

---

## Example 2

\[
(4,-1)
\]

becomes

\[
(1,-4)
\]

---

## Example 3

\[
(-2,3)
\]

becomes

\[
(-3,2)
\]

---

## Visual

Reflection line:

\[
y=-x
\]

```
\
 \
  \
   \
    \

```

---

## Memory Trick

Reflection across \(y=-x\):

```
Swap coordinates
Change both signs
```

---

# 6. Determinant of Isometric Transformations

## Simple Definition

An **Isometric Transformation** preserves size.

Examples:

- Reflection
- Rotation

---

## Important Rule

Reflections do NOT change area.

Therefore:

\[
|det(R)|=1
\]

---

## Example 1

Reflection in y-axis:

\[
\begin{bmatrix}
-1 & 0\\
0 & 1
\end{bmatrix}
\]

Determinant:

\[
(-1)(1)-0
=
-1
\]

---

## Example 2

Reflection in x-axis:

\[
\begin{bmatrix}
1 & 0\\
0 & -1
\end{bmatrix}
\]

Determinant:

\[
-1
\]

---

## Example 3

Reflection in \(y=x\):

\[
\begin{bmatrix}
0 & 1\\
1 & 0
\end{bmatrix}
\]

Determinant:

\[
-1
\]

---

## Interpretation

Area remains unchanged.

Orientation flips.

---

## Visual Analogy

A mirror image:

- Same size
- Opposite orientation

---

# 7. Self-Inverse Matrices

## Simple Definition

Some transformations undo themselves when applied twice.

These matrices are called:

**Self-Inverse Matrices**

---

## Rule

\[
A^{-1}=A
\]

or

\[
AA=I
\]

---

## Meaning

Apply transformation:

Once → reflected.

Twice → original object returns.

---

## Example 1

Reflection in x-axis.

First reflection:

\[
(3,2)
\rightarrow
(3,-2)
\]

Second reflection:

\[
(3,-2)
\rightarrow
(3,2)
\]

Back to original.

---

## Example 2

Reflection in y-axis.

Apply twice.

Original position returns.

---

## Example 3

Mirror image.

Looking at your reflection in another mirror facing the first.

The image returns to original orientation.

---

# Why?

Because reflection reverses itself.

---

# 8. Identity Matrix Connection

## Rule

For reflection matrices:

\[
R^2=I
\]

---

## Example

Reflection in x-axis:

\[
R=
\begin{bmatrix}
1 & 0\\
0 & -1
\end{bmatrix}
\]

Multiply:

\[
RR
\]

---

Result:

\[
\begin{bmatrix}
1 & 0\\
0 & 1
\end{bmatrix}
\]

---

This is:

\[
I
\]

---

## Interpretation

Reflecting twice equals doing nothing.

---

## Example 2

Reflection in y-axis.

Same result.

---

## Example 3

Reflection in \(y=x\).

Again:

\[
R^2=I
\]

---

# Visual Idea

```
Original
   ↓
Reflection
   ↓
Reflection Again
   ↓
Original
```

---

# 9. Vertex Matrix Transformation

## Simple Definition

A shape can be represented using a matrix of vertices.

Each column stores one point.

---

# Example Triangle

Vertices:

\[
(0,0)
\]

\[
(2,0)
\]

\[
(1,3)
\]

---

Vertex Matrix:

\[
T=
\begin{bmatrix}
0 & 2 & 1\\
0 & 0 & 3
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
(1,3)
\]

---

# Reflection Example

Reflection in y-axis:

\[
R=
\begin{bmatrix}
-1 & 0\\
0 & 1
\end{bmatrix}
\]

---

Transform:

\[
RT
\]

---

Result:

\[
\begin{bmatrix}
0 & -2 & -1\\
0 & 0 & 3
\end{bmatrix}
\]

---

New vertices:

\[
(0,0)
\]

\[
(-2,0)
\]

\[
(-1,3)
\]

---

Entire triangle reflected at once.

---

# Example 2

Reflect a square.

All four vertices transform simultaneously.

---

# Example 3

Video game sprite.

Thousands of points transform through one matrix multiplication.

---

# Why This Is Powerful

Instead of transforming:

```
Point 1
Point 2
Point 3
Point 4
...
```

individually,

we transform the whole shape using:

\[
RT
\]

---

# Complete Big Picture

## Reflection Matrices

Create mirror images.

---

## Reflection in Y-Axis

\[
\begin{bmatrix}
-1 & 0\\
0 & 1
\end{bmatrix}
\]

Changes x sign.

---

## Reflection in X-Axis

\[
\begin{bmatrix}
1 & 0\\
0 & -1
\end{bmatrix}
\]

Changes y sign.

---

## Reflection in \(y=x\)

\[
\begin{bmatrix}
0 & 1\\
1 & 0
\end{bmatrix}
\]

Swaps coordinates.

---

## Reflection in \(y=-x\)

\[
\begin{bmatrix}
0 & -1\\
-1 & 0
\end{bmatrix}
\]

Swaps coordinates and changes signs.

---

## Determinants

Reflection matrices satisfy:

\[
|det(R)|=1
\]

Area preserved.

---

## Self-Inverse Property

\[
R^{-1}=R
\]

---

## Identity Connection

\[
R^2=I
\]

Reflect twice.

Return to original.

---

## Vertex Matrix Transformations

Entire shapes can be transformed using one matrix multiplication.

---

These concepts form the foundation for:

- Computer Graphics
- CAD Software
- Robotics
- Animation
- Computer Vision
- Video Games
- Geometry Processing
- Image Manipulation
- Machine Learning
- Neural Networks
- Scientific Simulations

where geometric transformations are performed millions of times per second.