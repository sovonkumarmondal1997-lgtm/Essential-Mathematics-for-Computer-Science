# Basic Differentiation Rules — Constants, Linear Functions, Negative Powers, and Polynomials

---

# Introduction

After proving the Power Rule:

\[
\frac{d}{dx}(x^n)=nx^{n-1}
\]

we can now differentiate many functions quickly.

These rules are the foundation of calculus and are used everywhere in:

- Physics
- Engineering
- Data Science
- Machine Learning
- Economics
- Computer Graphics

The good news is that the rules are simple and follow clear patterns.

---

# 1. The Derivative of a Constant is Zero

---

## What Is a Constant?

A constant is a number that never changes.

Examples:

\[
3
\]

\[
7
\]

\[
100
\]

\[
-5
\]

\[
\pi
\]

---

## Example

Consider:

\[
f(x)=3
\]

No matter what value of \(x\) you choose:

| x | f(x) |
|---|---|
| 1 | 3 |
| 5 | 3 |
| 100 | 3 |

The output never changes.

---

# Geometric View

The graph is a horizontal line.

```
3 ──────────────────
```

---

A horizontal line has slope:

\[
0
\]

everywhere.

Therefore:

\[
\boxed{
\frac{d}{dx}(3)=0
}
\]

---

# More Examples

---

## Example 1

\[
\frac{d}{dx}(10)=0
\]

---

## Example 2

\[
\frac{d}{dx}(500)=0
\]

---

## Example 3

\[
\frac{d}{dx}(\pi)=0
\]

---

## Example 4

\[
\frac{d}{dx}(-8)=0
\]

---

# Real-Life Example

Imagine your bank account always contains:

₹1000

every day.

No increase.

No decrease.

Change rate:

\[
0
\]

Derivative:

\[
0
\]

---

# Easy Memory Rule

**Constants never change, so their derivatives are always zero.**

---

# 2. The Derivative of a Linear Term

---

Consider:

\[
f(x)=4x
\]

---

Apply the Power Rule:

\[
\frac{d}{dx}(x^n)
=
nx^{n-1}
\]

---

Here:

\[
n=1
\]

---

Differentiate:

\[
\frac{d}{dx}(4x)
=
4\frac{d}{dx}(x)
\]

---

Apply power rule:

\[
=
4(1)x^{1-1}
\]

---

\[
=
4x^0
\]

---

Since:

\[
x^0=1
\]

---

Answer:

\[
\boxed{
\frac{d}{dx}(4x)=4
}
\]

---

# Why Does This Make Sense?

The graph:

\[
y=4x
\]

is a straight line.

---

Every straight line has one constant slope.

The slope is:

\[
4
\]

---

Therefore the derivative is:

\[
4
\]

---

# More Examples

---

## Example 1

\[
\frac{d}{dx}(7x)=7
\]

---

## Example 2

\[
\frac{d}{dx}(100x)=100
\]

---

## Example 3

\[
\frac{d}{dx}(-3x)=-3
\]

---

## Example 4

\[
\frac{d}{dx}(x)=1
\]

---

# Real-Life Example

Suppose:

\[
y=60t
\]

represents distance traveled at a constant speed.

The derivative:

\[
60
\]

means:

60 km/hour

The speed never changes.

---

# Easy Memory Rule

**The derivative of \(ax\) is simply \(a\).**

---

# 3. The Linearity / Addition Rule of Calculus

---

## The Rule

If a function contains multiple terms:

\[
f(x)=A+B+C
\]

then:

\[
f'(x)=A'+B'+C'
\]

---

In words:

Differentiate each term separately.

Then add the results.

---

# Example 1

\[
f(x)=x^2+5x
\]

---

Differentiate term-by-term:

\[
\frac{d}{dx}(x^2)=2x
\]

\[
\frac{d}{dx}(5x)=5
\]

---

Answer:

\[
\boxed{
f'(x)=2x+5
}
\]

---

# Example 2

\[
f(x)=x^3+2x^2+7
\]

---

Differentiate:

\[
3x^2
\]

\[
+4x
\]

\[
+0
\]

---

Answer:

\[
\boxed{
3x^2+4x
}
\]

---

# Example 3

\[
f(x)=5x^4+x^2+8x+10
\]

---

Derivative:

\[
20x^3+2x+8
\]

---

# Real-Life Analogy

Imagine three workers painting a wall.

Worker A paints:

20 m²

Worker B paints:

30 m²

Worker C paints:

50 m²

Total work:

\[
20+30+50
\]

Each contribution is added separately.

Differentiation works the same way.

---

# Easy Memory Rule

**Differentiate each term separately, then combine the answers.**

---

# 4. Connection to Linear Slope (\(y=mx+c\))

---

# Coordinate Geometry

You may already know:

\[
y=mx+c
\]

---

Where:

\[
m
\]

is the slope.

---

Example:

\[
y=3x+2
\]

Slope:

\[
3
\]

---

# Differentiate

\[
\frac{d}{dx}(3x+2)
\]

---

Term by term:

\[
3+0
\]

---

Answer:

\[
\boxed{
3
}
\]

---

Exactly the same slope.

---

# Another Example

\[
y=-5x+7
\]

Derivative:

\[
-5
\]

---

The slope is also:

\[
-5
\]

---

# Why Is This Important?

Calculus agrees perfectly with coordinate geometry.

The derivative of a straight line equals its slope.

---

# Visual Example

```
Positive Slope

     /
    /
   /
  /

Slope = 3
Derivative = 3
```

---

```
Negative Slope

\
 \
  \
   \

Slope = -5
Derivative = -5
```

---

# Easy Memory Rule

**For \(y=mx+c\), the derivative is always \(m\).**

---

# 5. Differentiating Negative Exponents

---

Many students think the Power Rule only works for positive exponents.

It actually works for:

- Positive powers
- Negative powers
- Fractional powers

---

# Example 1

\[
f(x)=x^{-1}
\]

Apply power rule:

\[
(-1)x^{-2}
\]

---

Answer:

\[
\boxed{
-x^{-2}
}
\]

---

Equivalent form:

\[
-\frac1{x^2}
\]

---

# Example 2

\[
f(x)=x^{-3}
\]

---

Derivative:

\[
-3x^{-4}
\]

---

Equivalent:

\[
-\frac3{x^4}
\]

---

# Example 3

\[
f(x)=5x^{-2}
\]

---

Derivative:

\[
5(-2)x^{-3}
\]

---

Answer:

\[
-10x^{-3}
\]

---

Equivalent:

\[
-\frac{10}{x^3}
\]

---

# Visual Understanding

Consider:

\[
y=\frac1x
\]

As x increases:

The curve falls.

Negative derivative indicates downward slope.

---

# Real-Life Example

Suppose:

\[
f(x)=\frac{100}{x}
\]

represents cost per person when sharing a bill.

As more people join:

Cost decreases.

Derivative becomes negative.

---

# Easy Memory Rule

**Negative exponents follow the exact same power rule.**

---

# 6. Combining Rules for Multi-Term Polynomials

---

Now we combine everything.

---

# Step-by-Step Method

For each term:

### Step 1

Multiply by its exponent.

### Step 2

Reduce exponent by 1.

### Step 3

Keep the sign.

### Step 4

Constants become 0.

---

# Example 1

\[
f(x)=3x^4+5x^2+7x+10
\]

---

Differentiate each term.

---

First term:

\[
3(4)x^3
=
12x^3
\]

---

Second term:

\[
5(2)x
=
10x
\]

---

Third term:

\[
7
\]

---

Fourth term:

\[
0
\]

---

Answer:

\[
\boxed{
12x^3+10x+7
}
\]

---

# Example 2

\[
f(x)=2x^5-4x^3+x^2-8
\]

---

Derivative:

\[
10x^4
-
12x^2
+
2x
\]

---

Answer:

\[
\boxed{
10x^4-12x^2+2x
}
\]

---

# Example 3

\[
f(x)=x^6+3x^{-2}+9
\]

---

Derivative:

\[
6x^5
-
6x^{-3}
+
0
\]

---

Answer:

\[
\boxed{
6x^5-6x^{-3}
}
\]

---

# Example 4

\[
f(x)=7x^3-2x+\frac1x
\]

---

Rewrite:

\[
7x^3-2x+x^{-1}
\]

---

Derivative:

\[
21x^2
-
2
-
x^{-2}
\]

---

Answer:

\[
\boxed{
21x^2-2-\frac1{x^2}
}
\]

---

# Master Shortcut Table

| Original | Derivative |
|-----------|-----------|
| \(c\) | 0 |
| \(x\) | 1 |
| \(x^2\) | \(2x\) |
| \(x^3\) | \(3x^2\) |
| \(x^4\) | \(4x^3\) |
| \(x^{-1}\) | \(-x^{-2}\) |
| \(x^{-2}\) | \(-2x^{-3}\) |
| \(mx+c\) | \(m\) |

---

# Complete Summary

---

## Constant Rule

\[
\frac{d}{dx}(c)=0
\]

because constants never change.

---

## Linear Rule

\[
\frac{d}{dx}(ax)=a
\]

because:

\[
x^1 \rightarrow 1x^0
\]

---

## Addition Rule

Differentiate each term separately and add the results.

---

## Straight Line Rule

For:

\[
y=mx+c
\]

the derivative is:

\[
m
\]

which is exactly the slope.

---

## Negative Exponents

The power rule still works:

\[
\frac{d}{dx}(x^{-n})
=
-nx^{-n-1}
\]

---

## Polynomial Rule

For every term:

1. Multiply by the exponent.
2. Reduce exponent by 1.
3. Constants become 0.

---

### One-Sentence Memory Rule

**To differentiate a polynomial, multiply each term by its exponent, reduce the exponent by one, keep constants as zero, and then combine all the resulting terms together.**