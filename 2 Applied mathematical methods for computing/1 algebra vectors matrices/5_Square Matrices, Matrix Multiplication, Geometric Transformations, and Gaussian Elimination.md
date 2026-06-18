# Square Matrices, Matrix Multiplication, Geometric Transformations, and Gaussian Elimination

---

# Introduction

In the previous chapter, we learned:

- Matrices
- Rows and Columns
- Matrix Dimensions
- Matrix Addition
- Scalar Multiplication
- Matrix Multiplication
- Identity Matrix

Now we will go deeper into:

- Square Matrices
- Commutativity and Non-Commutativity
- Proof by Counterexample
- Matrix Multiplication Algorithms
- Geometric Transformations
- Gaussian Elimination

These concepts form the foundation of:

- Computer Graphics
- Machine Learning
- Robotics
- Computer Vision
- Engineering
- Large Language Models (LLMs)

---

# 1. Square Matrices

## Simple Definition

A **Square Matrix** is a matrix that has:

\[
\text{Number of Rows}
=
\text{Number of Columns}
\]

In other words:

\[
n \times n
\]

---

## Examples of Square Matrices

### 2 × 2 Matrix

\[
A=
\begin{bmatrix}
1 & 2\\
3 & 4
\end{bmatrix}
\]

Rows = 2

Columns = 2

Square Matrix ✔

---

### 3 × 3 Matrix

\[
B=
\begin{bmatrix}
1 & 2 & 3\\
4 & 5 & 6\\
7 & 8 & 9
\end{bmatrix}
\]

Rows = 3

Columns = 3

Square Matrix ✔

---

### 4 × 4 Matrix

\[
C=
\begin{bmatrix}
1 & 0 & 0 & 0\\
0 & 1 & 0 & 0\\
0 & 0 & 1 & 0\\
0 & 0 & 0 & 1
\end{bmatrix}
\]

Rows = 4

Columns = 4

Square Matrix ✔

---

## Not Square

### 2 × 3 Matrix

\[
\begin{bmatrix}
1 & 2 & 3\\
4 & 5 & 6
\end{bmatrix}
\]

Rows = 2

Columns = 3

Not Square ✘

---

## Real-Life Example

Imagine a table showing distances between cities:

|     | A | B | C |
|-----|---|---|---|
| A | 0 | 5 | 10 |
| B | 5 | 0 | 7 |
| C |10 | 7 | 0 |

Three rows.

Three columns.

This is a 3×3 square matrix.

---

# Why Square Matrices Matter

Most advanced matrix operations require square matrices:

- Determinants
- Inverse Matrices
- Eigenvalues
- Eigenvectors

---

# 2. Matrix Addition

## Simple Definition

Matrix addition means:

Add corresponding elements.

---

## Rule

Matrices must have the same dimensions.

---

## Example 1

\[
A=
\begin{bmatrix}
1 & 2\\
3 & 4
\end{bmatrix}
\]

\[
B=
\begin{bmatrix}
5 & 6\\
7 & 8
\end{bmatrix}
\]

---

Add element-by-element:

\[
A+B=
\begin{bmatrix}
1+5 & 2+6\\
3+7 & 4+8
\end{bmatrix}
\]

---

Result:

\[
=
\begin{bmatrix}
6 & 8\\
10 & 12
\end{bmatrix}
\]

---

## Example 2

Temperature Data

Monday:

\[
\begin{bmatrix}
20 & 25\\
18 & 22
\end{bmatrix}
\]

Tuesday:

\[
\begin{bmatrix}
2 & 3\\
1 & 4
\end{bmatrix}
\]

Combined:

\[
\begin{bmatrix}
22 & 28\\
19 & 26
\end{bmatrix}
\]

---

## Example 3

Image Processing

Two images:

```
Image A + Image B
```

Pixel-by-pixel addition.

---

# Important Property

Matrix addition IS commutative.

\[
A+B=B+A
\]

---

# Example

\[
2+5=5+2
\]

Similarly:

\[
A+B=B+A
\]

---

# 3. Commutativity vs Non-Commutativity

## What is Commutativity?

Operation where order does not matter.

---

## Formula

\[
A+B=B+A
\]

---

## Example 1

Numbers

\[
3+5=5+3
\]

---

## Example 2

Multiplication

\[
2\times4=4\times2
\]

---

## Example 3

Matrix Addition

\[
A+B=B+A
\]

---

# Non-Commutativity

Order changes the result.

---

## Example

Putting on:

- Socks
- Shoes

Works.

---

Reverse order:

- Shoes
- Socks

Does not work.

Order matters.

---

## Matrix Multiplication

Generally:

\[
AB\ne BA
\]

---

# Example

\[
A=
\begin{bmatrix}
1 & 2
\end{bmatrix}
\]

\[
B=
\begin{bmatrix}
3\\
4
\end{bmatrix}
\]

---

### AB

\[
(1\times2)(2\times1)
\]

Result:

\[
1\times1
\]

---

### BA

\[
(2\times1)(1\times2)
\]

Result:

\[
2\times2
\]

---

Different matrices.

Therefore:

\[
AB\ne BA
\]

---

# 4. Proof by Counterexample

## Simple Definition

To prove a statement is FALSE,

you only need ONE example where it fails.

This is called a:

**Counterexample**

---

# Statement

"All matrix multiplication is commutative."

Meaning:

\[
AB=BA
\]

for every matrix.

---

# Counterexample

Let

\[
A=
\begin{bmatrix}
1 & 1\\
0 & 0
\end{bmatrix}
\]

---

\[
B=
\begin{bmatrix}
1 & 0\\
1 & 0
\end{bmatrix}
\]

---

## Compute AB

\[
AB=
\begin{bmatrix}
2 & 0\\
0 & 0
\end{bmatrix}
\]

---

## Compute BA

\[
BA=
\begin{bmatrix}
1 & 1\\
1 & 1
\end{bmatrix}
\]

---

Clearly:

\[
AB\ne BA
\]

---

Therefore:

The statement is false.

One counterexample is enough.

---

# Real-Life Example

Statement:

"All birds can fly."

Counterexample:

Penguin.

Statement immediately becomes false.

---

# 5. Matrix Multiplication Algorithmic Process

## Simple Definition

Matrix multiplication follows a fixed procedure.

Every entry is obtained by:

\[
Row \cdot Column
\]

(dot product)

---

# Example

Multiply

\[
A=
\begin{bmatrix}
1 & 2 & 3\\
4 & 5 & 6\\
7 & 8 & 9
\end{bmatrix}
\]

by

\[
B=
\begin{bmatrix}
1 & 0 & 2\\
0 & 1 & 3\\
4 & 5 & 6
\end{bmatrix}
\]

---

# Step 1

First entry

Row 1 × Column 1

\[
(1,2,3)
\cdot
(1,0,4)
\]

---

Compute:

\[
1(1)+2(0)+3(4)
\]

\[
=13
\]

---

# Step 2

First row × second column

\[
(1,2,3)
\cdot
(0,1,5)
\]

\[
=17
\]

---

# Step 3

Continue until every position is filled.

---

Result becomes another 3×3 matrix.

---

## Memory Trick

```
Row → Across

Column ↓ Down

```

Every answer comes from:

```
Row × Column
```

---

# 6. Geometric Transformations via Matrices

## Simple Definition

Matrices can move and transform objects.

---

Examples:

- Rotate
- Stretch
- Shrink
- Reflect
- Move

---

# Example 1: Scaling

Original point:

\[
(2,3)
\]

---

Scaling matrix:

\[
\begin{bmatrix}
2 & 0\\
0 & 2
\end{bmatrix}
\]

---

Result:

\[
(4,6)
\]

Everything doubles.

---

# Example 2: Shrinking

Scaling matrix:

\[
\begin{bmatrix}
0.5 & 0\\
0 & 0.5
\end{bmatrix}
\]

---

Point:

\[
(4,8)
\]

Result:

\[
(2,4)
\]

---

# Example 3: Rotation

Rotate 90°

Original point:

\[
(1,0)
\]

After rotation:

\[
(0,1)
\]

---

# Real-Life Uses

Computer Games

```
Character movement
Camera movement
Object rotation
```

All performed using matrices.

---

# Example 4: 3D Animation

Movies like:

- Toy Story
- Frozen
- Avatar

depend heavily on matrix transformations.

---

# Example 5: Robotics

Robot arm movement.

Every joint rotation uses matrices.

---

# Why AI Uses Matrix Transformations

Neural Networks:

\[
Output = WX+b
\]

where:

- W = Matrix
- X = Input Vector

Every prediction involves matrix transformations.

---

# 7. Gaussian Elimination

## Simple Definition

Gaussian Elimination is a systematic method for solving equations.

---

# Example Problem

Solve:

\[
x+y=5
\]

\[
x-y=1
\]

---

# Step 1

Write as matrix:

\[
\begin{bmatrix}
1 & 1 & 5\\
1 & -1 & 1
\end{bmatrix}
\]

---

This is called an:

Augmented Matrix

---

# Step 2

Subtract Row 1 from Row 2

\[
R_2-R_1
\]

---

New matrix:

\[
\begin{bmatrix}
1 & 1 & 5\\
0 & -2 & -4
\end{bmatrix}
\]

---

# Step 3

Solve second row

\[
-2y=-4
\]

\[
y=2
\]

---

# Step 4

Substitute into first row

\[
x+2=5
\]

\[
x=3
\]

---

Final Solution

\[
x=3
\]

\[
y=2
\]

---

# Real-Life Example

Suppose:

A shop sells:

- Apples
- Oranges

Given:

\[
Apple + Orange = 5
\]

\[
Apple - Orange = 1
\]

Gaussian elimination finds individual values.

---

# Why Gaussian Elimination Matters

Used in:

- Engineering
- Physics
- Economics
- Statistics
- Data Science
- Machine Learning

Whenever large systems of equations must be solved.

---

# Complete Big Picture

## Square Matrix

\[
n\times n
\]

Same number of rows and columns.

---

## Matrix Addition

Add matching entries.

\[
A+B
\]

Requires same dimensions.

---

## Commutativity

Order does not matter.

\[
A+B=B+A
\]

---

## Non-Commutativity

Order matters.

\[
AB\ne BA
\]

in general.

---

## Counterexample

One valid example that disproves a statement.

---

## Matrix Multiplication

Every element is:

\[
Row\cdot Column
\]

---

## Geometric Transformations

Matrices can:

- Rotate
- Scale
- Reflect
- Transform

objects in 2D and 3D space.

---

## Gaussian Elimination

A systematic technique for solving systems of equations using row operations.

---

These ideas form the foundation for:

- Determinants
- Matrix Inverses
- Linear Systems
- Eigenvalues
- Eigenvectors
- Singular Value Decomposition (SVD)
- Principal Component Analysis (PCA)
- Machine Learning
- Deep Learning
- Neural Networks
- Transformers
- Large Language Models (LLMs)

where billions of matrix operations are performed every second.