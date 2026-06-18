# Vector Operations and 3D Geometry Fundamentals

---

# 1. Scalar Product / Dot Product

## Simple Definition

The **dot product** (also called the **scalar product**) is a mathematical operation that takes two vectors and produces a single number (scalar).

For vectors:

\[
\mathbf{A} = (a_1,a_2)
\]

\[
\mathbf{B} = (b_1,b_2)
\]

The dot product is:

\[
\mathbf{A}\cdot\mathbf{B}
=
a_1b_1+a_2b_2
\]

---

## Example 1

\[
(2,3)\cdot(4,5)
\]

\[
=(2\times4)+(3\times5)
\]

\[
=8+15
\]

\[
=23
\]

Result:

\[
23
\]

A single number.

---

## Example 2

Student Scores

Student A:

\[
(80,90)
\]

Student B:

\[
(70,85)
\]

Dot Product:

\[
80\times70+90\times85
\]

\[
=5600+7650
\]

\[
=13250
\]

This measures similarity.

---

## Example 3

Force and Motion

Dot products help calculate:

- Work Done
- Similarity
- Projection

in physics and machine learning.

---

# 2. Vector Representation in Higher Dimensions

## Simple Definition

Vectors are not limited to 2D.

They can exist in:

- 2D
- 3D
- 4D
- 100D
- Millions of dimensions

---

# 2D Vector

\[
(3,4)
\]

Represents:

- 3 units in x direction
- 4 units in y direction

---

# 3D Vector

\[
(3,4,5)
\]

Represents:

- 3 units x
- 4 units y
- 5 units z

---

## Example 1

Video Game Character

\[
(5,2)
\]

Position on screen.

---

## Example 2

Drone

\[
(5,2,10)
\]

Position in air.

---

## Example 3

Machine Learning

An image may be represented as:

\[
(0.3,0.8,0.4,0.9,\ldots)
\]

Thousands of dimensions.

---

# 3. Angle Between Two Vectors

## Simple Definition

The dot product helps determine the angle between vectors.

Formula:

\[
\mathbf{A}\cdot\mathbf{B}
=
|\mathbf{A}||\mathbf{B}|\cos\theta
\]

Therefore:

\[
\cos\theta
=
\frac{\mathbf{A}\cdot\mathbf{B}}
{|\mathbf{A}||\mathbf{B}|}
\]

---

## Example 1

Vectors:

\[
(1,0)
\]

\[
(0,1)
\]

Dot product:

\[
1(0)+0(1)
=
0
\]

Thus:

\[
\theta=90^\circ
\]

---

## Example 2

Vectors:

\[
(1,0)
\]

\[
(1,0)
\]

Angle:

\[
0^\circ
\]

Same direction.

---

## Example 3

Vectors:

\[
(1,0)
\]

\[
(-1,0)
\]

Angle:

\[
180^\circ
\]

Opposite directions.

---

# 4. Parallel Vectors

## Simple Definition

Vectors are parallel if they point:

- Same direction
- Opposite direction

---

## Example 1

\[
(2,4)
\]

\[
(1,2)
\]

Since:

\[
(2,4)=2(1,2)
\]

Parallel.

---

## Example 2

Roads

Two straight roads heading east.

Parallel.

---

## Example 3

\[
(1,2)
\]

\[
(-1,-2)
\]

Opposite direction.

Still parallel.

---

# 5. Perpendicular / Orthogonal Vectors

## Simple Definition

Two vectors are perpendicular if they meet at:

\[
90^\circ
\]

---

## Key Rule

\[
\mathbf{A}\cdot\mathbf{B}=0
\]

---

## Example 1

\[
(1,0)
\]

\[
(0,1)
\]

Dot Product:

\[
0
\]

Therefore perpendicular.

---

## Example 2

Room Corner

Wall and floor meet at:

\[
90^\circ
\]

Orthogonal.

---

## Example 3

\[
(2,3)
\]

\[
(3,-2)
\]

Dot Product:

\[
6-6=0
\]

Perpendicular.

---

# 6. Modulus / Magnitude of a Vector

## Simple Definition

Magnitude means length.

---

## Formula (2D)

\[
|\mathbf{v}|
=
\sqrt{x^2+y^2}
\]

---

## Example 1

\[
(3,4)
\]

\[
\sqrt{3^2+4^2}
\]

\[
=\sqrt{25}
\]

\[
=5
\]

---

## Example 2

\[
(6,8)
\]

\[
=10
\]

---

## Example 3

Distance from origin.

Vector:

\[
(5,12)
\]

Length:

\[
13
\]

---

# 7. Vector Quantities vs Scalar Quantities

## Scalars

Only magnitude.

---

### Examples

- Temperature
- Age
- Mass
- Time
- Money

---

## Vectors

Magnitude + Direction.

---

### Examples

- Velocity
- Force
- Displacement
- Acceleration

---

## Example

Scalar:

"Car speed is 60 km/h"

---

Vector:

"Car velocity is 60 km/h North"

---

# 8. Unit Vectors in 3D

## Definition

Unit vectors have length:

\[
1
\]

---

## Along x-axis

\[
\hat{i}
=
(1,0,0)
\]

---

## Along y-axis

\[
\hat{j}
=
(0,1,0)
\]

---

## Along z-axis

\[
\hat{k}
=
(0,0,1)
\]

---

## Example

\[
(3,4,5)
\]

can be written:

\[
3\hat{i}
+
4\hat{j}
+
5\hat{k}
\]

---

# 9. Trigonometric Functions (Cosine and Sine)

## Cosine

Measures horizontal position on unit circle.

---

## Sine

Measures vertical position on unit circle.

---

# Important Values

| Angle | Cos | Sin |
|---------|---------|---------|
| 0° | 1 | 0 |
| 30° | 0.866 | 0.5 |
| 45° | 0.707 | 0.707 |
| 60° | 0.5 | 0.866 |
| 90° | 0 | 1 |

---

## Example

At

\[
90^\circ
\]

\[
\cos(90^\circ)=0
\]

\[
\sin(90^\circ)=1
\]

---

# 10. Distributive Property of Dot Product

## Rule

\[
\mathbf{u}\cdot(\mathbf{v}+\mathbf{w})
=
\mathbf{u}\cdot\mathbf{v}
+
\mathbf{u}\cdot\mathbf{w}
\]

---

## Example

Let

\[
u=(1,2)
\]

\[
v=(3,4)
\]

\[
w=(5,6)
\]

---

Left Side

\[
(1,2)\cdot(8,10)
\]

\[
=28
\]

---

Right Side

\[
(1,2)\cdot(3,4)
+
(1,2)\cdot(5,6)
\]

\[
=11+17
\]

\[
=28
\]

Same answer.

---

# 11. Inverse Cosine (cos⁻¹)

## Simple Definition

Inverse cosine finds the angle.

---

If

\[
\cos\theta=0.5
\]

then

\[
\theta=\cos^{-1}(0.5)
\]

\[
=60^\circ
\]

---

## Example 1

\[
\cos\theta=1
\]

\[
\theta=0^\circ
\]

---

## Example 2

\[
\cos\theta=0
\]

\[
\theta=90^\circ
\]

---

## Example 3

\[
\cos\theta=-1
\]

\[
\theta=180^\circ
\]

---

# 12. Cartesian Coordinates in 3D

## Simple Definition

3D space uses:

\[
(x,y,z)
\]

---

## Axes

- x = left-right
- y = forward-backward
- z = up-down

---

## Example 1

Drone:

\[
(10,5,20)
\]

---

## Example 2

Building corner.

---

## Example 3

Game world coordinates.

---

## Visual

```
       z
       ↑
       |
       |
       O------→ x
      /
     /
    y

```

---

# 13. Right-Hand Rule Approximation

## Simple Definition

A simple way to visualize 3D axes.

---

Use your right hand:

- Index finger → x-axis
- Middle finger → y-axis
- Thumb → z-axis

---

## Example

Computer graphics.

---

## Example

Engineering drawings.

---

## Example

Physics simulations.

---

# 14. Physical Modeling with 3D Vectors

## Simple Definition

3D vectors model real-world quantities.

---

## Example 1: Force

Push a box:

\[
(10,0,0)
\]

---

## Example 2: Airplane Velocity

\[
(500,50,100)
\]

Meaning:

- Forward
- Sideways
- Upward

movement.

---

## Example 3: Drone Motion

\[
(5,3,2)
\]

Represents movement in all three directions.

---

# 15. Cross Product (Upcoming Topic)

## Simple Definition

The cross product takes two vectors and produces another vector.

---

## Dot Product

Input:

Two vectors

Output:

One number

---

## Cross Product

Input:

Two vectors

Output:

One vector

---

## Formula

\[
\mathbf{A}\times\mathbf{B}
=
\mathbf{C}
\]

---

## Example

\[
(1,0,0)
\times
(0,1,0)
=
(0,0,1)
\]

or

\[
\hat{i}\times\hat{j}
=
\hat{k}
\]

---

## Real-Life Examples

### Physics

Torque

### Engineering

Rotational forces

### Computer Graphics

Surface normals

### Robotics

Orientation calculations

---

# Complete Big Picture

A vector can be represented as:

\[
(3,4)
\]

or

\[
3\hat{i}+4\hat{j}
\]

Its magnitude is:

\[
5
\]

Its angle is:

\[
\theta
=
\cos^{-1}
\left(
\frac{\mathbf{A}\cdot\mathbf{B}}
{|\mathbf{A}||\mathbf{B}|}
\right)
\]

Dot products help us measure:

- Similarity
- Angles
- Orthogonality

while cross products help us determine:

- Orientation
- Rotation
- Perpendicular directions

These concepts form the mathematical foundation of:

- Linear Algebra
- Physics
- Computer Graphics
- Robotics
- Machine Learning
- Deep Learning
- Embeddings
- Vector Databases
- Large Language Models (LLMs)