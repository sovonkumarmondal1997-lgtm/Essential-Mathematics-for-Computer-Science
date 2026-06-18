# Cross Product (Vector Product) Fundamentals

---

# Introduction

Previously, we learned:

- Vector Addition
- Vector Subtraction
- Dot Product

The **Dot Product** takes two vectors and produces a **scalar (number)**.

Now we learn the **Cross Product**, which takes two vectors and produces another **vector**.

This makes the cross product extremely important in:

- Physics
- Robotics
- Computer Graphics
- Engineering
- Aerospace
- Machine Learning Geometry

---

# 1. Cross Product / Vector Product

## Simple Definition

The **cross product** is a mathematical operation between two vectors in three-dimensional space.

It produces:

\[
\mathbf{u}\times\mathbf{v}
=
\mathbf{w}
\]

where:

- Input = Two vectors
- Output = One vector

---

## Visual Idea

Suppose:

- One vector points East
- One vector points North

The cross product produces a vector pointing Up.

```
        Up
         ↑
         |
         |
North ←--+--> East

```

---

## Example 1

\[
\hat{i}\times\hat{j}
=
\hat{k}
\]

Meaning:

- Right direction
- Cross Up direction

Produces:

- Forward/Outward direction

---

## Example 2

Physics

Force:

\[
\mathbf{F}
\]

Applied to a wrench.

Distance from pivot:

\[
\mathbf{r}
\]

Torque:

\[
\mathbf{\tau}
=
\mathbf{r}\times\mathbf{F}
\]

Cross products create rotational effects.

---

## Example 3

Computer Graphics

Cross product helps determine:

- Surface orientation
- Lighting direction
- Face normals

---

# 2. Vector Output vs Scalar Output

## Dot Product

Input:

\[
\mathbf{u},\mathbf{v}
\]

Output:

\[
\mathbf{u}\cdot\mathbf{v}
=
5
\]

A number.

---

## Cross Product

Input:

\[
\mathbf{u},\mathbf{v}
\]

Output:

\[
\mathbf{u}\times\mathbf{v}
=
(1,2,3)
\]

A vector.

---

## Example

Dot Product

```
Two vectors
     ↓
Single Number

```

Cross Product

```
Two vectors
     ↓
Another Vector

```

---

## Real-Life Analogy

Dot Product:

"How similar are these directions?"

Cross Product:

"What direction is perpendicular to both?"

---

# 3. Geometric Definition of Cross Product

## Formula

\[
\mathbf{u}\times\mathbf{v}
=
||\mathbf{u}||
\,||\mathbf{v}||
\sin(\theta)
\hat{n}
\]

where:

- \(||u||\) = magnitude of u
- \(||v||\) = magnitude of v
- \(\theta\) = angle between vectors
- \(\hat{n}\) = perpendicular unit vector

---

## Interpretation

Magnitude of cross product:

\[
||u||||v||\sin(\theta)
\]

Direction:

\[
\hat{n}
\]

---

## Example

Suppose

\[
||u||=3
\]

\[
||v||=4
\]

\[
\theta=90^\circ
\]

Then

\[
3\times4\times1
=
12
\]

Cross product magnitude = 12.

---

## Important Observation

When angle increases:

\[
\sin(\theta)
\]

changes.

Therefore cross product changes.

---

# 4. Normal Unit Vector (n̂)

## Simple Definition

A normal vector is perpendicular to a surface or plane.

A normal unit vector has:

\[
||\hat{n}||=1
\]

---

## Visual

```
      n̂
      ↑
      |
      |
------------
 Plane

```

---

## Example 1

Table surface.

Normal vector points upward.

---

## Example 2

Wall.

Normal vector sticks directly outward.

---

## Example 3

Two vectors define a plane.

Cross product finds the perpendicular direction.

---

# 5. Cross Product of Parallel Vectors

## Rule

If vectors are parallel:

\[
\theta=0^\circ
\]

or

\[
180^\circ
\]

Then:

\[
\sin(\theta)=0
\]

Therefore:

\[
u\times v=0
\]

---

## Example 1

\[
(1,2,3)
\times
(1,2,3)
=
0
\]

---

## Example 2

\[
(2,4)
\times
(1,2)
=
0
\]

Parallel.

---

## Example 3

Car moving East.

Another car moving East.

No perpendicular direction exists.

Cross product is zero.

---

# Self Cross Product

Any vector crossed with itself:

\[
u\times u=0
\]

because angle is:

\[
0^\circ
\]

---

# 6. Odd Function Property

## Rule

For sine:

\[
\sin(-\theta)
=
-\sin(\theta)
\]

---

## Example 1

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
\sin(45^\circ)
=
0.707
\]

\[
\sin(-45^\circ)
=
-0.707
\]

---

## Why Important?

Cross product direction changes when angle direction changes.

---

# 7. Anticlockwise / Positive Angular Direction

## Simple Definition

Positive angles are measured anticlockwise.

---

## Visual

```
          y
          ↑
          |
          |
          |
----------+------→ x

```

Moving from x-axis toward y-axis:

Counterclockwise.

Positive angle.

---

## Example

\[
\hat{i}
\rightarrow
\hat{j}
\]

Rotation:

\[
+90^\circ
\]

---

## Example

Clock hands move clockwise.

That is usually considered negative rotation.

---

# 8. Anticommutativity

## Rule

Vector addition:

\[
u+v=v+u
\]

Cross product:

\[
u\times v
=
-(v\times u)
\]

---

## Example

\[
\hat{i}\times\hat{j}
=
\hat{k}
\]

Swap order:

\[
\hat{j}\times\hat{i}
=
-\hat{k}
\]

---

## Example 2

Forward then Right

is not the same as

Right then Forward.

Direction flips.

---

## Why?

Changing order reverses orientation.

---

# 9. Right-Hand Rule Orientation

## Simple Definition

Right-Hand Rule determines cross product direction.

---

## Steps

Point:

- Index finger → first vector
- Middle finger → second vector
- Thumb → result

---

## Example

\[
\hat{i}\times\hat{j}
\]

Index finger:

x-direction

Middle finger:

y-direction

Thumb:

z-direction

Result:

\[
\hat{k}
\]

---

## Example 2

\[
\hat{j}\times\hat{i}
\]

Thumb points opposite.

Result:

\[
-\hat{k}
\]

---

# Visual Idea

```
Thumb  → Result

Middle → Second Vector

Index  → First Vector

```

---

# 10. Cyclic Permutation of Unit Vectors

## Fundamental Relationships

\[
\hat{i}\times\hat{j}
=
\hat{k}
\]

\[
\hat{j}\times\hat{k}
=
\hat{i}
\]

\[
\hat{k}\times\hat{i}
=
\hat{j}
\]

---

## Easy Memory Trick

Cycle:

\[
i
\rightarrow
j
\rightarrow
k
\rightarrow
i
\]

Moving forward:

Positive.

---

## Example

\[
j\times k=i
\]

Positive.

---

## Reverse Direction

\[
j\times i=-k
\]

Negative.

---

# Complete Table

| Cross Product | Result |
|--------------|---------|
| i × j | k |
| j × k | i |
| k × i | j |
| j × i | -k |
| k × j | -i |
| i × k | -j |

---

# 11. Distributive Property of Cross Product

## Rule

\[
u\times(v+w)
=
u\times v
+
u\times w
\]

---

## Example

Let

\[
u=i
\]

\[
v=j
\]

\[
w=k
\]

Then

\[
i\times(j+k)
\]

---

Expand:

\[
(i\times j)
+
(i\times k)
\]

---

Substitute:

\[
k+(-j)
\]

Result:

\[
k-j
\]

---

## Real-Life Analogy

Multiply each component separately.

Then add results.

---

# 12. Standard Notational Ordering

## Simple Definition

Final vectors are written in order:

\[
\hat{i}
\]

\[
\hat{j}
\]

\[
\hat{k}
\]

---

## Example

Instead of writing:

\[
3k+2i+5j
\]

Write:

\[
2i+5j+3k
\]

---

## Why?

Consistency.

Makes vectors easier to read.

---

## Example

Vector:

\[
(4,2,7)
\]

written as:

\[
4i+2j+7k
\]

not

\[
7k+4i+2j
\]

---

# Complete Big Picture

Cross Product:

\[
u\times v
\]

takes:

- Two vectors

and produces:

- One perpendicular vector

---

Magnitude:

\[
||u||||v||\sin(\theta)
\]

Direction:

\[
\hat{n}
\]

determined by:

- Right-Hand Rule

---

Important Properties

### Parallel Vectors

\[
u\times v=0
\]

---

### Self Cross Product

\[
u\times u=0
\]

---

### Anticommutative

\[
u\times v
=
-(v\times u)
\]

---

### Distributive

\[
u\times(v+w)
=
u\times v
+
u\times w
\]

---

### Cyclic Unit Vectors

\[
i\times j=k
\]

\[
j\times k=i
\]

\[
k\times i=j
\]

---

Cross products are heavily used in:

- Physics (Torque)
- Engineering
- Robotics
- Aerospace
- Computer Graphics
- 3D Game Engines
- Computer Vision
- Geometry
- Machine Learning
- Simulation Systems

and are one of the most important operations in three-dimensional mathematics.