# Matrices Fundamentals

---

# Introduction

So far, we have learned:

- Scalars
- Vectors
- Dot Products
- Cross Products

Vectors store data in a single row or column.

But in real-world applications, we often need to store **many vectors together**.

This is where **Matrices** come into play.

Matrices are one of the most important concepts in:

- Linear Algebra
- Computer Graphics
- Data Science
- Machine Learning
- Deep Learning
- Computer Vision
- Robotics
- Recommendation Systems
- Large Language Models (LLMs)

---

# 1. Matrix / Matrices

## Simple Definition

A **Matrix** is a rectangular arrangement of numbers organized into:

- Rows
- Columns

A single matrix is called a **Matrix**.

Multiple matrices are called **Matrices**.

---

## Example 1

\[
A=
\begin{bmatrix}
1 & 2\\
3 & 4
\end{bmatrix}
\]

This matrix contains:

- 2 rows
- 2 columns

---

## Example 2

Student Marks

\[
\begin{bmatrix}
80 & 90 & 85\\
75 & 88 & 92
\end{bmatrix}
\]

Rows:

- Students

Columns:

- Subjects

---

## Example 3

Image Representation

A grayscale image:

\[
\begin{bmatrix}
0 & 255 & 100\\
50 & 120 & 220\\
10 & 90 & 255
\end{bmatrix}
\]

Each number represents pixel brightness.

---

# Why Matrices Matter

Imagine a classroom.

| Student | Math | Physics | Chemistry |
|----------|---------|---------|---------|
| John | 80 | 90 | 85 |
| Alice | 70 | 88 | 92 |

The table itself is a matrix.

---

# 2. Matrix Dimensions / Order

## Simple Definition

The size of a matrix is determined by:

\[
Rows \times Columns
\]

---

## General Form

\[
n \times m
\]

where:

- n = rows
- m = columns

---

## Example 1

\[
\begin{bmatrix}
1 & 2\\
3 & 4
\end{bmatrix}
\]

Dimension:

\[
2 \times 2
\]

---

## Example 2

\[
\begin{bmatrix}
1 & 2 & 3
\end{bmatrix}
\]

Dimension:

\[
1 \times 3
\]

---

## Example 3

\[
\begin{bmatrix}
1\\
2\\
3
\end{bmatrix}
\]

Dimension:

\[
3 \times 1
\]

---

## Memory Trick

```
Rows × Columns

```

Always count rows first.

Then columns.

---

# 3. Rows and Columns

## Rows

Rows run horizontally.

---

### Example

\[
\begin{bmatrix}
1 & 2 & 3\\
4 & 5 & 6
\end{bmatrix}
\]

Row 1:

\[
(1,2,3)
\]

Row 2:

\[
(4,5,6)
\]

---

## Columns

Columns run vertically.

---

Column 1:

\[
\begin{bmatrix}
1\\
4
\end{bmatrix}
\]

Column 2:

\[
\begin{bmatrix}
2\\
5
\end{bmatrix}
\]

Column 3:

\[
\begin{bmatrix}
3\\
6
\end{bmatrix}
\]

---

## Real-Life Example

Spreadsheet:

| Name | Age | Salary |
|--------|--------|--------|
| John | 25 | 50000 |
| Alice | 30 | 70000 |

Rows = people

Columns = attributes

---

# 4. Matrix Addition

## Simple Definition

To add two matrices:

Add corresponding elements.

---

## Rule

Matrices must have the same dimensions.

---

### Valid Example

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

Add:

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

## Invalid Example

\[
2\times2
+
3\times2
\]

Cannot be added.

Different dimensions.

---

## Real-Life Example

Monthly sales tables.

January sales matrix +

February sales matrix

=

Combined sales matrix.

---

# 5. Scalar Multiplication of a Matrix

## Simple Definition

Multiply every element by the same number.

That number is called a scalar.

---

## Example 1

\[
2
\begin{bmatrix}
1 & 2\\
3 & 4
\end{bmatrix}
\]

---

Multiply every entry:

\[
=
\begin{bmatrix}
2 & 4\\
6 & 8
\end{bmatrix}
\]

---

## Example 2

\[
5
\begin{bmatrix}
1 & 3
\end{bmatrix}
\]

---

Result:

\[
\begin{bmatrix}
5 & 15
\end{bmatrix}
\]

---

## Real-Life Example

Salary Increase

Original salaries:

\[
\begin{bmatrix}
50000\\
60000\\
70000
\end{bmatrix}
\]

10% increase:

Multiply by:

\[
1.1
\]

---

# 6. Matrix Multiplication

## Simple Definition

Matrix multiplication combines information from two matrices.

Unlike addition:

Dimensions do NOT need to be identical.

Instead:

A special rule must be satisfied.

---

## Rule

Number of columns in first matrix

must equal

Number of rows in second matrix.

---

## Example

\[
A=
\begin{bmatrix}
1 & 2
\end{bmatrix}
\]

Dimension:

\[
1\times2
\]

---

\[
B=
\begin{bmatrix}
3\\
4
\end{bmatrix}
\]

Dimension:

\[
2\times1
\]

---

Multiplication is possible because:

\[
2=2
\]

---

# 7. Resulting Dimension of Matrix Multiplication

## General Rule

\[
(m\times n)
\times
(n\times p)
=
(m\times p)
\]

---

## Example 1

\[
(2\times3)
\times
(3\times4)
\]

Result:

\[
2\times4
\]

---

## Example 2

\[
(5\times2)
\times
(2\times7)
\]

Result:

\[
5\times7
\]

---

## Memory Trick

Inside numbers disappear.

Outside numbers remain.

---

Example:

\[
(2\times3)
\times
(3\times4)
\]

Remove middle:

```
3 3

```

Remain:

\[
2\times4
\]

---

# 8. Non-Commutativity of Matrix Multiplication

## Simple Definition

For ordinary numbers:

\[
2\times3
=
3\times2
\]

---

But matrices behave differently.

Usually:

\[
AB \ne BA
\]

---

## Example

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

Dimension:

\[
(1\times2)(2\times1)
\]

Result:

\[
1\times1
\]

---

### BA

Dimension:

\[
(2\times1)(1\times2)
\]

Result:

\[
2\times2
\]

---

Different dimensions.

Therefore:

\[
AB\ne BA
\]

---

## Real-Life Example

Putting on socks then shoes.

Works.

Putting on shoes then socks.

Does not work.

Order matters.

---

# 9. Row-Column Multiplication Method (Dot Product Method)

## Simple Definition

Each entry in the result matrix comes from:

Row × Column

using the dot product.

---

## Example

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

Take:

Row from A:

\[
(1,2)
\]

Column from B:

\[
\begin{bmatrix}
3\\
4
\end{bmatrix}
\]

---

Compute dot product:

\[
1(3)+2(4)
\]

\[
=3+8
\]

\[
=11
\]

---

Result:

\[
AB=
\begin{bmatrix}
11
\end{bmatrix}
\]

---

# Larger Example

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

First Entry

\[
(1,2)\cdot(5,7)
\]

\[
=1(5)+2(7)
\]

\[
=19
\]

---

Second Entry

\[
(1,2)\cdot(6,8)
\]

\[
=22
\]

---

Third Entry

\[
(3,4)\cdot(5,7)
\]

\[
=43
\]

---

Fourth Entry

\[
(3,4)\cdot(6,8)
\]

\[
=50
\]

---

Result:

\[
\begin{bmatrix}
19 & 22\\
43 & 50
\end{bmatrix}
\]

---

# Why Matrix Multiplication Matters

Machine Learning:

\[
Predictions = Data \times Weights
\]

Computer Graphics:

\[
NewPosition = Transformation \times Position
\]

Neural Networks:

\[
Output = Input \times Weights + Bias
\]

Every modern AI system uses matrix multiplication extensively.

---

# 10. Identity Matrix (Upcoming Topic)

## Simple Definition

The identity matrix is the matrix version of the number:

\[
1
\]

for multiplication.

---

For numbers:

\[
5\times1=5
\]

---

For matrices:

\[
AI=A
\]

and

\[
IA=A
\]

---

## Example

2×2 Identity Matrix

\[
I=
\begin{bmatrix}
1 & 0\\
0 & 1
\end{bmatrix}
\]

---

3×3 Identity Matrix

\[
I=
\begin{bmatrix}
1 & 0 & 0\\
0 & 1 & 0\\
0 & 0 & 1
\end{bmatrix}
\]

---

## What Makes It Special?

Multiplying by the identity matrix leaves the matrix unchanged.

Just like multiplying by 1.

---

# Complete Big Picture

A Matrix is:

\[
\begin{bmatrix}
a & b\\
c & d
\end{bmatrix}
\]

organized into:

- Rows
- Columns

---

Important Operations

### Matrix Addition

\[
A+B
\]

Requires same dimensions.

---

### Scalar Multiplication

\[
kA
\]

Multiply every element by k.

---

### Matrix Multiplication

\[
AB
\]

Requires:

\[
Columns(A)=Rows(B)
\]

---

### Result Size

\[
(m\times n)(n\times p)
=
(m\times p)
\]

---

### Matrix Multiplication is NOT Commutative

\[
AB\ne BA
\]

in general.

---

### Row-Column Method

Every entry is calculated using:

\[
Row\cdot Column
\]

(dot product)

---

### Identity Matrix

Matrix version of:

\[
1
\]

for multiplication.

---

These concepts form the foundation of:

- Linear Algebra
- Computer Graphics
- Data Analysis
- Machine Learning
- Deep Learning
- Neural Networks
- Transformers
- Embeddings
- Recommendation Systems
- Vector Databases
- Large Language Models (LLMs)