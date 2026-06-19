# Special Derivatives: Polynomials, Exponentials, Logarithms, and Trigonometric Functions

---

# Introduction

So far, we have learned the **Power Rule**:

\[
\frac{d}{dx}(x^n)=nx^{n-1}
\]

This rule allows us to differentiate polynomial functions such as:

\[
x^2,\quad x^3,\quad x^5,\quad x^{100}
\]

However, mathematics contains many important functions that are **not polynomials**, including:

- Exponential functions (\(e^x\))
- Logarithmic functions (\(\ln x\))
- Trigonometric functions (\(\sin x,\cos x,\tan x\))

These functions have their own special derivative rules.

---

# 1. Review of the General Polynomial Rule

---

## The Power Rule

For any polynomial term:

\[
x^n
\]

the derivative is:

\[
\boxed{
\frac{d}{dx}(x^n)=nx^{n-1}
}
\]

---

# What Does the Rule Mean?

Differentiation performs two actions:

### Step 1

Bring the exponent down to the front.

### Step 2

Reduce the exponent by 1.

---

# Example 1

\[
\frac{d}{dx}(x^4)
\]

Bring down 4:

\[
4x^{4-1}
\]

Answer:

\[
\boxed{4x^3}
\]

---

# Example 2

\[
\frac{d}{dx}(x^7)
\]

Answer:

\[
\boxed{7x^6}
\]

---

# Example 3

\[
\frac{d}{dx}(5x^3)
\]

Differentiate:

\[
5(3)x^2
\]

Answer:

\[
\boxed{15x^2}
\]

---

# Example 4

\[
\frac{d}{dx}(2x^5+4x^2+7)
\]

Differentiate term-by-term:

\[
10x^4+8x+0
\]

Answer:

\[
\boxed{10x^4+8x}
\]

---

# Real-Life Example

Suppose:

\[
s(t)=t^4
\]

represents distance.

Velocity:

\[
v(t)=4t^3
\]

The derivative tells us how quickly the distance changes.

---

# Easy Memory Rule

**Bring the power down and subtract one from the exponent.**

---

# 2. The Derivative of \(e^x\)

---

# What Is \(e\)?

\(e\) is a special mathematical constant:

\[
e\approx2.718281828
\]

It is similar to:

\[
\pi\approx3.14159
\]

because it continues forever without repeating.

---

# Why Is \(e\) Special?

Most functions change when differentiated.

Example:

\[
x^2 \rightarrow 2x
\]

---

But:

\[
e^x
\]

remains exactly the same.

---

# Derivative Rule

\[
\boxed{
\frac{d}{dx}(e^x)=e^x
}
\]

---

# Example 1

Differentiate:

\[
e^x
\]

Answer:

\[
e^x
\]

---

# Example 2

At:

\[
x=0
\]

Function value:

\[
e^0=1
\]

Derivative:

\[
e^0=1
\]

---

Function value equals slope.

---

# Example 3

At:

\[
x=2
\]

Function value:

\[
e^2
\approx7.389
\]

Derivative:

\[
e^2
\approx7.389
\]

Again identical.

---

# Why Is This Amazing?

For every point:

\[
\text{Value}=\text{Slope}
\]

---

# Visual Interpretation

Imagine a population that grows proportionally to its current size.

The larger it becomes, the faster it grows.

This naturally creates:

\[
e^x
\]

---

# Real-Life Applications

- Population growth
- Compound interest
- Radioactive decay
- Machine learning
- Probability theory

---

# Easy Memory Rule

**\(e^x\) is the only function whose derivative is itself.**

---

# 3. The Derivative of \(\ln x\) (Natural Logarithm)

---

# What Is \(\ln x\)?

\[
\ln x
\]

means:

\[
\log_e x
\]

---

It is the inverse function of:

\[
e^x
\]

---

# Relationship

\[
e^{\ln x}=x
\]

and

\[
\ln(e^x)=x
\]

---

# Derivative Rule

\[
\boxed{
\frac{d}{dx}(\ln x)=\frac1x
}
\]

---

# Example 1

Differentiate:

\[
\ln x
\]

Answer:

\[
\frac1x
\]

---

# Example 2

Find slope at:

\[
x=2
\]

Derivative:

\[
\frac12
\]

---

Slope:

\[
0.5
\]

---

# Example 3

Find slope at:

\[
x=10
\]

Derivative:

\[
\frac1{10}
\]

---

Slope:

\[
0.1
\]

---

Notice:

As x increases, the slope decreases.

---

# Real-Life Example

Suppose:

\[
y=\ln x
\]

represents learning progress.

Initially learning happens quickly.

Later improvements become slower.

This produces a logarithmic shape.

---

# Visual Pattern

| x | \(1/x\) |
|---|---|
|1|1|
|2|0.5|
|5|0.2|
|10|0.1|
|100|0.01|

---

# Easy Memory Rule

**The derivative of \(\ln x\) is always \(1/x\).**

---

# 4. The Derivatives of Sine and Cosine

---

# Derivative of Sine

\[
\boxed{
\frac{d}{dx}(\sin x)=\cos x
}
\]

---

# Example 1

Differentiate:

\[
\sin x
\]

Answer:

\[
\cos x
\]

---

# Example 2

At:

\[
x=0
\]

Derivative:

\[
\cos0=1
\]

---

Slope equals 1.

---

# Visual Meaning

The sine wave changes exactly like the cosine wave.

---

# Derivative of Cosine

\[
\boxed{
\frac{d}{dx}(\cos x)=-\sin x
}
\]

---

# Example 1

Differentiate:

\[
\cos x
\]

Answer:

\[
-\sin x
\]

---

# Example 2

At:

\[
x=0
\]

Derivative:

\[
-\sin0=0
\]

---

Slope equals zero.

---

# Important Exam Mistake

Many students forget:

\[
\boxed{
\frac{d}{dx}(\cos x)=-\sin x
}
\]

The negative sign is extremely important.

---

# Visual Memory Trick

Sine becomes cosine.

Cosine becomes negative sine.

---

# Cycle of Derivatives

Differentiate repeatedly:

\[
\sin x
\]

↓

\[
\cos x
\]

↓

\[
-\sin x
\]

↓

\[
-\cos x
\]

↓

\[
\sin x
\]

(back to start)

---

# Real-Life Example

Sine and cosine model:

- Waves
- Sound
- Electricity
- Vibrations
- Rotating wheels

---

# Easy Memory Rule

\[
\sin x \rightarrow \cos x
\]

\[
\cos x \rightarrow -\sin x
\]

---

# 5. The Derivative of Tangent

---

# What Is Tangent?

\[
\tan x
=
\frac{\sin x}{\cos x}
\]

---

# Derivative Rule

\[
\boxed{
\frac{d}{dx}(\tan x)
=
\frac1{\cos^2x}
}
\]

---

This is also written as:

\[
\boxed{
\sec^2x
}
\]

because:

\[
\sec x=\frac1{\cos x}
\]

---

# Example 1

Differentiate:

\[
\tan x
\]

Answer:

\[
\sec^2x
\]

---

# Example 2

At:

\[
x=0
\]

Derivative:

\[
\frac1{\cos^20}
\]

---

Since:

\[
\cos0=1
\]

---

Answer:

\[
1
\]

---

# Example 3

At:

\[
x=\frac{\pi}{3}
\]

---

\[
\cos\left(\frac{\pi}{3}\right)=\frac12
\]

---

Derivative:

\[
\frac1{(1/2)^2}
\]

\[
=4
\]

---

Slope equals 4.

---

# Why Does Tangent Grow So Fast?

Near:

\[
x=\frac{\pi}{2}
\]

cosine approaches zero.

---

Since:

\[
\frac1{\cos^2x}
\]

has a tiny denominator,

the derivative becomes huge.

---

# Real-Life Example

Tangent functions appear in:

- Navigation
- Surveying
- Engineering
- Computer graphics
- Camera angles

---

# Easy Memory Rule

**The derivative of tangent is secant squared.**

---

# Quick Derivative Summary Table

| Function | Derivative |
|-----------|-----------|
| \(c\) | \(0\) |
| \(x^n\) | \(nx^{n-1}\) |
| \(e^x\) | \(e^x\) |
| \(\ln x\) | \(1/x\) |
| \(\sin x\) | \(\cos x\) |
| \(\cos x\) | \(-\sin x\) |
| \(\tan x\) | \(\sec^2 x\) |

---

# Complete Summary

---

## Polynomial Rule

\[
\frac{d}{dx}(x^n)=nx^{n-1}
\]

---

## Exponential Rule

\[
\frac{d}{dx}(e^x)=e^x
\]

The function equals its own derivative.

---

## Logarithm Rule

\[
\frac{d}{dx}(\ln x)=\frac1x
\]

---

## Trigonometric Rules

\[
\frac{d}{dx}(\sin x)=\cos x
\]

\[
\frac{d}{dx}(\cos x)=-\sin x
\]

\[
\frac{d}{dx}(\tan x)=\sec^2 x
\]

---

## Most Common Exam Error

Forgetting the negative sign:

\[
\frac{d}{dx}(\cos x)=-\sin x
\]

---

### One-Sentence Memory Rule

**The most important derivative formulas beyond the Power Rule are \(e^x \rightarrow e^x\), \(\ln x \rightarrow 1/x\), \(\sin x \rightarrow \cos x\), \(\cos x \rightarrow -\sin x\), and \(\tan x \rightarrow \sec^2x\), all of which appear repeatedly throughout calculus, physics, and engineering.**