# Trigonometric Problem Solving, Sine Rule, Cosine Rule, and Inverse Trigonometric Functions

---

# 1. Problem-Solving Strategy: "Knowns vs. Unknowns"

## What Does "Knowns vs. Unknowns" Mean?

Whenever you solve a mathematics problem, the first step is to identify:

### Knowns

Things already given in the question.

```text
"What do I know?"
```

Examples:

- Side lengths
- Angles
- Radius
- Area
- Coordinates

---

### Unknowns

Things you need to find.

```text
"What do I need to know?"
```

Examples:

- Missing side
- Missing angle
- Area
- Perimeter

---

## Why Is This Important?

Many students immediately start calculating.

Professional engineers, mathematicians, and scientists first ask:

```text
What information do I have?
```

and

```text
What information am I missing?
```

This helps choose the correct formula.

---

# Example 1

Suppose a triangle has:

```text
Angle A = 40°
Angle B = 60°
Side a = 8 cm
```

Find:

```text
Side b
```

---

### Knowns

```text
A = 40°
B = 60°
a = 8 cm
```

---

### Unknown

```text
b = ?
```

---

### Best Method

Since we know:

```text
Two angles + one side
```

Use:

```text
Sine Rule
```

---

# Example 2

Suppose:

```text
a = 5
b = 7
c = 9
```

Find:

```text
Angle A
```

---

### Knowns

```text
All three sides
```

---

### Unknown

```text
Angle A
```

---

### Best Method

Use:

```text
Cosine Rule
```

because no angles are given.

---

# Example 3

Before Solving

Always ask:

```text
Is this a right triangle?
```

```text
Do I know enough information?
```

```text
Which formula fits the data?
```

This habit saves time and avoids mistakes.

---

# Problem-Solving Checklist

```text
Step 1: List known values
Step 2: List unknown values
Step 3: Check assumptions
Step 4: Choose formula
Step 5: Solve
Step 6: Verify answer
```

---

# 2. The Sine Rule

## What is the Sine Rule?

The Sine Rule states that:

In any triangle, the ratio between a side and the sine of its opposite angle is constant.

---

## Triangle Notation

```text
         A
        /\
       /  \
    b /    \ c
     /      \
    /________\
   B     a    C
```

Notice:

```text
Side a opposite Angle A
Side b opposite Angle B
Side c opposite Angle C
```

---

# Standard Form

```text
sin(A)/a
=
sin(B)/b
=
sin(C)/c
```

---

# Reciprocal Form

```text
a/sin(A)
=
b/sin(B)
=
c/sin(C)
```

Both forms mean exactly the same thing.

Use whichever is easier.

---

# When Do We Use the Sine Rule?

Usually when we know:

### Case 1

```text
Two angles + one side
```

Find unknown side.

---

### Case 2

```text
Two sides + one opposite angle
```

Find unknown angle.

---

# Example 1: Find an Unknown Side

Given:

```text
A = 30°
B = 60°
a = 10 cm
```

Find:

```text
b
```

---

Using:

```text
a/sin(A)
=
b/sin(B)
```

Substitute:

```text
10/sin(30°)
=
b/sin(60°)
```

---

Since:

```text
sin(30°)=0.5
```

```text
10/0.5
=
b/0.866
```

```text
20
=
b/0.866
```

```text
b = 17.32 cm
```

---

# Example 2: Find an Unknown Angle

Given:

```text
a = 6
b = 10
A = 30°
```

Find:

```text
B
```

---

Using:

```text
sin(A)/a
=
sin(B)/b
```

Substitute:

```text
0.5/6
=
sin(B)/10
```

Multiply both sides:

```text
sin(B)
=
10 × 0.5 / 6
```

```text
sin(B)
=
0.8333
```

Now:

```text
B = sin⁻¹(0.8333)
```

```text
B ≈ 56.44°
```

---

# Real-Life Example

Suppose two surveyors measure:

- One side of a field
- Two angles

The Sine Rule can determine the remaining distances without directly measuring them.

---

# 3. The Cosine Rule

## What is the Cosine Rule?

The Cosine Rule is a generalization of Pythagoras' theorem.

---

# Recall Pythagoras

For right triangles:

```text
a²+b²=c²
```

Works only when:

```text
One angle = 90°
```

---

# Problem

Most triangles are not right triangles.

We need a formula that works for all triangles.

---

# Cosine Rule

```text
a²
=
b²+c²
-
2bc cos(A)
```

---

# Other Forms

```text
b²
=
a²+c²
-
2ac cos(B)
```

```text
c²
=
a²+b²
-
2ab cos(C)
```

---

# When Do We Use the Cosine Rule?

### Case 1

Given:

```text
Three sides
```

Find:

```text
Unknown angle
```

---

### Case 2

Given:

```text
Two sides
+
Included angle
```

Find:

```text
Unknown side
```

---

# Example 1: Find Unknown Side

Given:

```text
b = 8
c = 10
A = 60°
```

Find:

```text
a
```

---

Use:

```text
a²
=
b²+c²-2bc cos(A)
```

Substitute:

```text
a²
=
8²+10²-2(8)(10)(0.5)
```

```text
a²
=
64+100-80
```

```text
a²
=
84
```

```text
a
=
√84
```

```text
a ≈ 9.17
```

---

# Example 2: Find Unknown Angle

Given:

```text
a = 7
b = 8
c = 10
```

Find:

```text
A
```

---

Use:

```text
a²
=
b²+c²-2bc cos(A)
```

Substitute:

```text
49
=
64+100-160 cos(A)
```

```text
49
=
164-160 cos(A)
```

```text
160 cos(A)
=
115
```

```text
cos(A)
=
115/160
```

```text
cos(A)
=
0.71875
```

Now use inverse cosine:

```text
A = cos⁻¹(0.71875)
```

```text
A ≈ 44°
```

---

# Real-Life Example

Architects often know:

- Two wall lengths
- The angle between them

The Cosine Rule helps calculate the third wall length.

---

# 4. Inverse Trigonometric Functions for Unknown Angles

## What Are Inverse Trigonometric Functions?

Normal trigonometric functions:

```text
Angle → Ratio
```

Example:

```text
sin(30°)=0.5
```

Input:

```text
30°
```

Output:

```text
0.5
```

---

# Reverse Problem

Suppose we know:

```text
sin(θ)=0.5
```

What is:

```text
θ ?
```

We need an inverse operation.

---

# Inverse Sine

Written as:

```text
sin⁻¹
```

or

```text
arcsin
```

---

Example:

```text
θ = sin⁻¹(0.5)
```

```text
θ = 30°
```

---

# Inverse Cosine

Written as:

```text
cos⁻¹
```

or

```text
arccos
```

---

Example:

```text
θ = cos⁻¹(0.5)
```

```text
θ = 60°
```

---

# Inverse Tangent

Written as:

```text
tan⁻¹
```

or

```text
arctan
```

---

Example:

```text
θ = tan⁻¹(1)
```

```text
θ = 45°
```

---

# Calculator Example

Suppose:

```text
sin(θ)=0.7071
```

Press:

```text
SHIFT
SIN
0.7071
=
```

Result:

```text
45°
```

---

# Why Inverse Functions Matter

When solving triangles:

You often calculate:

```text
sin(θ)
```

or

```text
cos(θ)
```

first.

To get the actual angle, you must use:

```text
sin⁻¹
```

or

```text
cos⁻¹
```

---

# Example Using Sine Rule

Suppose:

```text
sin(A)=0.8
```

Then:

```text
A=sin⁻¹(0.8)
```

```text
A≈53.13°
```

---

# Example Using Cosine Rule

Suppose:

```text
cos(B)=0.6
```

Then:

```text
B=cos⁻¹(0.6)
```

```text
B≈53.13°
```

---

# Summary of Trigonometric Tools

| Situation | Best Formula |
|------------|------------|
| Right triangle | SOH-CAH-TOA |
| Two angles + one side | Sine Rule |
| Two sides + opposite angle | Sine Rule |
| Three sides known | Cosine Rule |
| Two sides + included angle | Cosine Rule |
| Need angle from sine value | sin⁻¹ |
| Need angle from cosine value | cos⁻¹ |
| Need angle from tangent value | tan⁻¹ |

---

# Quick Formula Sheet

## Sine Rule

```text
sin(A)/a
=
sin(B)/b
=
sin(C)/c
```

or

```text
a/sin(A)
=
b/sin(B)
=
c/sin(C)
```

---

## Cosine Rule

```text
a²
=
b²+c²
-
2bc cos(A)
```

---

## Inverse Functions

```text
θ = sin⁻¹(x)
```

```text
θ = cos⁻¹(x)
```

```text
θ = tan⁻¹(x)
```

---

# Final Key Idea

Successful trigonometric problem solving starts by separating:

```text
Known Information
```

from

```text
Unknown Information
```

Once you know what information is available:

- Use the **Sine Rule** when angles and opposite sides are related.
- Use the **Cosine Rule** when side lengths dominate the problem.
- Use **inverse trigonometric functions** to convert ratios back into actual angles.

Together, these tools allow you to solve almost any triangle, whether it contains a right angle or not.
