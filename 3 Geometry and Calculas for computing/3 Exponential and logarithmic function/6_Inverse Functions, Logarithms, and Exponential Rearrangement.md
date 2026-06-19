# Inverse Functions, Logarithms, and Exponential Rearrangement

---

# Introduction

One of the most important uses of logarithms is finding inverse functions and solving equations where variables are trapped inside exponents or logarithms.

The key idea is:

> Exponentials and logarithms are opposites (inverse operations).

Just as:

- Addition is undone by subtraction
- Multiplication is undone by division

Similarly:

- Exponentials are undone by logarithms
- Logarithms are undone by exponentials

---

# 1. Goal of Finding an Inverse

## What Is an Inverse Function?

An inverse function reverses what the original function does.

If a function sends:

\[
x \rightarrow y
\]

the inverse sends:

\[
y \rightarrow x
\]

---

# The Standard Strategy

Whenever you find an inverse function, follow these steps:

### Step 1

Replace:

\[
f(x)
\]

with:

\[
y
\]

---

### Step 2

Interchange x and y

Replace:

\[
x \leftrightarrow y
\]

---

### Step 3

Solve for y

Make y the subject of the formula.

---

### Step 4

Rename y as:

\[
f^{-1}(x)
\]

---

# Example 1

Find the inverse of:

\[
f(x)=x+5
\]

---

## Step 1

Replace with y:

\[
y=x+5
\]

---

## Step 2

Swap x and y:

\[
x=y+5
\]

---

## Step 3

Solve for y:

\[
y=x-5
\]

---

## Step 4

Write inverse:

\[
f^{-1}(x)=x-5
\]

---

# Check

Original:

\[
3 \rightarrow 8
\]

Inverse:

\[
8 \rightarrow 3
\]

Works perfectly.

---

# Example 2

Find inverse of:

\[
f(x)=2x+1
\]

---

Swap:

\[
x=2y+1
\]

---

Solve:

\[
x-1=2y
\]

\[
y=\frac{x-1}{2}
\]

---

Inverse:

\[
f^{-1}(x)=\frac{x-1}{2}
\]

---

# Real-Life Analogy

Imagine a vending machine.

Original function:

- Insert ₹10
- Machine adds ₹5 bonus

Result:

₹15

Inverse function:

- Remove ₹5 bonus

Result:

₹10

---

# Easy Memory Rule

Finding an inverse means:

**Swap x and y, then solve for y.**

---

# 2. Using Logarithms to Isolate Exponential Exponents

---

# The Problem

Sometimes a variable is trapped inside an exponent.

Example:

\[
y=3^{2x+1}
\]

---

We cannot use normal algebra because:

\[
2x+1
\]

is inside the exponent.

---

# The Solution

Apply the logarithm with the matching base.

Since the base is:

\[
3
\]

apply:

\[
\log_3
\]

to both sides.

---

# Example 1

\[
y=3^{2x+1}
\]

---

Apply \(\log_3\):

\[
\log_3(y)
=
\log_3(3^{2x+1})
\]

---

Use cancellation:

\[
\log_3(3^k)=k
\]

Therefore:

\[
\log_3(y)=2x+1
\]

---

Now solve normally:

\[
\log_3(y)-1=2x
\]

\[
x=\frac{\log_3(y)-1}{2}
\]

---

# Example 2

\[
y=2^{x+4}
\]

Apply:

\[
\log_2
\]

to both sides.

---

\[
\log_2(y)=x+4
\]

---

Solve:

\[
x=\log_2(y)-4
\]

---

# Example 3

\[
y=5^{3x}
\]

Apply:

\[
\log_5
\]

---

\[
\log_5(y)=3x
\]

---

\[
x=\frac{\log_5(y)}{3}
\]

---

# Real-Life Analogy

Imagine a person trapped inside a locked room.

Normal algebra cannot reach them.

The logarithm acts like the correct key.

Only the matching logarithm can unlock the exponent.

---

# Easy Memory Rule

Variable in exponent?

Use a logarithm.

---

# 3. Canceling Logs Using Exponential Bases

---

# The Reverse Situation

Now the variable is trapped inside a logarithm.

Example:

\[
y=\log_2(x-1)
\]

---

To remove the logarithm:

Raise the matching base to both sides.

Since the log base is 2:

Use:

\[
2^{}
\]

on both sides.

---

# Example 1

\[
y=\log_2(x-1)
\]

---

Raise 2 to both sides:

\[
2^y
=
2^{\log_2(x-1)}
\]

---

Apply cancellation:

\[
2^{\log_2(x-1)}
=
x-1
\]

---

Therefore:

\[
2^y=x-1
\]

---

\[
x=2^y+1
\]

---

# Example 2

\[
y=\log_3(x+4)
\]

---

Raise 3 to both sides:

\[
3^y=x+4
\]

---

\[
x=3^y-4
\]

---

# Example 3

\[
y=\log_5(2x)
\]

---

Raise 5 to both sides:

\[
5^y=2x
\]

---

\[
x=\frac{5^y}{2}
\]

---

# Real-Life Analogy

A logarithm is like a wrapper around a gift.

Using the matching exponential removes the wrapper.

The gift inside becomes visible.

---

# Easy Memory Rule

Variable inside log?

Use the matching exponential.

---

# 4. Applying Laws of Indices in Rearrangement

---

# Important Exponent Rule

Remember:

\[
a^{m+n}
=
a^m \times a^n
\]

---

This rule is extremely useful when finding inverses.

---

# Example 1

Consider:

\[
2^{\log_2(x-1)+3}
\]

---

Split the exponent:

\[
=
2^{\log_2(x-1)}
\times
2^3
\]

---

Apply cancellation:

\[
=
(x-1)\times8
\]

---

Answer:

\[
8(x-1)
\]

---

# Example 2

\[
3^{\log_3(x)+2}
\]

---

Split:

\[
=
3^{\log_3(x)}
\times
3^2
\]

---

\[
=x\times9
\]

---

\[
=9x
\]

---

# Example 3

\[
5^{\log_5(y)+1}
\]

---

Split:

\[
=
5^{\log_5(y)}
\times
5^1
\]

---

\[
=5y
\]

---

# Why Is This Useful?

It transforms complicated exponentials into simple multiplication.

---

# Real-Life Analogy

Think of:

\[
2^{a+b}
\]

like two separate machines working together.

Machine A:

\[
2^a
\]

Machine B:

\[
2^b
\]

The final result is:

\[
2^a \times 2^b
\]

---

# Easy Memory Rule

Addition in exponent

becomes

Multiplication outside.

---

# 5. The Cancellation Property in Action

---

# The Most Important Rule

\[
a^{\log_a(x)}
=
x
\]

and

\[
\log_a(a^x)
=
x
\]

---

These identities power almost every logarithm problem.

---

# Example 1

\[
2^{\log_2(7)}
\]

---

Cancellation:

\[
=7
\]

---

# Example 2

\[
3^{\log_3(50)}
\]

---

Cancellation:

\[
=50
\]

---

# Example 3

\[
\log_5(5^8)
\]

---

Cancellation:

\[
=8
\]

---

# Example 4

\[
10^{\log_{10}(1000)}
\]

---

Cancellation:

\[
=1000
\]

---

# Step-by-Step Example

Simplify:

\[
2^{\log_2(x-1)+3}
\]

---

## Step 1

Split exponent

\[
=
2^{\log_2(x-1)}
\times
2^3
\]

---

## Step 2

Cancel

\[
=
(x-1)\times8
\]

---

## Step 3

Simplify

\[
=8x-8
\]

---

# Why Does Cancellation Work?

Because logarithms and exponentials are inverse operations.

Just like:

\[
(+5) \quad \text{and} \quad (-5)
\]

cancel each other.

Similarly:

\[
\log_a
\]

and

\[
a^x
\]

cancel each other.

---

# Real-Life Analogy

Think of a zip file.

### Compress

File → ZIP

### Decompress

ZIP → File

Nothing changes.

You get the original file back.

Logarithms and exponentials behave exactly the same way.

---

# Complete Summary

---

## Finding an Inverse

1. Replace \(f(x)\) with \(y\)
2. Swap \(x\) and \(y\)
3. Solve for \(y\)

---

## Variable in Exponent

Example:

\[
y=3^{2x+1}
\]

Use:

\[
\log_3
\]

to isolate the exponent.

---

## Variable Inside Logarithm

Example:

\[
y=\log_2(x-1)
\]

Use:

\[
2^{}
\]

to remove the logarithm.

---

## Exponent Rule

\[
a^{m+n}
=
a^m a^n
\]

Addition in exponent becomes multiplication.

---

## Cancellation Rules

\[
a^{\log_a(x)}
=
x
\]

\[
\log_a(a^x)
=
x
\]

---

## Key Idea

Every logarithm problem is fundamentally about recognizing and using the fact that logarithms and exponentials are inverse operations that perfectly undo one another.

---

### One-Sentence Memory Rule

**If the variable is trapped inside an exponent, use a logarithm; if the variable is trapped inside a logarithm, use the matching exponential, because exponentials and logarithms always cancel each other when their bases match.**