# Trigonometric Symmetry, Periodicity, Graph Transformations, and Angle Identities

---

# 1. Even Functions and the Symmetry of Cosine

## What is an Even Function?

An **even function** is a function that satisfies:

\[
f(-x) = f(x)
\]

This means:

```text
The left side of the graph is a mirror image
of the right side.
```

The graph is symmetric about the **y-axis**.

---

## Example of an Even Function

Consider:

\[
f(x)=x^2
\]

Evaluate:

```text
f(2)=4
```

and

```text
f(-2)=4
```

Since both are equal:

\[
f(-x)=f(x)
\]

so \(x^2\) is an even function.

---

# Cosine is an Even Function

Cosine satisfies:

\[
\cos(-\theta)=\cos(\theta)
\]

---

## Why?

On the unit circle:

- Positive angles move counterclockwise.
- Negative angles move clockwise.

Both positions have the same horizontal distance from the y-axis.

Since cosine measures horizontal position:

```text
Cosine remains unchanged.
```

---

## Example 1

\[
\cos(60^\circ)=0.5
\]

and

\[
\cos(-60^\circ)=0.5
\]

Therefore:

\[
\cos(-60^\circ)=\cos(60^\circ)
\]

---

## Unit Circle Visualization

```text
          *
       *     *
    *           *
 *               *
--------------------
 *               *
    *           *
       *     *
          *
```

Points above and below the x-axis have the same x-coordinate.

---

# Supplementary Cosine Identity

Another useful identity:

\[
\cos(\theta)
=
-\cos(\pi-\theta)
\]

---

## Example

Take:

\[
\theta=60^\circ
\]

Then:

\[
\pi-\theta
=
180^\circ-60^\circ
=
120^\circ
\]

We know:

\[
\cos(60^\circ)=0.5
\]

\[
\cos(120^\circ)=-0.5
\]

Thus:

\[
0.5=-(-0.5)
\]

Correct.

---

# Real-Life Analogy

Imagine standing:

```text
60° to the right
```

or

```text
60° to the left
```

Your forward distance remains identical.

That forward distance behaves like cosine.

---

# 2. Odd Functions and the Rotation of Sine

## What is an Odd Function?

An odd function satisfies:

\[
f(-x)=-f(x)
\]

---

## Meaning

The graph has:

```text
180° rotational symmetry
```

around the origin.

---

## Example

Consider:

\[
f(x)=x^3
\]

Evaluate:

```text
f(2)=8
```

```text
f(-2)=-8
```

Thus:

\[
f(-x)=-f(x)
\]

---

# Sine is an Odd Function

Sine satisfies:

\[
\sin(-\theta)
=
-\sin(\theta)
\]

---

## Why?

Sine measures vertical height.

If a point moves below the x-axis:

```text
Positive height becomes negative height.
```

---

## Example

\[
\sin(30^\circ)=0.5
\]

and

\[
\sin(-30^\circ)=-0.5
\]

Therefore:

\[
\sin(-30^\circ)
=
-\sin(30^\circ)
\]

---

# Supplementary Sine Identity

Sine also satisfies:

\[
\sin(\theta)
=
\sin(\pi-\theta)
\]

---

## Example

Let:

\[
\theta=30^\circ
\]

Then:

\[
180^\circ-30^\circ
=
150^\circ
\]

Now:

\[
\sin(30^\circ)=0.5
\]

\[
\sin(150^\circ)=0.5
\]

Therefore:

\[
\sin(\theta)
=
\sin(\pi-\theta)
\]

---

# Real-Life Analogy

Imagine throwing a ball.

The ball reaches the same height:

```text
Before the peak
```

and

```text
After the peak
```

This mirror behavior resembles sine symmetry.

---

# 3. Periodicity of Trigonometric Functions

## What is Periodicity?

A function is periodic if it repeats the same pattern forever.

---

# Everyday Example

A clock repeats every:

```text
12 hours
```

After 12 hours:

```text
Pattern repeats.
```

---

# Sine Periodicity

Sine repeats every:

\[
2\pi
\]

Therefore:

\[
\sin(x+2n\pi)
=
\sin(x)
\]

---

## Example

\[
\sin(30^\circ)
=
0.5
\]

Add one full cycle:

\[
30^\circ+360^\circ
=
390^\circ
\]

Then:

\[
\sin(390^\circ)
=
0.5
\]

---

# Cosine Periodicity

Cosine also repeats every:

\[
2\pi
\]

Thus:

\[
\cos(x+2n\pi)
=
\cos(x)
\]

---

## Example

\[
\cos(60^\circ)
=
0.5
\]

\[
\cos(420^\circ)
=
0.5
\]

---

# Tangent Periodicity

Tangent repeats faster.

Its period is:

\[
\pi
\]

Therefore:

\[
\tan(x+n\pi)
=
\tan(x)
\]

---

## Example

\[
\tan(45^\circ)
=
1
\]

Add:

\[
180^\circ
\]

\[
\tan(225^\circ)
=
1
\]

---

# Period Summary

| Function | Period |
|-----------|---------|
| sin(x) | \(2\pi\) |
| cos(x) | \(2\pi\) |
| tan(x) | \(\pi\) |

---

# 4. Graph Transformations and Wave Properties

Consider the general wave:

\[
y=A\sin(Bx-C)
\]

---

# Amplitude (A)

Amplitude measures:

```text
Wave Height
```

---

## Standard Sine Wave

\[
y=\sin(x)
\]

Maximum:

```text
1
```

Minimum:

```text
-1
```

Amplitude:

```text
1
```

---

## Example

\[
y=3\sin(x)
\]

Maximum:

```text
3
```

Minimum:

```text
-3
```

Amplitude:

```text
3
```

---

## Visualization

```text
Normal Wave

   1
---+---
  -1

Stretched Wave

   3
---+---
  -3
```

---

# Period Adjustment (B)

B changes the horizontal speed.

Formula:

\[
\text{Period}
=
\frac{2\pi}{B}
\]

---

## Example 1

\[
y=\sin(2x)
\]

Period:

\[
\frac{2\pi}{2}
=
\pi
\]

Wave repeats twice as fast.

---

## Example 2

\[
y=\sin\left(\frac{x}{2}\right)
\]

Period:

\[
\frac{2\pi}{1/2}
=
4\pi
\]

Wave stretches horizontally.

---

# Phase Shift (C)

The value inside the brackets moves the graph sideways.

---

## Right Shift

\[
y=\sin(x-2)
\]

Moves:

```text
2 units right
```

---

## Left Shift

\[
y=\sin(x+2)
\]

Moves:

```text
2 units left
```

---

# Real-Life Example

Different musical notes have:

- Different amplitudes (volume)
- Different frequencies (pitch)

These transformations model those differences.

---

# 5. Complementary Shift Linking Sine and Cosine

## Relationship

Sine and cosine have the same shape.

The only difference is their starting position.

---

# Identity

\[
\sin\left(x+\frac{\pi}{2}\right)
=
\cos(x)
\]

---

## Meaning

Move the sine graph left by:

\[
\frac{\pi}{2}
\]

and it becomes a cosine graph.

---

## Example

Let:

\[
x=0
\]

Then:

\[
\sin\left(0+\frac{\pi}{2}\right)
=
\sin\left(\frac{\pi}{2}\right)
=
1
\]

and

\[
\cos(0)
=
1
\]

Both match.

---

# Visualization

```text
Cosine

*------*

Sine

    *------*
```

The graphs are identical but shifted.

---

# Real-Life Analogy

Imagine two runners on the same circular track.

One starts:

```text
90° ahead
```

Their motion pattern is identical but shifted.

---

# 6. Compound Angle Identities

These formulas help calculate:

\[
(\alpha+\beta)
\]

or

\[
(\alpha-\beta)
\]

without measuring directly.

---

# Cosine Addition Formula

\[
\cos(\alpha+\beta)
=
\cos\alpha\cos\beta
-
\sin\alpha\sin\beta
\]

---

# Cosine Subtraction Formula

\[
\cos(\alpha-\beta)
=
\cos\alpha\cos\beta
+
\sin\alpha\sin\beta
\]

---

# Example

Find:

\[
\cos(75^\circ)
\]

Write:

\[
75^\circ
=
45^\circ+30^\circ
\]

Use formula:

\[
\cos(75^\circ)
=
\cos45^\circ\cos30^\circ
-
\sin45^\circ\sin30^\circ
\]

Substitute values:

\[
=
\frac{1}{\sqrt2}\cdot\frac{\sqrt3}{2}
-
\frac{1}{\sqrt2}\cdot\frac12
\]

which gives the exact answer.

---

# Sine Addition Formula

\[
\sin(\alpha+\beta)
=
\sin\alpha\cos\beta
+
\cos\alpha\sin\beta
\]

---

# Sine Subtraction Formula

\[
\sin(\alpha-\beta)
=
\sin\alpha\cos\beta
-
\cos\alpha\sin\beta
\]

---

# Example

Find:

\[
\sin(75^\circ)
\]

Write:

\[
75^\circ
=
45^\circ+30^\circ
\]

Then:

\[
\sin(75^\circ)
=
\sin45^\circ\cos30^\circ
+
\cos45^\circ\sin30^\circ
\]

---

# Why Are These Useful?

They allow calculation of many exact trigonometric values.

Used extensively in:

- Physics
- Signal processing
- Engineering
- Computer graphics

---

# 7. Double-Angle Identities

## What is a Double Angle?

A double angle means:

```text
Twice an angle
```

Example:

\[
2\alpha
\]

---

# Double-Angle Sine

\[
\sin(2\alpha)
=
2\sin\alpha\cos\alpha
\]

---

## Example

Let:

\[
\alpha=30^\circ
\]

Then:

\[
\sin(60^\circ)
=
2\sin30^\circ\cos30^\circ
\]

\[
=
2\times\frac12\times\frac{\sqrt3}{2}
\]

\[
=
\frac{\sqrt3}{2}
\]

Correct.

---

# Double-Angle Cosine

\[
\cos(2\alpha)
=
\cos^2\alpha
-
\sin^2\alpha
\]

---

## Example

Let:

\[
\alpha=30^\circ
\]

Then:

\[
\cos(60^\circ)
=
\left(\frac{\sqrt3}{2}\right)^2
-
\left(\frac12\right)^2
\]

\[
=
\frac34-\frac14
\]

\[
=
\frac12
\]

Correct.

---

# Why Double-Angle Identities Matter

They connect:

```text
One angle
```

with

```text
Twice that angle
```

and appear throughout advanced mathematics.

---

# Quick Formula Sheet

## Even/Odd Functions

\[
\cos(-x)=\cos(x)
\]

\[
\sin(-x)=-\sin(x)
\]

---

## Supplementary Identities

\[
\sin(\theta)=\sin(\pi-\theta)
\]

\[
\cos(\theta)=-\cos(\pi-\theta)
\]

---

## Periodicity

\[
\sin(x+2n\pi)=\sin(x)
\]

\[
\cos(x+2n\pi)=\cos(x)
\]

\[
\tan(x+n\pi)=\tan(x)
\]

---

## Compound Angles

\[
\sin(\alpha+\beta)
=
\sin\alpha\cos\beta+\cos\alpha\sin\beta
\]

\[
\sin(\alpha-\beta)
=
\sin\alpha\cos\beta-\cos\alpha\sin\beta
\]

\[
\cos(\alpha+\beta)
=
\cos\alpha\cos\beta-\sin\alpha\sin\beta
\]

\[
\cos(\alpha-\beta)
=
\cos\alpha\cos\beta+\sin\alpha\sin\beta
\]

---

## Double Angles

\[
\sin(2\alpha)
=
2\sin\alpha\cos\alpha
\]

\[
\cos(2\alpha)
=
\cos^2\alpha-\sin^2\alpha
\]

---

# Final Key Idea

Trigonometric functions are not random curves. They possess powerful patterns:

- **Cosine** is an even function (mirror symmetry).
- **Sine** is an odd function (rotational symmetry).
- Both repeat forever through **periodicity**.
- Their graphs can be stretched, compressed, and shifted using transformations.
- Sine and cosine are the same wave separated by a **90° phase shift**.
- Compound-angle and double-angle identities allow us to compute new angles from known ones.

These patterns form the mathematical foundation of waves, sound, electricity, communications, physics, engineering, machine learning, and signal processing.
