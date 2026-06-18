# Infinity, Limits, Convergence, and Divergence of Sequences

---

# Introduction

In previous chapters, we learned:

- Sequences
- Arithmetic Sequences
- Geometric Sequences
- Prime Numbers
- Series
- Explicit Formulas

Now we move to one of the most important ideas in mathematics:

# Limits

Limits help answer questions such as:

- What happens if a sequence continues forever?
- Does it approach a particular value?
- Does it grow without bound?
- Does it settle down or explode?

These concepts are fundamental in:

- Calculus
- Machine Learning
- Physics
- Engineering
- Data Science
- Probability
- Mathematical Analysis

---

# 1. Infinity (\(\infty\))

## Simple Definition

Infinity is the idea of something continuing forever without end.

---

## Symbol

\[
\infty
\]

---

## Example 1

Natural numbers:

\[
1,2,3,4,5,\dots
\]

The dots:

\[
\dots
\]

mean:

"Keep going forever."

---

## Example 2

Even numbers:

\[
2,4,6,8,10,\dots
\]

No largest even number exists.

---

## Example 3

Odd numbers:

\[
1,3,5,7,9,\dots
\]

Continue forever.

---

## Important Note

Infinity is NOT an ordinary number.

You cannot reach infinity by counting.

It is an idea describing endless growth.

---

## Real-Life Example

Imagine counting stars:

```
1
2
3
4
...
```

You never finish counting.

---

## Visual Idea

```
→→→→→→→→→→→→→
```

Keeps going forever.

---

# Why Infinity Matters

Many mathematical patterns become interesting only when we ask:

> What happens as we continue forever?

---

# 2. Limit of a Sequence

## Simple Definition

The limit of a sequence is the value that the terms get closer and closer to as:

\[
n \to \infty
\]

---

## Mathematical Notation

\[
\lim_{n\to\infty} u_n
\]

---

## Example 1

Sequence:

\[
1,\frac12,\frac13,\frac14,\frac15,\dots
\]

---

Terms:

\[
1
\]

\[
0.5
\]

\[
0.333
\]

\[
0.25
\]

\[
0.2
\]

---

Getting closer to:

\[
0
\]

---

Limit:

\[
\lim_{n\to\infty}\frac1n=0
\]

---

## Example 2

Sequence:

\[
10,\;5,\;2.5,\;1.25,\dots
\]

Approaches:

\[
0
\]

---

## Example 3

Sequence:

\[
5,\;5,\;5,\;5,\dots
\]

Limit:

\[
5
\]

---

## Real-Life Example

A bouncing ball:

```
10m
5m
2.5m
1.25m
...
```

The bounce height approaches zero.

---

# Why Limits Matter

Limits describe the long-term behavior of sequences.

---

# 3. Divergent Sequence / Divergent Series

## Simple Definition

A sequence is divergent if it does NOT approach a finite value.

---

Instead, it may:

- Grow forever
- Decrease forever
- Oscillate endlessly

---

## Example 1

\[
1,2,3,4,5,\dots
\]

Grows forever.

---

Limit:

\[
\infty
\]

---

Divergent.

---

## Example 2

\[
1,4,9,16,25,\dots
\]

Grows forever.

---

Divergent.

---

## Example 3

\[
1,-1,1,-1,1,-1,\dots
\]

Never settles.

---

Divergent.

---

## Visual

```
↑
↑
↑
↑
↑
```

Keeps growing.

---

# Real-Life Example

Population doubling forever without limit.

No stable value.

---

# 4. Divergence of Polynomial Sequences

## Simple Definition

Polynomial sequences grow larger and larger as:

\[
n
\]

increases.

---

# Example 1: Natural Numbers

Formula:

\[
u_n=n
\]

---

Sequence:

\[
1,2,3,4,5,\dots
\]

---

As:

\[
n\to\infty
\]

values become larger forever.

---

Limit:

\[
\infty
\]

---

Divergent.

---

# Example 2: Perfect Squares

Formula:

\[
u_n=n^2
\]

---

Sequence:

\[
1,4,9,16,25,\dots
\]

---

Growth becomes faster.

---

Limit:

\[
\infty
\]

---

Divergent.

---

# Example 3: Cubes

\[
u_n=n^3
\]

---

Sequence:

\[
1,8,27,64,125,\dots
\]

---

Also divergent.

---

## Important Observation

Polynomial growth never settles.

It keeps increasing forever.

---

# 5. Geometric Sequence Divergence Condition

## Rule

A geometric sequence:

\[
u_n=ar^{n-1}
\]

diverges when:

\[
r>1
\]

---

# Example 1

\[
1,2,4,8,16,\dots
\]

---

Ratio:

\[
r=2
\]

---

Values grow forever.

---

Divergent.

---

# Example 2

\[
3,6,12,24,\dots
\]

---

Ratio:

\[
r=2
\]

---

Divergent.

---

# Example 3

\[
5,15,45,135,\dots
\]

---

Ratio:

\[
r=3
\]

---

Divergent.

---

## Real-Life Example

Compound interest.

Money keeps growing exponentially.

---

# Why?

Each term becomes larger than the previous one.

Growth accelerates.

---

# 6. Convergent Sequence / Convergent Series

## Simple Definition

A sequence is convergent if it approaches a finite value.

---

The terms get closer and closer to a particular number.

---

## Example 1

\[
1,\frac12,\frac14,\frac18,\frac1{16},\dots
\]

---

Approaches:

\[
0
\]

---

Convergent.

---

## Example 2

\[
5,\;5,\;5,\;5,\dots
\]

---

Approaches:

\[
5
\]

---

Convergent.

---

## Example 3

\[
10,\;9,\;8.5,\;8.25,\dots
\]

Approaches:

\[
8
\]

---

Convergent.

---

## Real-Life Example

A cooling cup of coffee.

Temperature approaches room temperature.

---

# Key Idea

Convergence means:

```
Settles Down
```

Divergence means:

```
Runs Away
```

---

# 7. Geometric Sequence Convergence Condition

## Rule

For geometric sequences:

\[
u_n=ar^{n-1}
\]

---

If:

\[
0<r<1
\]

the sequence converges to:

\[
0
\]

---

# Example 1

\[
1,\frac12,\frac14,\frac18,\dots
\]

---

Ratio:

\[
r=\frac12
\]

---

Limit:

\[
0
\]

---

# Example 2

\[
10,5,2.5,1.25,\dots
\]

---

Ratio:

\[
r=\frac12
\]

---

Limit:

\[
0
\]

---

# Example 3

\[
100,10,1,0.1,0.01,\dots
\]

---

Ratio:

\[
0.1
\]

---

Limit:

\[
0
\]

---

## Why?

Multiplying repeatedly by a fraction shrinks the values.

---

# Real-Life Example

A bouncing ball losing half its height each bounce.

Eventually approaches ground level.

---

# 8. Asymptotic Approach

## Simple Definition

A sequence can get closer and closer to a value without ever actually reaching it.

---

This behavior is called:

# Asymptotic Approach

---

# Example 1

\[
1,\frac12,\frac14,\frac18,\dots
\]

---

Values:

\[
1
\]

\[
0.5
\]

\[
0.25
\]

\[
0.125
\]

---

Approach:

\[
0
\]

but never equal 0.

---

## Visual

```
1
|
0.5
|
0.25
|
0.125
|
0.0625
|
0
```

Closer and closer.

---

# Example 2

Distance remaining:

```
100m
50m
25m
12.5m
...
```

Approaches:

```
0m
```

---

# Example 3

A cooling object.

Temperature gets closer to room temperature.

---

# Important Idea

Approaching is enough.

The sequence does NOT need to actually reach the limit.

---

# 9. Boundary Condition Convergence (\(r=1\))

## Special Case

Consider:

\[
u_n=ar^{n-1}
\]

with:

\[
r=1
\]

---

Formula becomes:

\[
u_n=a(1)^{n-1}
\]

---

\[
u_n=a
\]

---

Every term is identical.

---

# Example 1

\[
5,5,5,5,5,\dots
\]

---

Limit:

\[
5
\]

---

Convergent.

---

# Example 2

\[
100,100,100,100,\dots
\]

---

Limit:

\[
100
\]

---

Convergent.

---

# Example 3

\[
-3,-3,-3,-3,\dots
\]

---

Limit:

\[
-3
\]

---

Convergent.

---

## Why Is This Special?

The sequence neither:

- grows
- shrinks

It remains constant forever.

---

# Comparison of Geometric Sequences

### Case 1

\[
r>1
\]

Example:

\[
1,2,4,8,\dots
\]

Diverges.

---

### Case 2

\[
0<r<1
\]

Example:

\[
1,\frac12,\frac14,\dots
\]

Converges to 0.

---

### Case 3

\[
r=1
\]

Example:

\[
5,5,5,5,\dots
\]

Converges to 5.

---

# Complete Big Picture

## Infinity

\[
\infty
\]

Means endless continuation.

---

## Limit

The value a sequence approaches as:

\[
n\to\infty
\]

---

## Divergent Sequence

Does not settle to a finite value.

Examples:

\[
n
\]

\[
n^2
\]

\[
2^n
\]

---

## Polynomial Divergence

\[
n,\;n^2,\;n^3
\]

all grow forever.

---

## Geometric Divergence

If:

\[
r>1
\]

the sequence diverges.

---

## Convergent Sequence

Approaches a finite value.

---

## Geometric Convergence

If:

\[
0<r<1
\]

the sequence converges to:

\[
0
\]

---

## Asymptotic Approach

Gets infinitely close to a value without necessarily reaching it.

---

## Boundary Case

\[
r=1
\]

Produces a constant sequence.

Still convergent.

---

These concepts form the foundation for:

- Calculus
- Infinite Series
- Differential Equations
- Probability Theory
- Statistics
- Signal Processing
- Machine Learning
- Optimization
- Numerical Analysis
- Deep Learning

where understanding long-term behavior and limits is essential.