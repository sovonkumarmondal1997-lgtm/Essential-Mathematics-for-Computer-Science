# Vectors and Vector Space Fundamentals

---

# 1. Vectors (Physical Displacements or Forces)

## Simple Definition

A **vector** is a quantity that has:

1. Magnitude (how much)
2. Direction (which way)

Unlike ordinary numbers, vectors tell us both **size** and **direction**.

---

## Example 1: Walking

Suppose you walk:

- 5 meters East

This information contains:

- Magnitude = 5 meters
- Direction = East

Therefore it is a vector.

---

### Not a Vector

If someone says:

"I walked 5 meters."

Direction is missing.

This is only a **scalar quantity**.

---

## Example 2: Force

You push a box:

- Force = 20 Newtons
- Direction = Right

This is a vector.

---

## Example 3: Car Movement

A car travels:

- 60 km North

This is a vector because it has:

- Magnitude = 60 km
- Direction = North

---

## Visual Representation

```
------->

```

The arrow length shows magnitude.

The arrow direction shows direction.

---

# 2. Cartesian Plane / Cartesian Coordinates

## Simple Definition

A Cartesian Plane is a coordinate system used to locate points.

Every point is represented by:

\[
(x,y)
\]

where:

- x = horizontal position
- y = vertical position

---

## Example 1: City Map

Suppose:

\[
(3,4)
\]

means:

- Move 3 units right
- Move 4 units up

---

### Graph

```
y
↑
|
|        ● (3,4)
|
|
+----------------→ x

```

---

## Example 2: Video Game Character

Player position:

\[
(5,2)
\]

means:

- 5 steps right
- 2 steps up

---

## Example 3: Robot

Robot location:

\[
(10,-3)
\]

means:

- 10 units right
- 3 units down

---

# 3. Vector Space

## Simple Definition

A vector space is a collection of vectors that obey certain rules.

You can:

- Add vectors
- Subtract vectors
- Multiply vectors by numbers

and still remain inside the same space.

---

## Example 1: Arrows on a Plane

All arrows on a 2D plane form a vector space.

Example:

\[
(1,2)
\]

and

\[
(3,4)
\]

Add:

\[
(1,2)+(3,4)
=(4,6)
\]

Still a valid vector.

---

## Example 2: Physical Movement

Possible movements:

- North
- South
- East
- West

Any combination is still a movement vector.

Therefore they form a vector space.

---

## Example 3: Computer Graphics

Points on a screen:

\[
(x,y)
\]

can be scaled and moved.

These coordinates form a vector space.

---

# 4. Dimensionality

## Simple Definition

Dimensionality tells us how many independent directions exist.

---

# Two-Dimensional Space (2D)

Requires two coordinates:

\[
(x,y)
\]

---

## Example

Chessboard

```
(4,5)

```

Need:

- Row
- Column

Only two directions.

---

## Real-Life Examples

- Maps
- Mobile screens
- Paper drawings

---

# Three-Dimensional Space (3D)

Requires:

\[
(x,y,z)
\]

---

## Example

Position of a drone:

\[
(5,2,10)
\]

means:

- 5 units right
- 2 units forward
- 10 units up

---

## Real-Life Examples

- Buildings
- Airplanes
- Human body movement

---

# 5. Polar Coordinates

## Simple Definition

Instead of saying:

\[
(x,y)
\]

we describe a vector using:

\[
(r,\theta)
\]

where:

- r = magnitude
- θ = angle

---

## Example 1

Vector length:

\[
r=5
\]

Angle:

\[
\theta = 45^\circ
\]

or

\[
\theta = \pi/4
\]

---

## Visual

```
      /
     /
    /
   /
  /
 O

```

The slanted line has:

- Length = r
- Angle = θ

---

## Example 2: Radar

Aircraft detected:

- 100 km away
- 30° from North

This is naturally represented in polar coordinates.

---

## Example 3: GPS Direction

"Walk 200 meters at 60°."

This is polar form.

---

# 6. Trigonometric Relationship of Vectors

Suppose:

\[
v=(x,y)
\]

We can find its angle.

---

## Formula

\[
\theta=\tan^{-1}\left(\frac{y}{x}\right)
\]

---

## Example 1

Vector:

\[
(3,3)
\]

\[
\theta=\tan^{-1}(3/3)
\]

\[
=\tan^{-1}(1)
\]

\[
=45^\circ
\]

---

## Example 2

Vector:

\[
(0,5)
\]

Points straight upward.

Angle:

\[
90^\circ
\]

---

## Example 3

Vector:

\[
(5,0)
\]

Angle:

\[
0^\circ
\]

Points right.

---

# 7. Associativity of Vector Addition

## Rule

\[
(u+v)+w
=
u+(v+w)
\]

Grouping does not matter.

---

## Example

Let:

\[
u=(1,1)
\]

\[
v=(2,2)
\]

\[
w=(3,3)
\]

---

### Left Side

\[
(u+v)+w
\]

\[
=(3,3)+(3,3)
\]

\[
=(6,6)
\]

---

### Right Side

\[
u+(v+w)
\]

\[
=(1,1)+(5,5)
\]

\[
=(6,6)
\]

Same result.

---

## Real-Life Example

You walk:

- 1 km East
- then 2 km East
- then 3 km East

Grouping journeys differently gives same destination.

---

# 8. Commutativity of Vector Addition

## Rule

\[
u+v=v+u
\]

Order does not matter.

---

## Example

\[
(2,3)+(4,1)
\]

\[
=(6,4)
\]

---

Reverse:

\[
(4,1)+(2,3)
\]

\[
=(6,4)
\]

Same answer.

---

## Real-Life Example

Move:

- 5 steps right
- 3 steps up

or

- 3 steps up
- 5 steps right

Final location is identical.

---

# 9. Identity Vector

## Simple Definition

The identity vector is the vector that changes nothing when added.

---

## Formula

\[
v+0=v
\]

where

\[
0=(0,0)
\]

---

## Example

\[
(5,7)+(0,0)
\]

\[
=(5,7)
\]

---

## Real-Life Example

Walking:

- 10 meters East
- then 0 meters

You remain at same location.

---

# 10. Inverse of a Vector

## Simple Definition

Every vector has an opposite vector.

---

## Formula

If

\[
v=(a,b)
\]

then

\[
-v=(-a,-b)
\]

---

## Example

\[
v=(3,4)
\]

Inverse:

\[
(-3,-4)
\]

---

### Add Them

\[
(3,4)+(-3,-4)
\]

\[
=(0,0)
\]

Identity vector obtained.

---

## Real-Life Example

Walk:

- 10 m East

then

- 10 m West

Net movement:

\[
0
\]

---

# 11. Distributive Property

## Rule

\[
k(u+v)
=
ku+kv
\]

where k is a scalar.

---

## Example

Let:

\[
k=2
\]

\[
u=(1,2)
\]

\[
v=(3,4)
\]

---

### Left Side

\[
2((1,2)+(3,4))
\]

\[
=2(4,6)
\]

\[
=(8,12)
\]

---

### Right Side

\[
2(1,2)+2(3,4)
\]

\[
=(2,4)+(6,8)
\]

\[
=(8,12)
\]

Same answer.

---

## Real-Life Example

Doubling two trips separately gives same result as doubling the total trip.

---

# 12. Unit Vectors

## Simple Definition

A unit vector has magnitude 1.

It indicates direction only.

---

# x-Direction Unit Vector

\[
\hat{i}
=
(1,0)
\]

Points right.

---

# y-Direction Unit Vector

\[
\hat{j}
=
(0,1)
\]

Points up.

---

## Visual

```
j ^
  |
  |
  |
--+----> i

```

---

## Example

Move:

- 3 units right

can be written:

\[
3\hat{i}
\]

---

## Example

Move:

- 5 units up

can be written:

\[
5\hat{j}
\]

---

# 13. Linear Combination of Unit Vectors

## Simple Definition

Any vector in 2D can be built from:

\[
\hat{i}
\]

and

\[
\hat{j}
\]

---

## General Form

\[
a\hat{i}+b\hat{j}
\]

---

## Example 1

Vector:

\[
(3,4)
\]

Written as:

\[
3\hat{i}+4\hat{j}
\]

---

## Example 2

Vector:

\[
(10,2)
\]

Written as:

\[
10\hat{i}+2\hat{j}
\]

---

## Example 3

Vector:

\[
(-5,7)
\]

Written as:

\[
-5\hat{i}+7\hat{j}
\]

---

# Complete Big Picture

A vector represents movement or force.

Example:

\[
(3,4)
\]

can be viewed as:

### Cartesian Form

\[
(3,4)
\]

---

### Unit Vector Form

\[
3\hat{i}+4\hat{j}
\]

---

### Polar Form

Magnitude:

\[
r=\sqrt{3^2+4^2}=5
\]

Angle:

\[
\theta=\tan^{-1}(4/3)
\]

\[
\theta \approx 53.13^\circ
\]

---

Thus the same vector can be represented in multiple ways:

\[
(3,4)
=
3\hat{i}+4\hat{j}
=
(5,53.13^\circ)
\]

All describe the exact same vector.