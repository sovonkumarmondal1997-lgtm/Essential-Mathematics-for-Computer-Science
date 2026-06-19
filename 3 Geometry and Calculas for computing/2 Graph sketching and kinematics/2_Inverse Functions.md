# Inverse Functions: Injectivity, Notation, Algebraic Method, and Geometric Interpretation

---

# 1. Visualizing Injectivity for an Inverse Function

## Why Do We Need Injectivity?

Before a function can have an inverse, it must be **injective (one-to-one)**.

This means:

```text
Different inputs must produce different outputs.
```

---

# The "Converging Lines" Test

Imagine a mapping diagram.

### Injective Function

```text
Domain          Range

1 ------------> A
2 ------------> B
3 ------------> C
```

Notice:

```text
No arrows meet.
```

No lines converge.

This is injective.

---

## Why Is This Good?

If we reverse the arrows:

```text
A ------------> 1
B ------------> 2
C ------------> 3
```

Each input still has exactly one output.

Therefore:

```text
The inverse is also a function.
```

---

# The Inversion Failure

Now consider:

```text
Domain          Range

1 ------------> A
2 ------------> A
3 ------------> B
```

Notice:

```text
Two arrows converge into A.
```

This is **many-to-one**.

---

# What Happens If We Reverse It?

Reverse the arrows:

```text
Range           Domain

A ------------> 1
A ------------> 2
B ------------> 3
```

Now:

```text
A
```

has two outputs.

---

# Problem

A function must satisfy:

```text
One input → One output
```

But here:

```text
A → 1
A → 2
```

One input gives two outputs.

Therefore:

```text
Not a function.
```

---

# Key Idea

### Forward Direction

Converging lines are allowed in a normal function.

```text
1 → A
2 → A
```

---

### Reverse Direction

The same converging lines become diverging lines.

```text
A → 1
A → 2
```

which breaks the function rule.

---

# Real-Life Example

Suppose:

```text
Rahul → 80 marks
Priya → 80 marks
```

Two students have the same score.

---

If we reverse:

```text
80 marks → Rahul
80 marks → Priya
```

we cannot determine uniquely which student corresponds to 80.

Therefore no inverse function exists.

---

# Rule for Inverse Functions

```text
Injective Function
      ↓
Valid Inverse
```

```text
Not Injective
      ↓
No Valid Inverse
```

---

# 2. Standard Function Notation

## What is Function Notation?

Function notation provides a way to describe:

```text
Input → Output
```

relationships.

---

# Mapping Arrow Notation

Example:

\[
f:x \rightarrow 3x-2
\]

Read as:

```text
Function f maps x to 3x−2.
```

---

# Example

Input:

```text
x = 4
```

Apply rule:

```text
3(4)-2
```

```text
12-2
```

```text
10
```

Output:

```text
10
```

---

# Standard Algebraic Notation

The same function can be written as:

\[
f(x)=3x-2
\]

Read as:

```text
f of x equals 3x−2
```

---

# Example

\[
f(4)=3(4)-2
\]

\[
=10
\]

---

# Another Example

\[
f(x)=x^2
\]

Then:

\[
f(5)=25
\]

---

# Why Use Function Notation?

It clearly separates:

```text
Input
```

from

```text
Rule
```

and

```text
Output
```

---

# Real-Life Example

Temperature Conversion:

\[
f(C)=\frac{9}{5}C+32
\]

Input:

```text
25°C
```

Output:

```text
77°F
```

---

# 3. Algorithm to Algebraically Calculate an Inverse Function

## Goal

Given:

\[
f(x)
\]

find:

\[
f^{-1}(x)
\]

---

# Step 1: Replace f(x) with y

Write:

\[
y=f(x)
\]

---

# Step 2: Solve for x

Use algebra until:

```text
x is alone.
```

---

# Step 3: Rewrite Using Inverse Notation

Replace:

```text
y → x
```

and write:

\[
f^{-1}(x)
\]

---

# Why Does This Work?

The inverse reverses the original operation.

Original:

```text
Input → Output
```

Inverse:

```text
Output → Input
```

---

# General Template

Start:

\[
y=f(x)
\]

Solve:

\[
x=...
\]

Rewrite:

\[
f^{-1}(x)=...
\]

---

# 4. Example 1 Walkthrough: Linear Function

## Given

\[
f(x)=3x-2
\]

Find:

\[
f^{-1}(x)
\]

---

# Step 1

Replace with y:

\[
y=3x-2
\]

---

# Step 2

Add 2:

\[
y+2=3x
\]

---

Divide by 3:

\[
x=\frac{y+2}{3}
\]

or

\[
x=\frac{1}{3}(y+2)
\]

---

# Step 3

Replace:

```text
y → x
```

Result:

\[
f^{-1}(x)
=
\frac{1}{3}(x+2)
\]

---

# Verification

Choose:

```text
x = 4
```

Original:

\[
f(4)
=
3(4)-2
=
10
\]

---

Apply inverse:

\[
f^{-1}(10)
=
\frac{10+2}{3}
=
4
\]

We return to the original value.

Perfect.

---

# Visual Interpretation

```text
4
↓
f(x)
↓
10
↓
f⁻¹(x)
↓
4
```

---

# 5. Example 2 Walkthrough: Rational/Fractional Function

## Given

\[
f(x)
=
\frac{1}{3}x-3
\]

Find:

\[
f^{-1}(x)
\]

---

# Step 1

Set:

\[
y
=
\frac{1}{3}x-3
\]

---

# Step 2

Add 3:

\[
y+3
=
\frac{1}{3}x
\]

---

Multiply by 3:

\[
x
=
3(y+3)
\]

---

# Step 3

Replace:

```text
y → x
```

Result:

\[
f^{-1}(x)
=
3(x+3)
\]

---

# Verification

Choose:

```text
x = 6
```

Original:

\[
f(6)
=
\frac{1}{3}(6)-3
\]

\[
=
2-3
\]

\[
=-1
\]

---

Apply inverse:

\[
f^{-1}(-1)
=
3(-1+3)
\]

\[
=
3(2)
\]

\[
=6
\]

We recover the original value.

Correct.

---

# Visual Interpretation

```text
6
↓
f(x)
↓
-1
↓
f⁻¹(x)
↓
6
```

---

# 6. Geometric Direction of Functions vs. Inverse Functions

## Forward Path

A function takes values from the domain and moves them to the range.

---

### Example

```text
Domain          Range

2 -----------> 4
3 -----------> 7
4 -----------> 10
```

using:

\[
f(x)=3x-2
\]

---

# Visualization

```text
Domain
  ↓
Function
  ↓
Range
```

---

# Return Path

The inverse reverses the journey.

---

### Example

```text
Range           Domain

4 -----------> 2
7 -----------> 3
10 ----------> 4
```

using:

\[
f^{-1}(x)
=
\frac{x+2}{3}
\]

---

# Visualization

```text
Domain
  ↓
f(x)
  ↓
Range
  ↓
f⁻¹(x)
  ↓
Domain
```

---

# Why Is It Called an "Undo"?

Suppose:

```text
Original operation:
×3 then −2
```

---

Inverse operation:

```text
+2 then ÷3
```

---

The inverse cancels the original action.

---

# Real-Life Example

Think of a password encryption system.

Original:

```text
Plain Text
    ↓
Encryption
    ↓
Cipher Text
```

---

Inverse:

```text
Cipher Text
    ↓
Decryption
    ↓
Plain Text
```

The inverse recovers the original information.

---

# Function and Inverse Together

For any valid inverse:

\[
f^{-1}(f(x))
=
x
\]

and

\[
f(f^{-1}(x))
=
x
\]

---

# Example

Given:

\[
f(x)=3x-2
\]

and

\[
f^{-1}(x)
=
\frac{x+2}{3}
\]

Compute:

\[
f^{-1}(f(5))
\]

---

First:

\[
f(5)
=
13
\]

Then:

\[
f^{-1}(13)
=
\frac{13+2}{3}
=
5
\]

Original value recovered.

---

# Summary Table

| Concept | Meaning |
|----------|----------|
| Injective Function | Different inputs → Different outputs |
| Converging Lines | Multiple inputs to same output |
| Diverging Lines | One input to multiple outputs |
| Inverse Function | Reverses a function |
| Mapping Notation | \(f:x\to3x-2\) |
| Standard Notation | \(f(x)=3x-2\) |
| Step 1 | Replace with y |
| Step 2 | Solve for x |
| Step 3 | Rewrite as \(f^{-1}(x)\) |
| Forward Path | Domain → Range |
| Return Path | Range → Domain |
| Inverse Property | \(f^{-1}(f(x))=x\) |

---

# Final Key Idea

An inverse function acts like a mathematical **undo button**.

```text
Function:
Input → Output
```

```text
Inverse:
Output → Input
```

For this to work correctly:

```text
Every output must come from only one input.
```

That is why a function must be **injective (one-to-one)** before a valid inverse can exist.

The standard process is:

```text
1. Write y = f(x)
2. Solve for x
3. Rewrite as f⁻¹(x)
```

This simple three-step method allows you to find the inverse of many algebraic functions and understand how functions and their inverses reverse each other's actions.
