# Linear Algebra, Gaussian Elimination, and Systems of Linear Equations

---

# Introduction

So far, we have learned:

- Vectors
- Matrices
- Matrix Multiplication
- Determinants
- Matrix Inverses
- Transformations
- Homogeneous Coordinates

Now we arrive at one of the most important topics in mathematics:

# Linear Algebra

Linear Algebra is the mathematical foundation behind:

- Machine Learning
- Artificial Intelligence
- Data Science
- Computer Graphics
- Robotics
- Physics
- Engineering
- Computer Vision
- Large Language Models (LLMs)

Almost every modern AI system performs millions or billions of linear algebra operations every second.

---

# 1. Linear Algebra

## Simple Definition

Linear Algebra is the branch of mathematics that studies:

- Linear Equations
- Vectors
- Matrices
- Vector Spaces
- Transformations

and how they work together.

---

## What Does "Linear" Mean?

A linear relationship creates a straight line.

Example:

\[
y=2x+1
\]

---

When plotted:

```
      /
     /
    /
   /
  /
 /
```

A straight line.

---

## Example 1

Equation:

\[
x+y=10
\]

Linear equation.

---

## Example 2

Equation:

\[
2x+3y=7
\]

Linear equation.

---

## Example 3

Equation:

\[
3x+2y-z=12
\]

Still linear.

---

# Real-Life Applications

## GPS Navigation

Calculates positions using linear algebra.

---

## Computer Graphics

Every object is transformed using matrices.

---

## Machine Learning

Predictions are often:

\[
Y=WX+b
\]

which is pure linear algebra.

---

# Why Linear Algebra Matters

Without linear algebra:

- Neural Networks
- Transformers
- Recommendation Systems
- Search Engines

would not exist.

---

# 2. Gaussian Elimination

## Simple Definition

Gaussian Elimination is a systematic method for solving systems of equations.

---

Instead of guessing answers,

we transform equations step by step until the solution becomes obvious.

---

## Goal

Convert a matrix into:

# Row Echelon Form

Then solve using:

# Back-Substitution

---

## Example 1

Solve:

\[
x+y=5
\]

\[
x-y=1
\]

---

Write as matrix:

\[
\begin{bmatrix}
1 & 1 & 5\\
1 & -1 & 1
\end{bmatrix}
\]

---

Subtract Row 1 from Row 2:

\[
R_2-R_1
\]

---

Result:

\[
\begin{bmatrix}
1 & 1 & 5\\
0 & -2 & -4
\end{bmatrix}
\]

---

Now solving becomes easy.

---

## Example 2

Finding prices:

- Apples
- Oranges

using two equations.

---

## Example 3

Finding unknown electrical currents.

---

# Why Gaussian Elimination Matters

Computers use it extensively.

Many scientific calculations depend on it.

---

# 3. System of Simultaneous Linear Equations

## Simple Definition

A system of simultaneous equations contains multiple equations that share the same variables.

---

## Example 1

\[
x+y=5
\]

\[
x-y=1
\]

---

Both equations involve:

- x
- y

---

The solution must satisfy BOTH equations.

---

## Example 2

\[
2x+y=8
\]

\[
x-y=1
\]

---

Solution must satisfy both simultaneously.

---

## Example 3

Three Variables

\[
x+y+z=10
\]

\[
x-y+z=4
\]

\[
2x+y-z=7
\]

---

Now we solve for:

- x
- y
- z

together.

---

# Real-Life Example

Suppose:

Apple price = x

Orange price = y

---

You know:

\[
x+y=50
\]

\[
2x+y=80
\]

---

Find:

- Apple price
- Orange price

---

# Why Systems Matter

Most real-world problems involve multiple unknowns.

---

# 4. Coefficient Matrix / Augmented Matrix

## Simple Definition

Instead of writing equations repeatedly,

we organize them into a matrix.

---

# Example

System:

\[
x+y=5
\]

\[
x-y=1
\]

---

# Coefficient Matrix

Only coefficients:

\[
\begin{bmatrix}
1 & 1\\
1 & -1
\end{bmatrix}
\]

---

# Augmented Matrix

Include solutions:

\[
\begin{bmatrix}
1 & 1 & 5\\
1 & -1 & 1
\end{bmatrix}
\]

---

The vertical separator is often written:

\[
\begin{bmatrix}
1 & 1 & | & 5\\
1 & -1 & | & 1
\end{bmatrix}
\]

---

# Example 2

\[
2x+3y=7
\]

\[
4x+y=9
\]

---

Coefficient Matrix:

\[
\begin{bmatrix}
2 & 3\\
4 & 1
\end{bmatrix}
\]

---

Augmented Matrix:

\[
\begin{bmatrix}
2 & 3 & 7\\
4 & 1 & 9
\end{bmatrix}
\]

---

# Why Useful?

Matrices make calculations systematic and efficient.

---

# 5. Row Operations

## Simple Definition

Row operations are legal moves that simplify a matrix without changing its solution.

---

# Three Basic Row Operations

---

## Operation 1

Swap two rows.

---

Example:

\[
R_1 \leftrightarrow R_2
\]

---

## Operation 2

Multiply a row by a non-zero number.

---

Example:

\[
2R_1
\]

---

## Operation 3

Add or subtract rows.

---

Example:

\[
R_2-R_1
\]

---

# Example 1

\[
\begin{bmatrix}
1 & 2\\
1 & 3
\end{bmatrix}
\]

---

Apply:

\[
R_2-R_1
\]

---

Result:

\[
\begin{bmatrix}
1 & 2\\
0 & 1
\end{bmatrix}
\]

---

# Example 2

Multiply row by 2.

---

# Example 3

Swap rows to place a better pivot on top.

---

# Why Important?

Row operations gradually transform a matrix into a simpler form.

---

# 6. Row Echelon Form

## Simple Definition

Row Echelon Form is a staircase-shaped matrix.

---

## Properties

### Property 1

Leading entries move right as we move downward.

---

### Property 2

Everything below each leading entry is zero.

---

# Example

\[
\begin{bmatrix}
1 & 2 & 3\\
0 & 1 & 4\\
0 & 0 & 1
\end{bmatrix}
\]

---

Notice:

Below each leading number:

Only zeros.

---

# Visual

```
1 * *
0 1 *
0 0 1
```

Looks like stairs.

---

# Example 2

\[
\begin{bmatrix}
2 & 5\\
0 & 3
\end{bmatrix}
\]

Already in row echelon form.

---

# Example 3

\[
\begin{bmatrix}
1 & 4 & 2\\
0 & 1 & 6\\
0 & 0 & 7
\end{bmatrix}
\]

Also row echelon form.

---

# Why Important?

Makes solving equations easy.

---

# 7. Leading Diagonal

## Simple Definition

The leading diagonal runs from:

Top-left

to

Bottom-right.

---

# Example

\[
\begin{bmatrix}
1 & 2 & 3\\
4 & 5 & 6\\
7 & 8 & 9
\end{bmatrix}
\]

---

Leading diagonal:

\[
1,\;5,\;9
\]

---

# Visual

```
[ X . . ]
[ . X . ]
[ . . X ]
```

---

# Example 2

\[
\begin{bmatrix}
4 & 1\\
7 & 3
\end{bmatrix}
\]

Diagonal:

\[
4,\;3
\]

---

# Example 3

Identity Matrix

\[
\begin{bmatrix}
1 & 0 & 0\\
0 & 1 & 0\\
0 & 0 & 1
\end{bmatrix}
\]

Diagonal:

\[
1,1,1
\]

---

# Why Important?

Many matrix operations focus on diagonal elements.

---

# 8. Back-Substitution

## Simple Definition

After reaching row echelon form,

we solve variables from bottom to top.

---

# Why?

The last equation is usually the simplest.

---

# Example

Suppose we have:

\[
\begin{bmatrix}
1 & 2 & 3 & 14\\
0 & 1 & 4 & 13\\
0 & 0 & 1 & 2
\end{bmatrix}
\]

---

Equivalent equations:

\[
x+2y+3z=14
\]

\[
y+4z=13
\]

\[
z=2
\]

---

# Step 1

Solve last equation:

\[
z=2
\]

---

# Step 2

Substitute into second equation:

\[
y+4(2)=13
\]

\[
y=5
\]

---

# Step 3

Substitute into first equation:

\[
x+2(5)+3(2)=14
\]

\[
x+10+6=14
\]

\[
x=-2
\]

---

# Final Answer

\[
x=-2
\]

\[
y=5
\]

\[
z=2
\]

---

# Example 2

Three unknowns in physics.

---

# Example 3

Electrical circuit calculations.

---

# Why It Works

Row echelon form simplifies equations so that one variable appears at a time.

---

# Complete Big Picture

## Linear Algebra

The study of:

- Vectors
- Matrices
- Linear Equations
- Transformations

---

## System of Simultaneous Equations

Multiple equations sharing the same variables.

---

## Coefficient Matrix

Contains only coefficients.

---

## Augmented Matrix

Contains coefficients plus solutions.

---

## Row Operations

Allowed moves:

- Swap rows
- Multiply rows
- Add/Subtract rows

---

## Gaussian Elimination

Transforms matrices into row echelon form.

---

## Row Echelon Form

Staircase-shaped matrix with zeros below pivots.

---

## Leading Diagonal

Top-left to bottom-right diagonal.

---

## Back-Substitution

Solve:

1. Last variable first
2. Substitute upward
3. Continue until all variables are found

---

Linear Algebra is the mathematical language behind:

- Machine Learning
- Neural Networks
- Deep Learning
- Transformers
- Computer Graphics
- Robotics
- Computer Vision
- Search Engines
- Recommendation Systems
- Scientific Computing
- Large Language Models (LLMs)

because nearly every modern AI system ultimately solves enormous systems of linear equations using matrices and vectors.