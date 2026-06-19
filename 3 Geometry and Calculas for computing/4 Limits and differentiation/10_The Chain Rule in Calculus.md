# The Chain Rule in Calculus — Complete Notes with Examples

---

# Introduction

So far, we have learned:

- Power Rule
- Product Rule
- Quotient Rule
- Exponential Derivatives
- Logarithmic Derivatives
- Trigonometric Derivatives

However, many functions are actually **functions inside other functions**.

Examples:

\[
e^{4x}
\]

\[
e^{3x^2}
\]

\[
\sin(x^2)
\]

\[
(5x+1)^7
\]

\[
\ln(x^2+1)
\]

These are called **composite functions**.

To differentiate them, we use one of the most important rules in all of calculus:

\[
\boxed{\text{The Chain Rule}}
\]

---

# 1. Introduction to the Chain Rule

---

## What Is a Composite Function?

A composite function is a function inside another function.

---

# Example 1

\[
e^{4x}
\]

The exponent:

\[
4x
\]

is itself a function.

Therefore:

\[
e^{4x}
\]

is a function inside another function.

---

# Example 2

\[
\sin(x^2)
\]

The inside function:

\[
x^2
\]

feeds into the outside function:

\[
\sin(\ )
\]

---

# Example 3

\[
\ln(x^2+1)
\]

Inside:

\[
x^2+1
\]

Outside:

\[
\ln(\ )
\]

---

# Why Can't We Use Ordinary Rules?

Consider:

\[
e^{4x}
\]

If we incorrectly use:

\[
\frac{d}{dx}(e^x)=e^x
\]

we would get:

\[
e^{4x}
\]

which is incomplete.

We ignored the effect of:

\[
4x
\]

inside the exponent.

---

The Chain Rule accounts for both:

- The outside function
- The inside function

---

# Real-Life Analogy

Imagine a factory.

Raw material enters:

Machine A

↓

Machine B

↓

Final product

---

If Machine A changes, the final output changes.

If Machine B changes, the final output changes.

Both layers matter.

The Chain Rule tracks both layers.

---

# Easy Memory Rule

**A Chain Rule problem contains a function inside another function.**

---

# 2. Algebraic Definition of the Chain Rule

---

Suppose:

\[
f(x)=g(h(x))
\]

---

where:

- \(h(x)\) = inner function
- \(g(x)\) = outer function

---

The Chain Rule says:

\[
\boxed{
f'(x)
=
g'(h(x))
\cdot
h'(x)
}
\]

---

# In Words

1. Differentiate the outside function.
2. Leave the inside unchanged.
3. Multiply by the derivative of the inside.

---

# Memory Phrase

Many students memorize:

> Differentiate the outside, keep the inside, multiply by the derivative of the inside.

---

# Visual Diagram

Original:

\[
g(h(x))
\]

---

Derivative:

\[
g'(h(x))
\cdot
h'(x)
\]

---

# Simple Example

\[
(x^2+1)^5
\]

---

Outer function:

\[
u^5
\]

Derivative:

\[
5u^4
\]

---

Keep inside:

\[
5(x^2+1)^4
\]

---

Multiply by derivative of inside:

\[
2x
\]

---

Answer:

\[
\boxed{
10x(x^2+1)^4
}
\]

---

# Easy Memory Rule

**Outside derivative × Inside derivative**

---

# 3. Simple Exponential Example (\(e^{4x}\))

---

Consider:

\[
f(x)=e^{4x}
\]

---

# Step 1: Identify Functions

Inner function:

\[
h(x)=4x
\]

---

Outer function:

\[
g(x)=e^x
\]

---

# Step 2: Differentiate Inner Function

\[
h'(x)=4
\]

---

# Step 3: Differentiate Outer Function

Derivative of:

\[
e^x
\]

is:

\[
e^x
\]

---

Keep the inside unchanged:

\[
e^{4x}
\]

---

# Step 4: Apply Chain Rule

\[
f'(x)
=
e^{4x}
\cdot4
\]

---

Answer:

\[
\boxed{
4e^{4x}
}
\]

---

# Another Example

\[
e^{7x}
\]

---

Inner:

\[
7x
\]

Derivative:

\[
7
\]

---

Answer:

\[
\boxed{
7e^{7x}
}
\]

---

# Another Example

\[
e^{-3x}
\]

---

Inner derivative:

\[
-3
\]

---

Answer:

\[
\boxed{
-3e^{-3x}
}
\]

---

# Real-Life Example

Suppose:

\[
P(t)=e^{4t}
\]

represents population growth.

The derivative:

\[
4e^{4t}
\]

measures the population growth rate.

---

# Easy Memory Rule

**Differentiate the exponent and multiply by \(e^{\text{same exponent}}\).**

---

# 4. Complex Polynomial-Exponential Example (\(e^{3x^2}\))

---

Consider:

\[
f(x)=e^{3x^2}
\]

---

This contains:

An exponential function

and

a polynomial inside it.

---

# Step 1: Identify Functions

Inner:

\[
h(x)=3x^2
\]

---

Outer:

\[
g(x)=e^x
\]

---

# Step 2: Differentiate Inner Function

\[
h'(x)=6x
\]

---

# Step 3: Differentiate Outer Function

Derivative of:

\[
e^x
\]

is:

\[
e^x
\]

---

Keep inside unchanged:

\[
e^{3x^2}
\]

---

# Step 4: Apply Chain Rule

\[
f'(x)
=
e^{3x^2}
\cdot6x
\]

---

Answer:

\[
\boxed{
6xe^{3x^2}
}
\]

---

# Another Example

\[
e^{5x^3}
\]

---

Inner:

\[
5x^3
\]

Derivative:

\[
15x^2
\]

---

Answer:

\[
\boxed{
15x^2e^{5x^3}
}
\]

---

# Another Example

\[
e^{x^4}
\]

---

Inner derivative:

\[
4x^3
\]

---

Answer:

\[
\boxed{
4x^3e^{x^4}
}
\]

---

# Why Is the Chain Rule Necessary?

Without the Chain Rule:

\[
e^{3x^2}
\]

would incorrectly differentiate to:

\[
e^{3x^2}
\]

---

We would completely miss:

\[
6x
\]

---

# Real-Life Analogy

Think of two gears.

The outer gear rotates.

The inner gear also rotates.

Total motion depends on both gears.

---

# Easy Memory Rule

**Differentiate the exponent, then multiply by the original exponential.**

---

# 5. The Value of Rigorous Notation for Error Checking

---

Many calculus mistakes happen because students skip steps.

---

# Poor Method

Immediately writing:

\[
e^{3x^2}
\rightarrow6xe^{3x^2}
\]

---

Although correct,

mistakes become difficult to detect.

---

# Better Method

Write everything clearly.

---

Example:

\[
f(x)=e^{3x^2}
\]

---

Inner:

\[
h(x)=3x^2
\]

\[
h'(x)=6x
\]

---

Outer:

\[
g(x)=e^x
\]

\[
g'(x)=e^x
\]

---

Apply Chain Rule:

\[
f'(x)
=
g'(h(x))
\cdot
h'(x)
\]

---

Substitute:

\[
=
e^{3x^2}
\cdot6x
\]

---

Answer:

\[
6xe^{3x^2}
\]

---

# Why Is This Helpful?

If an answer looks wrong,

you can inspect:

- Inner function
- Outer function
- Inner derivative
- Outer derivative

and immediately find the mistake.

---

# Example of a Common Error

Differentiate:

\[
e^{5x^2}
\]

---

Wrong answer:

\[
10x
\]

---

What's missing?

The outer derivative:

\[
e^{5x^2}
\]

---

Correct answer:

\[
\boxed{
10xe^{5x^2}
}
\]

---

# Real-Life Analogy

Programmers debug code by showing intermediate variables.

Mathematicians do the same thing.

Clear notation acts like debugging output.

---

# Easy Memory Rule

**Writing every component separately makes mistakes easy to spot.**

---

# More Chain Rule Examples

---

## Example 1

\[
\sin(x^2)
\]

---

Outer:

\[
\sin u
\]

Derivative:

\[
\cos u
\]

---

Inner:

\[
x^2
\]

Derivative:

\[
2x
\]

---

Answer:

\[
\boxed{
2x\cos(x^2)
}
\]

---

## Example 2

\[
\cos(3x)
\]

---

Outer derivative:

\[
-\sin(3x)
\]

---

Inner derivative:

\[
3
\]

---

Answer:

\[
\boxed{
-3\sin(3x)
}
\]

---

## Example 3

\[
\ln(x^2+1)
\]

---

Outer derivative:

\[
\frac1{x^2+1}
\]

---

Inner derivative:

\[
2x
\]

---

Answer:

\[
\boxed{
\frac{2x}{x^2+1}
}
\]

---

# Complete Summary

---

## When to Use the Chain Rule

Use it whenever a function contains another function inside it.

Examples:

\[
e^{4x}
\]

\[
\sin(x^2)
\]

\[
(x^2+1)^5
\]

\[
\ln(x^2+1)
\]

---

## Chain Rule Formula

\[
\boxed{
f'(x)
=
g'(h(x))
\cdot
h'(x)
}
\]

---

## Working Method

1. Identify inner function.
2. Identify outer function.
3. Differentiate outer function.
4. Keep inside unchanged.
5. Multiply by derivative of inside.

---

## Example

\[
e^{4x}
\]

Derivative:

\[
\boxed{
4e^{4x}
}
\]

---

## Example

\[
e^{3x^2}
\]

Derivative:

\[
\boxed{
6xe^{3x^2}
}
\]

---

## Why Write Everything Clearly?

Clear notation:

- Prevents mistakes.
- Helps debugging.
- Makes exams easier.
- Shows all reasoning steps.

---

### One-Sentence Memory Rule

**The Chain Rule says to differentiate the outside function while leaving the inside unchanged, then multiply by the derivative of the inside function, making it the essential tool for differentiating any function-of-a-function expression.**