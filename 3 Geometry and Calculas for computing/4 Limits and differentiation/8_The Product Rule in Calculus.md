# The Product Rule in Calculus — Complete Notes with Examples

---

# Introduction

So far, we have learned how to differentiate:

- Polynomials
- Exponential functions
- Logarithms
- Trigonometric functions

Examples:

\[
x^5
\]

\[
e^x
\]

\[
\sin x
\]

\[
\ln x
\]

But what happens when two functions are multiplied together?

Example:

\[
x^2 e^x
\]

\[
x\sin x
\]

\[
\sin x\cos x
\]

These cannot be differentiated by simply differentiating each part separately and multiplying the results.

Instead, we use one of the most important rules in calculus:

\[
\boxed{\text{The Product Rule}}
\]

---

# 1. Introduction to the Product Rule

---

## Why Do We Need the Product Rule?

Suppose we have:

\[
f(x)=x^2e^x
\]

This function contains:

- A polynomial (\(x^2\))
- An exponential (\(e^x\))

multiplied together.

---

If we incorrectly differentiate both separately and multiply:

\[
(2x)(e^x)
\]

we miss part of the answer.

---

The reason is:

Both pieces are changing simultaneously.

The derivative must account for both changes.

---

# Real-Life Analogy

Imagine a company's profit depends on:

\[
\text{Price} \times \text{Sales}
\]

If both price and sales change,

the total profit change depends on:

- Change in price
- Change in sales

You must consider both effects.

---

The Product Rule does exactly this.

---

# Easy Memory Rule

**When two functions are multiplied, both functions get a turn being differentiated.**

---

# 2. Algebraic Definition of the Product Rule

---

Suppose:

\[
f(x)=g(x)h(x)
\]

where:

- \(g(x)\) is the first function
- \(h(x)\) is the second function

---

The Product Rule states:

\[
\boxed{
f'(x)
=
g'(x)h(x)
+
g(x)h'(x)
}
\]

---

# In Words

Differentiate the first function.

Leave the second alone.

PLUS

Leave the first alone.

Differentiate the second.

---

# Memory Phrase

Many students memorize:

> Differentiate the first, keep the second.  
> Plus keep the first, differentiate the second.

---

# Visual Layout

\[
g(x)h(x)
\]

becomes

\[
g'(x)h(x)
+
g(x)h'(x)
\]

---

# Example 1

\[
f(x)=x\sin x
\]

---

First:

\[
g(x)=x
\]

\[
g'(x)=1
\]

---

Second:

\[
h(x)=\sin x
\]

\[
h'(x)=\cos x
\]

---

Apply Product Rule:

\[
f'(x)
=
(1)(\sin x)
+
(x)(\cos x)
\]

---

Answer:

\[
\boxed{
\sin x+x\cos x
}
\]

---

# Example 2

\[
f(x)=x^2\cos x
\]

---

Derivative:

\[
(2x)(\cos x)
+
(x^2)(-\sin x)
\]

---

Answer:

\[
\boxed{
2x\cos x-x^2\sin x
}
\]

---

# Easy Memory Rule

**First derivative × second + first × second derivative**

---

# 3. Systematic Extraction of Components

---

# The Best Method

Whenever you see a product:

\[
g(x)h(x)
\]

follow these four steps.

---

## Step 1

Identify:

\[
g(x)
\]

---

## Step 2

Identify:

\[
h(x)
\]

---

## Step 3

Differentiate each:

\[
g'(x)
\]

\[
h'(x)
\]

---

## Step 4

Substitute into:

\[
g'(x)h(x)+g(x)h'(x)
\]

---

# Example

\[
f(x)=x^3e^x
\]

---

Identify:

\[
g(x)=x^3
\]

\[
h(x)=e^x
\]

---

Differentiate:

\[
g'(x)=3x^2
\]

\[
h'(x)=e^x
\]

---

Substitute:

\[
(3x^2)(e^x)
+
(x^3)(e^x)
\]

---

Answer:

\[
3x^2e^x+x^3e^x
\]

---

# Why This Method Works

It prevents mistakes.

Students usually make errors when trying to do everything mentally.

---

# Real-Life Analogy

Before assembling furniture:

- Identify pieces
- Organize pieces
- Follow instructions

The Product Rule works the same way.

---

# Easy Memory Rule

**Label first, differentiate second, then substitute.**

---

# 4. Trigonometric Application Example

---

Consider:

\[
f(x)=\sin x\cos x
\]

---

# Step 1

Let:

\[
g(x)=\sin x
\]

\[
h(x)=\cos x
\]

---

# Step 2

Differentiate:

\[
g'(x)=\cos x
\]

\[
h'(x)=-\sin x
\]

---

# Step 3

Apply Product Rule

\[
f'(x)
=
(\cos x)(\cos x)
+
(\sin x)(-\sin x)
\]

---

# Step 4

Simplify

\[
=
\cos^2x
-
\sin^2x
\]

---

Answer:

\[
\boxed{
\cos^2x-\sin^2x
}
\]

---

# Numerical Example

At:

\[
x=0
\]

---

Derivative:

\[
\cos^20-\sin^20
\]

---

\[
=1-0
\]

---

\[
=1
\]

---

# Why Is This Important?

This expression appears frequently in:

- Trigonometry
- Physics
- Signal processing

---

# Real-Life Example

Sound waves often involve products of sine and cosine functions.

The Product Rule helps calculate how these waves change.

---

# Easy Memory Rule

**Differentiate sine to cosine and cosine to negative sine.**

---

# 5. Exponential Application Example

---

Consider:

\[
f(x)=x^5e^x
\]

---

This is a combination of:

- Polynomial
- Exponential

---

# Step 1

Identify:

\[
g(x)=x^5
\]

\[
h(x)=e^x
\]

---

# Step 2

Differentiate

\[
g'(x)=5x^4
\]

\[
h'(x)=e^x
\]

---

# Step 3

Apply Product Rule

\[
f'(x)
=
(5x^4)(e^x)
+
(x^5)(e^x)
\]

---

Answer:

\[
\boxed{
5x^4e^x+x^5e^x
}
\]

---

Notice:

\[
e^x
\]

remains unchanged because:

\[
\frac{d}{dx}(e^x)=e^x
\]

---

# Another Example

\[
f(x)=xe^x
\]

---

Derivative:

\[
(1)(e^x)
+
(x)(e^x)
\]

---

Answer:

\[
\boxed{
e^x+xe^x
}
\]

---

# Real-Life Example

Population models often contain:

\[
xe^x
\]

or

\[
x^2e^x
\]

The Product Rule allows scientists to calculate growth rates.

---

# Easy Memory Rule

**\(e^x\) keeps reappearing because its derivative equals itself.**

---

# 6. Algorithmic Factoring and Cleanup

---

# Why Simplify?

After applying the Product Rule, answers often contain common factors.

Factoring makes the result:

- Shorter
- Cleaner
- Easier to read

---

# Example 1

We obtained:

\[
5x^4e^x+x^5e^x
\]

---

Notice common factor:

\[
x^4e^x
\]

---

Factor it out:

\[
x^4e^x(5+x)
\]

---

Rearrange:

\[
\boxed{
x^4e^x(x+5)
}
\]

---

# Example 2

\[
3x^2e^x+x^3e^x
\]

---

Factor:

\[
x^2e^x
\]

---

Answer:

\[
\boxed{
x^2e^x(x+3)
}
\]

---

# Example 3

\[
2x\sin x+x^2\cos x
\]

---

Factor:

\[
x
\]

---

Answer:

\[
\boxed{
x(2\sin x+x\cos x)
}
\]

---

# Why Mathematicians Simplify

Simplified expressions:

- Reveal patterns
- Make future differentiation easier
- Reduce algebra mistakes

---

# Real-Life Analogy

Think of code optimization.

Before:

```python
x*x*x*x*e + x*x*x*x*5*e
```

After factoring:

```python
x4e*(x+5)
```

Same result.

Much cleaner.

---

# Easy Memory Rule

**Always look for common factors before writing the final answer.**

---

# Complete Summary

---

## Product Rule Formula

If:

\[
f(x)=g(x)h(x)
\]

then:

\[
\boxed{
f'(x)=g'(x)h(x)+g(x)h'(x)
}
\]

---

## Working Method

1. Identify \(g(x)\)
2. Identify \(h(x)\)
3. Find \(g'(x)\)
4. Find \(h'(x)\)
5. Substitute into Product Rule

---

## Trigonometric Example

\[
f(x)=\sin x\cos x
\]

Derivative:

\[
\boxed{
\cos^2x-\sin^2x
}
\]

---

## Exponential Example

\[
f(x)=x^5e^x
\]

Derivative:

\[
5x^4e^x+x^5e^x
\]

Factored:

\[
\boxed{
x^4e^x(x+5)
}
\]

---

## Final Simplification Rule

After differentiating:

- Search for common factors.
- Factor them out.
- Write the cleanest possible expression.

---

### One-Sentence Memory Rule

**For a product of two functions, differentiate the first and keep the second, then add the first kept unchanged times the derivative of the second, and finally simplify by factoring out any common terms.**