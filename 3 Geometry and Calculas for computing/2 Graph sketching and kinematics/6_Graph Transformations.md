# Graph Transformations: Vertical Shifts, Vertical Scaling, and Horizontal Shifts

---

# Introduction

One of the most useful skills in mathematics is understanding how a graph changes when we slightly modify its equation.

Instead of drawing a completely new graph from scratch, we can often start with a familiar graph and then:

- Move it up or down
- Stretch it taller
- Compress it flatter
- Move it left or right

These changes are called:

```text
Graph Transformations
```

Think of graph transformations like moving or resizing a picture on your computer. The picture remains the same shape, but its position or size changes.

---

# Base Graph

Throughout this lesson, we will use the simple quadratic:

\[
y=x^2
\]

as our starting graph.

---

# Original Graph

```text
      *
     * *
    *   *
   *     *
  *       *
```

This graph:

- Opens upward
- Has a turning point at:

\[
(0,0)
\]

---

# 1. Vertical Translations (Shifting Up and Down)

## What is a Vertical Translation?

A vertical translation moves the entire graph:

```text
Up
```

or

```text
Down
```

along the y-axis.

---

# Rule

### Shift Up

\[
y=f(x)+c
\]

Move graph upward by:

```text
c units
```

---

### Shift Down

\[
y=f(x)-c
\]

Move graph downward by:

```text
c units
```

---

# Why Does This Work?

The value added or subtracted affects every output.

Original:

\[
y=f(x)
\]

New:

\[
y=f(x)+c
\]

Every y-value becomes larger by c.

---

# Example 1: Shift Up

Original:

\[
y=x^2
\]

New:

\[
y=x^2+2
\]

---

# Compare Values

| x | x² | x²+2 |
|---|---|---|
| -2 | 4 | 6 |
| -1 | 1 | 3 |
| 0 | 0 | 2 |
| 1 | 1 | 3 |
| 2 | 4 | 6 |

Notice:

```text
Every output increased by 2.
```

---

# Graph Effect

Original vertex:

\[
(0,0)
\]

moves to:

\[
(0,2)
\]

---

# Visualization

Original:

```text
      *
     * *
    *   *
```

Shifted Up:

```text
      *
     * *
    *   *

      ↑ 2 units
```

---

# Example 2: Shift Down

Original:

\[
y=x^2
\]

New:

\[
y=x^2-3
\]

---

# Compare Values

| x | x² | x²−3 |
|---|---|---|
| -1 | 1 | -2 |
| 0 | 0 | -3 |
| 1 | 1 | -2 |

---

# Graph Effect

Vertex moves from:

\[
(0,0)
\]

to:

\[
(0,-3)
\]

---

# Visualization

```text
Original Vertex

(0,0)

↓

Shift Down 3

↓

(0,-3)
```

---

# Real-Life Analogy

Imagine lifting a bowl.

The shape stays exactly the same.

Only its height changes.

---

# Summary

| Equation | Effect |
|-----------|-----------|
| f(x)+5 | Up 5 |
| f(x)+2 | Up 2 |
| f(x)-1 | Down 1 |
| f(x)-4 | Down 4 |

---

# 2. Vertical Stretching and Shrinking (Scaling)

## What is Vertical Scaling?

Vertical scaling changes the height of the graph.

The graph becomes:

```text
Taller
```

or

```text
Flatter
```

---

# Rule

\[
y=mf(x)
\]

where:

```text
m = scaling factor
```

---

# Stretching

If:

\[
m>1
\]

the graph stretches vertically.

---

# Example

\[
y=6x^2
\]

Every output becomes:

```text
6 times larger
```

---

# Compare Values

| x | x² | 6x² |
|---|---|---|
| -2 | 4 | 24 |
| -1 | 1 | 6 |
| 0 | 0 | 0 |
| 1 | 1 | 6 |
| 2 | 4 | 24 |

---

# Effect

The parabola becomes narrower and taller.

---

# Visualization

Original:

```text
      *
     * *
    *   *
```

Stretched:

```text
       *
      * *
     *   *
    *     *
```

---

# Example: Sine Wave Stretch

Original:

\[
y=\sin(x)
\]

Amplitude:

```text
1
```

---

New:

\[
y=3\sin(x)
\]

Amplitude:

```text
3
```

---

# Values

Original range:

```text
-1 to 1
```

New range:

```text
-3 to 3
```

---

# Shrinking / Compressing

If:

\[
0<m<1
\]

the graph compresses vertically.

---

# Example

\[
y=\frac12 x^2
\]

---

# Compare Values

| x | x² | (1/2)x² |
|---|---|---|
| -2 | 4 | 2 |
| -1 | 1 | 0.5 |
| 0 | 0 | 0 |
| 1 | 1 | 0.5 |
| 2 | 4 | 2 |

---

# Effect

The graph becomes flatter and wider.

---

# Visualization

Original:

```text
      *
     * *
    *   *
```

Compressed:

```text
    *     *
      * *
        *
```

---

# Real-Life Analogy

Think of a rubber band.

Stretch it vertically:

```text
Taller graph
```

Compress it:

```text
Flatter graph
```

---

# Summary

| Scale Factor | Effect |
|-------------|---------|
| m = 6 | Stretch by 6 |
| m = 3 | Stretch by 3 |
| m = 1 | No change |
| m = 1/2 | Compress by half |
| m = 1/4 | Compress by quarter |

---

# 3. Horizontal Translations (Shifting Left and Right)

## What is a Horizontal Translation?

A horizontal translation moves the graph:

```text
Left
```

or

```text
Right
```

along the x-axis.

---

# Important Warning

Horizontal shifts feel backwards.

---

# Rule

### Right Shift

\[
y=f(x-a)
\]

moves graph:

```text
Right by a units
```

---

### Left Shift

\[
y=f(x+a)
\]

moves graph:

```text
Left by a units
```

---

# Why Does It Look Backwards?

Suppose:

\[
(x-2)^2
\]

To make the inside zero:

\[
x=2
\]

Therefore the turning point moves to:

\[
(2,0)
\]

which is 2 units right.

---

# Example 1: Shift Right

Original:

\[
y=x^2
\]

New:

\[
y=(x-2)^2
\]

---

# Compare Vertices

Original:

\[
(0,0)
\]

New:

\[
(2,0)
\]

---

# Visualization

```text
Original

      *
     * *
    *   *

Shift Right

           *
          * *
         *   *
```

---

# Example Values

| x | (x−2)² |
|---|---|
| 2 | 0 |
| 3 | 1 |
| 4 | 4 |

Notice:

The graph behaves exactly like \(x^2\) but starts at x = 2.

---

# Example 2: Shift Left

Original:

\[
y=x^2
\]

New:

\[
y=(x+2)^2
\]

---

# Vertex

Original:

\[
(0,0)
\]

moves to:

\[
(-2,0)
\]

---

# Visualization

```text
Shift Left

      *
     * *
    *   *

← 2 units
```

---

# Example Values

| x | (x+2)² |
|---|---|
| -2 | 0 |
| -1 | 1 |
| 0 | 4 |

---

# Real-Life Analogy

Imagine moving a chair across a room.

The chair's shape never changes.

Only its position changes.

Horizontal translations do the same thing to graphs.

---

# Combining Transformations

Graphs can experience multiple transformations at once.

---

# Example

\[
y=2(x-3)^2+4
\]

---

# Analyze Step-by-Step

Starting graph:

\[
y=x^2
\]

---

### (x−3)

Move right:

```text
3 units
```

---

### +4

Move up:

```text
4 units
```

---

### 2×

Stretch vertically:

```text
Factor of 2
```

---

# Final Result

The graph is:

- Shifted right 3
- Shifted up 4
- Stretched vertically by 2

---

# Quick Transformation Summary

## Vertical Shifts

\[
f(x)+c
\]

```text
Move Up c
```

---

\[
f(x)-c
\]

```text
Move Down c
```

---

## Vertical Scaling

\[
mf(x)
\]

```text
Stretch if m > 1
```

```text
Compress if 0 < m < 1
```

---

## Horizontal Shifts

\[
f(x-a)
\]

```text
Move Right a
```

---

\[
f(x+a)
\]

```text
Move Left a
```

---

# Visual Memory Trick

### Outside the Function

\[
f(x)+3
\]

```text
Normal Direction
```

Up 3.

---

### Inside the Function

\[
f(x-3)
\]

```text
Opposite Direction
```

Right 3.

---

# Complete Summary Table

| Transformation | Equation | Effect |
|---------------|-----------|---------|
| Shift Up | f(x)+c | Up c |
| Shift Down | f(x)-c | Down c |
| Stretch | mf(x), m>1 | Taller |
| Compress | mf(x), 0<m<1 | Flatter |
| Shift Right | f(x-a) | Right a |
| Shift Left | f(x+a) | Left a |

---

# Final Key Idea

Most graph transformations can be understood using three simple operations:

### Move Up or Down

\[
f(x)\pm c
\]

---

### Stretch or Compress

\[
m f(x)
\]

---

### Move Left or Right

\[
f(x\pm a)
\]

The most important thing to remember is:

```text
Outside the function → Normal direction
Inside the function → Opposite direction
```

Understanding these transformations allows you to sketch complex graphs quickly and forms the foundation for calculus, physics, engineering, computer graphics, signal processing, machine learning, and data visualization.
