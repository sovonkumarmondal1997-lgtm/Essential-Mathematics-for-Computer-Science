# Identity Matrices, Determinants, and Matrix Inverses

---

# Introduction

In previous chapters, we learned:

- Vectors
- Dot Product
- Cross Product
- Matrices
- Matrix Addition
- Matrix Multiplication
- Gaussian Elimination

Now we will learn one of the most important topics in Linear Algebra:

- Identity Elements
- Identity Matrices
- Determinants
- Matrix Inverses

These concepts are heavily used in:

- Computer Graphics
- Robotics
- Engineering
- Physics
- Machine Learning
- Deep Learning
- Computer Vision
- Large Language Models (LLMs)

---

# 1. Identity Element (in Multiplication)

## Simple Definition

An **Identity Element** is a value that leaves another value unchanged when an operation is performed.

For multiplication, the identity element is:

\[
1
\]

because:

\[
n \times 1 = n
\]

for any number \(n\).

---

## Example 1

\[
5 \times 1 = 5
\]

Nothing changes.

---

## Example 2

\[
100 \times 1 = 100
\]

Still unchanged.

---

## Example 3

\[
-7 \times 1 = -7
\]

Again unchanged.

---

## Real-Life Analogy

Imagine a photocopier that makes an exact copy without altering anything.

Multiplying by 1 works similarly.

---

# Why It Matters

Identity elements appear everywhere:

- Numbers → 1
- Matrices → Identity Matrix
- Programming → Neutral values
- Algebra → Fundamental structures

---

# 2. Identity Matrix (2×2)

## Simple Definition

The **Identity Matrix** is the matrix version of the number 1.

For a 2×2 matrix:

\[
I=
\begin{bmatrix}
1 & 0\\
0 & 1
\end{bmatrix}
\]

---

## Why These Numbers?

The diagonal contains:

\[
1
\]

Everything else is:

\[
0
\]

---

## Example 1

Let

\[
A=
\begin{bmatrix}
2 & 3\\
4 & 5
\end{bmatrix}
\]

Multiply:

\[
AI
\]

Result:

\[
A
\]

unchanged.

---

## Example 2

\[
IA=A
\]

also unchanged.

---

## Example 3

\[
\begin{bmatrix}
10 & 20\\
30 & 40
\end{bmatrix}
I
=
\begin{bmatrix}
10 & 20\\
30 & 40
\end{bmatrix}
\]

---

## Real-Life Analogy

Identity Matrix is like multiplying by 1.

Nothing changes.

---

# 3. Inverse of a Number (Multiplicative Inverse)

## Simple Definition

The inverse of a number is the value that produces 1 when multiplied by the original number.

---

## Formula

For any non-zero number:

\[
n^{-1}
=
\frac{1}{n}
\]

---

## Example 1

\[
5^{-1}
=
\frac{1}{5}
\]

Check:

\[
5 \times \frac{1}{5}
=
1
\]

---

## Example 2

\[
2^{-1}
=
\frac{1}{2}
\]

\[
2 \times \frac12
=
1
\]

---

## Example 3

\[
10^{-1}
=
0.1
\]

\[
10 \times 0.1
=
1
\]

---

## Important Observation

Zero has no inverse.

Why?

Because:

\[
0\times x=0
\]

never becomes 1.

---

# 4. Inverse Matrix (2×2)

## Simple Definition

The inverse matrix plays the same role for matrices that reciprocals play for numbers.

---

For numbers:

\[
5\times\frac15=1
\]

For matrices:

\[
AA^{-1}=I
\]

---

## Meaning

Multiplying a matrix by its inverse produces the identity matrix.

---

## Example

Suppose:

\[
A=
\begin{bmatrix}
1 & 2\\
3 & 4
\end{bmatrix}
\]

Its inverse is:

\[
A^{-1}
=
\begin{bmatrix}
-2 & 1\\
1.5 & -0.5
\end{bmatrix}
\]

Then:

\[
AA^{-1}
=
I
\]

---

## Why Useful?

Matrix inverses help solve:

\[
AX=B
\]

similar to:

\[
5x=20
\]

---

# Number Version

\[
x=\frac{20}{5}
\]

---

# Matrix Version

\[
X=A^{-1}B
\]

---

# 5. Determinant of a Matrix (2×2)

## Simple Definition

The determinant is a special number associated with a square matrix.

For:

\[
A=
\begin{bmatrix}
a & b\\
c & d
\end{bmatrix}
\]

---

Formula:

\[
det(A)=ad-bc
\]

---

## Example 1

\[
\begin{bmatrix}
1 & 2\\
3 & 4
\end{bmatrix}
\]

---

Compute:

\[
(1)(4)-(2)(3)
\]

\[
=4-6
\]

\[
=-2
\]

---

## Example 2

\[
\begin{bmatrix}
5 & 1\\
2 & 3
\end{bmatrix}
\]

---

\[
(5)(3)-(1)(2)
\]

\[
15-2
\]

\[
=13
\]

---

## Example 3

\[
\begin{bmatrix}
2 & 4\\
1 & 2
\end{bmatrix}
\]

---

\[
(2)(2)-(4)(1)
\]

\[
4-4
\]

\[
=0
\]

---

# Why Determinants Matter

Determinants tell us:

- Whether an inverse exists
- Whether information is lost
- Area scaling
- Volume scaling

---

# 6. Invertibility Condition

## Simple Definition

A matrix can have an inverse only when:

\[
det(A)\ne0
\]

---

## Rule

### If

\[
det(A)\ne0
\]

Inverse exists.

---

### If

\[
det(A)=0
\]

Inverse does NOT exist.

---

## Example 1

\[
\begin{bmatrix}
1 & 2\\
3 & 4
\end{bmatrix}
\]

Determinant:

\[
-2
\]

Inverse exists.

---

## Example 2

\[
\begin{bmatrix}
2 & 4\\
1 & 2
\end{bmatrix}
\]

Determinant:

\[
0
\]

Inverse does not exist.

---

## Memory Trick

```
Non-zero determinant
      ↓
Inverse Exists

Zero determinant
      ↓
No Inverse
```

---

# 7. Leading Diagonal (Main Diagonal)

## Simple Definition

The leading diagonal runs:

Top-left

to

Bottom-right.

---

## Example

\[
\begin{bmatrix}
1 & 2 & 3\\
4 & 5 & 6\\
7 & 8 & 9
\end{bmatrix}
\]

Leading diagonal:

\[
1,\;5,\;9
\]

---

## Example 2

\[
\begin{bmatrix}
8 & 1\\
3 & 7
\end{bmatrix}
\]

Leading diagonal:

\[
8,\;7
\]

---

## Visual

```
[ X  .  . ]
[ .  X  . ]
[ .  .  X ]
```

X marks the leading diagonal.

---

# Why Important?

Identity matrices place all their 1s on this diagonal.

---

# 8. Matrix Inverse Formula (2×2)

## Original Matrix

\[
A=
\begin{bmatrix}
a & b\\
c & d
\end{bmatrix}
\]

---

## Determinant

\[
det(A)=ad-bc
\]

---

## Inverse Formula

\[
A^{-1}
=
\frac{1}{ad-bc}
\begin{bmatrix}
d & -b\\
-c & a
\end{bmatrix}
\]

---

# Easy Memory Trick

Step 1:

Swap diagonal values.

\[
a \leftrightarrow d
\]

---

Step 2:

Change signs of remaining values.

\[
b \to -b
\]

\[
c \to -c
\]

---

Step 3:

Divide everything by determinant.

---

## Example

\[
A=
\begin{bmatrix}
2 & 1\\
3 & 4
\end{bmatrix}
\]

---

Determinant:

\[
(2)(4)-(1)(3)
\]

\[
8-3=5
\]

---

Swap diagonal:

\[
\begin{bmatrix}
4 & 1\\
3 & 2
\end{bmatrix}
\]

---

Change signs:

\[
\begin{bmatrix}
4 & -1\\
-3 & 2
\end{bmatrix}
\]

---

Divide by 5:

\[
A^{-1}
=
\frac15
\begin{bmatrix}
4 & -1\\
-3 & 2
\end{bmatrix}
\]

---

# 9. Identity Matrix (3×3)

## Simple Definition

The 3×3 identity matrix extends the same idea.

---

\[
I=
\begin{bmatrix}
1 & 0 & 0\\
0 & 1 & 0\\
0 & 0 & 1
\end{bmatrix}
\]

---

## Pattern

Leading diagonal:

\[
1,1,1
\]

Everything else:

\[
0
\]

---

## Example

\[
AI=A
\]

for every compatible 3×3 matrix.

---

## Visual

```
[1 0 0]
[0 1 0]
[0 0 1]
```

---

# 10. Inverse of a 3×3 Matrix

## Simple Definition

The inverse of a 3×3 matrix exists when:

\[
det(A)\ne0
\]

---

Unlike 2×2 matrices,

there is no simple swap-and-sign formula.

---

## General Process

1. Compute determinant
2. Find minors
3. Find cofactors
4. Build cofactor matrix
5. Transpose it
6. Divide by determinant

---

## Example

\[
A=
\begin{bmatrix}
1 & 2 & 3\\
0 & 1 & 4\\
5 & 6 & 0
\end{bmatrix}
\]

Inverse exists because determinant is non-zero.

---

## Why It Is Difficult

A 2×2 inverse needs only a few steps.

A 3×3 inverse requires many calculations.

---

## Real-Life Use

3D graphics transformations.

Robotics.

Physics simulations.

Neural network computations.

---

# 11. Geometric Transformations via Matrices

## Simple Definition

Matrices can transform shapes and points.

---

Common transformations:

- Scaling
- Rotation
- Reflection
- Shearing

---

# Example 1: Scaling

Point:

\[
(2,3)
\]

Scaling Matrix:

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

# Example 2: Shrinking

Scaling Matrix:

\[
\begin{bmatrix}
0.5 & 0\\
0 & 0.5
\end{bmatrix}
\]

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

Point:

\[
(1,0)
\]

Rotate 90°

Result:

\[
(0,1)
\]

---

# Example 4: Reflection

Reflect across x-axis.

Point:

\[
(2,3)
\]

Becomes:

\[
(2,-3)
\]

---

# Example 5: Computer Graphics

Every moving object in a video game is transformed using matrices.

---

# Example 6: Robotics

Robot arm movements are computed through matrix transformations.

---

# Complete Big Picture

## Identity Element

\[
1
\]

Leaves numbers unchanged.

---

## Identity Matrix

\[
I
\]

Leaves matrices unchanged.

---

## Multiplicative Inverse

\[
n^{-1}
=
\frac1n
\]

---

## Matrix Inverse

\[
AA^{-1}=I
\]

---

## Determinant

For:

\[
\begin{bmatrix}
a & b\\
c & d
\end{bmatrix}
\]

\[
det(A)=ad-bc
\]

---

## Invertibility Condition

\[
det(A)\ne0
\]

---

## Main Diagonal

Top-left to bottom-right.

---

## 2×2 Inverse Formula

\[
A^{-1}
=
\frac{1}{ad-bc}
\begin{bmatrix}
d & -b\\
-c & a
\end{bmatrix}
\]

---

## 3×3 Identity Matrix

\[
\begin{bmatrix}
1&0&0\\
0&1&0\\
0&0&1
\end{bmatrix}
\]

---

## Geometric Transformations

Matrices can:

- Rotate
- Scale
- Reflect
- Transform

objects in 2D and 3D spaces.

---

These concepts form the foundation for:

- Linear Algebra
- Computer Graphics
- Computer Vision
- Robotics
- Data Science
- Machine Learning
- Deep Learning
- Neural Networks
- Transformers
- Embeddings
- Large Language Models (LLMs)

where matrix multiplication and matrix inverses are used extensively.