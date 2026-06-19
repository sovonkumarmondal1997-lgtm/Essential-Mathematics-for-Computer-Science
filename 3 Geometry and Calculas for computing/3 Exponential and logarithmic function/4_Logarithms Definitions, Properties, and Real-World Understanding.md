# Logarithms — Definitions, Properties, and Real-World Understanding

---

# 1. Structure of the Logarithm Lecture

## What Is the Overall Goal of the Lecture?

The purpose of the logarithm lecture is to teach:

1. What logarithms are.
2. How logarithms relate to exponentials.
3. How logarithmic graphs behave.
4. How logarithms help solve difficult equations.

The lecture is typically divided into three major sections.

---

# Part 1: Algebraic Definitions

This section answers:

> "What exactly is a logarithm?"

Topics include:

- Inverse functions
- Exponential functions
- Definition of logarithms
- Basic logarithm laws

---

## Example

Question:

\[
2^x = 8
\]

We can solve mentally:

\[
x = 3
\]

because:

\[
2^3 = 8
\]

A logarithm provides a systematic way to find such exponents.

---

# Part 2: Graph Plotting

This section studies:

\[
y=\log_a x
\]

Graph behavior:

- Shape
- Intercepts
- Symmetry with exponential functions
- Domain and range

---

## Example

Graph:

\[
y=\log_2 x
\]

contains points:

\[
(1,0)
\]

\[
(2,1)
\]

\[
(4,2)
\]

\[
(8,3)
\]

---

# Part 3: Solving Equations

This section uses logarithms as algebraic tools.

---

## Example

Solve:

\[
3^x=100
\]

This cannot be solved easily by inspection.

Using logarithms:

\[
x=\log_3(100)
\]

---

# Why This Matters

Applications include:

- Finance
- Data Science
- Engineering
- Population modeling
- Radioactive decay
- Machine learning

---

# 2. Definition of an Inverse Function

---

## What Is a Function?

A function maps an input to an output.

Example:

\[
f(x)=x+5
\]

Input:

\[
3
\]

Output:

\[
8
\]

because:

\[
3+5=8
\]

---

# What Is an Inverse Function?

An inverse function reverses the process.

If:

\[
3 \rightarrow 8
\]

the inverse sends:

\[
8 \rightarrow 3
\]

---

## Everyday Example: Elevator

Imagine an elevator.

### Original Function

Go up 5 floors.

Floor 2 becomes Floor 7.

---

### Inverse Function

Go down 5 floors.

Floor 7 becomes Floor 2.

---

# Example

Original:

\[
f(x)=x+5
\]

Inverse:

\[
f^{-1}(x)=x-5
\]

Check:

\[
f(3)=8
\]

Then:

\[
f^{-1}(8)=3
\]

Perfect reversal.

---

# Why Must a Function Be One-to-One?

A function can only have an inverse if every output comes from exactly one input.

---

## Good Example

\[
f(x)=2x
\]

| x | y |
|---|---|
|1|2|
|2|4|
|3|6|

Every output is unique.

Inverse exists.

---

## Bad Example

\[
f(x)=x^2
\]

| x | y |
|---|---|
|-2|4|
|2|4|

Output 4 comes from two inputs.

Inverse becomes ambiguous.

---

# Easy Memory Trick

A function must never "merge roads" if you want to drive backward.

---

# 3. Logarithms Defined as Exponential Inverses

---

# The Exponential Function

Consider:

\[
y=2^x
\]

Examples:

\[
2^3=8
\]

\[
2^4=16
\]

---

# The Logarithm Function

A logarithm asks:

> "What exponent created this number?"

---

## Example

Question:

\[
2^?=8
\]

Answer:

\[
3
\]

Therefore:

\[
\log_2(8)=3
\]

---

# General Definition

\[
\log_a(x)=y
\]

means:

\[
a^y=x
\]

---

# Example 1

\[
\log_2(32)
\]

means:

\[
2^?=32
\]

Answer:

\[
5
\]

because:

\[
2^5=32
\]

Therefore:

\[
\log_2(32)=5
\]

---

# Example 2

\[
\log_{10}(1000)
\]

means:

\[
10^?=1000
\]

Answer:

\[
3
\]

---

# Easy Memory Trick

Exponentials create numbers.

Logarithms discover the exponent.

---

# 4. The Principle of Cancellation

---

## What Is Cancellation?

Exponential and logarithmic functions undo each other.

Just like:

- Lock and key
- Forward and reverse
- Multiply and divide

---

# Rule 1

\[
a^{\log_a x}=x
\]

---

## Example

\[
2^{\log_2(16)}
\]

Since:

\[
\log_2(16)=4
\]

Then:

\[
2^4=16
\]

---

# Rule 2

\[
\log_a(a^x)=x
\]

---

## Example

\[
\log_2(2^5)
\]

Answer:

\[
5
\]

---

# Real-Life Analogy

Imagine:

1. Compress a file.
2. Immediately unzip it.

You get the original file back.

Logarithms and exponentials behave similarly.

---

# 5. Universal Intercepts for Logarithmic Graphs

---

# Point 1: \((1,0)\)

Because:

\[
\log_a(1)=0
\]

since:

\[
a^0=1
\]

---

## Examples

\[
\log_2(1)=0
\]

\[
\log_3(1)=0
\]

\[
\log_{10}(1)=0
\]

---

Therefore every logarithmic graph passes through:

\[
(1,0)
\]

---

# Point 2: \((a,1)\)

Because:

\[
\log_a(a)=1
\]

since:

\[
a^1=a
\]

---

## Examples

### Base 2

\[
\log_2(2)=1
\]

Point:

\[
(2,1)
\]

---

### Base 3

\[
\log_3(3)=1
\]

Point:

\[
(3,1)
\]

---

### Base 10

\[
\log_{10}(10)=1
\]

Point:

\[
(10,1)
\]

---

# Easy Memory Trick

Every logarithmic graph always passes through:

\[
(1,0)
\]

and

\[
(a,1)
\]

---

# 6. The Power Rule of Logarithms

---

# Rule

\[
\log_b(m^k)
=
k\log_b(m)
\]

---

## Meaning

An exponent inside the logarithm can move outside.

---

# Example 1

\[
\log_2(8^3)
\]

Move exponent:

\[
=3\log_2(8)
\]

\[
=3\times3
\]

\[
=9
\]

---

# Example 2

\[
\log_{10}(100^2)
\]

\[
=2\log_{10}(100)
\]

\[
=2\times2
\]

\[
=4
\]

---

# Easy Memory Trick

Exponent inside → multiplier outside.

---

# 7. The Product Rule of Logarithms

---

# Rule

\[
\log_b(mn)
=
\log_b(m)
+
\log_b(n)
\]

---

# Meaning

Multiplication becomes addition.

---

## Example 1

\[
\log_2(8\times4)
\]

\[
=
\log_2(8)
+
\log_2(4)
\]

\[
=
3+2
\]

\[
=5
\]

---

Check:

\[
8\times4=32
\]

\[
\log_2(32)=5
\]

Correct.

---

## Example 2

\[
\log_{10}(100\times1000)
\]

\[
=
2+3
\]

\[
=5
\]

---

# Why Is This Useful?

It converts difficult multiplication into simple addition.

---

# 8. Historical Use of the Product Rule (Slide Rules)

---

## Before Calculators

People had no calculators.

Engineers used:

- Logarithm tables
- Slide rules

to perform calculations.

---

# Example

Suppose you want:

\[
250\times400
\]

Instead of multiplying directly:

1. Find logarithms.
2. Add them.
3. Convert back.

---

Using logs:

\[
\log(250)
+
\log(400)
\]

Then reverse the logarithm.

Result:

\[
100000
\]

---

# Real-Life Analogy

Today:

Calculator → multiplication

Old days:

Logarithms → addition → answer

This made huge calculations possible.

---

# 9. The Quotient Rule of Logarithms

---

# Rule

\[
\log_b\left(\frac{m}{n}\right)
=
\log_b(m)
-
\log_b(n)
\]

---

# Meaning

Division becomes subtraction.

---

# Example 1

\[
\log_2\left(\frac{32}{4}\right)
\]

\[
=
\log_2(32)
-
\log_2(4)
\]

\[
=
5-2
\]

\[
=3
\]

---

Check:

\[
\frac{32}{4}=8
\]

\[
\log_2(8)=3
\]

Correct.

---

# Example 2

\[
\log_{10}\left(\frac{1000}{10}\right)
\]

\[
=
3-1
\]

\[
=2
\]

---

# Easy Memory Trick

Division inside log

becomes

Subtraction outside log.

---

# 10. Algebraic Proof of the Product Rule

---

We want to prove:

\[
\log_a(xy)
=
\log_a(x)
+
\log_a(y)
\]

---

# Step 1

Use exponential definitions:

\[
x=a^{\log_a(x)}
\]

\[
y=a^{\log_a(y)}
\]

---

# Step 2

Multiply

\[
xy
=
a^{\log_a(x)}
\cdot
a^{\log_a(y)}
\]

---

# Step 3

Apply exponent rule

\[
a^m a^n
=
a^{m+n}
\]

Therefore:

\[
xy
=
a^{\log_a(x)+\log_a(y)}
\]

---

# Step 4

Take logarithm of both sides

\[
\log_a(xy)
=
\log_a
\left(
a^{\log_a(x)+\log_a(y)}
\right)
\]

---

# Step 5

Apply cancellation

\[
\log_a(a^k)
=
k
\]

Therefore:

\[
\log_a(xy)
=
\log_a(x)
+
\log_a(y)
\]

---

# Proven

\[
\boxed{
\log_a(xy)
=
\log_a(x)
+
\log_a(y)
}
\]

---

# Final Summary

## Logarithms Are Inverses of Exponentials

\[
\log_a(x)=y
\]

means

\[
a^y=x
\]

---

## Cancellation Rules

\[
a^{\log_a x}=x
\]

\[
\log_a(a^x)=x
\]

---

## Universal Graph Points

\[
(1,0)
\]

and

\[
(a,1)
\]

---

## Power Rule

\[
\log_b(m^k)
=
k\log_b(m)
\]

---

## Product Rule

\[
\log_b(mn)
=
\log_b(m)
+
\log_b(n)
\]

Multiplication becomes addition.

---

## Quotient Rule

\[
\log_b\left(\frac{m}{n}\right)
=
\log_b(m)
-
\log_b(n)
\]

Division becomes subtraction.

---

## Historical Importance

Logarithms allowed engineers and scientists to replace difficult multiplication and division with simple addition and subtraction long before electronic calculators existed.

---

### One-Sentence Memory Rule

**A logarithm is simply the inverse of an exponential, and its rules transform multiplication into addition, division into subtraction, and powers into multiplication, making complex calculations much easier to perform.**