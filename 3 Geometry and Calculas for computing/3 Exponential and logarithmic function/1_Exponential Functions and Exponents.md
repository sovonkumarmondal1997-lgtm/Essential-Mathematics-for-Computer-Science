# Exponential Functions and Exponents — Simple Notes with Real-Life Examples

---

# 1. Definition and Real-World Applications of Exponential Functions

## What is an Exponential Function?

An exponential function is a function where the variable appears in the exponent.

General form:

\[
y = a^x
\]

Where:

- \(a\) = base (positive number)
- \(x\) = exponent

Examples:

\[
y = 2^x
\]

\[
y = 3^x
\]

\[
y = 10^x
\]

\[
y = e^x
\]

---

## Why Are Exponential Functions Important?

They model situations where change becomes faster and faster (or slower and slower).

Unlike linear growth:

\[
y = x
\]

which increases by the same amount every time,

exponential growth multiplies by the same factor every time.

---

## Example 1: Population Growth

Suppose a town has 1000 people.

Population doubles every 10 years.

| Years | Population |
|---------|---------|
| 0 | 1000 |
| 10 | 2000 |
| 20 | 4000 |
| 30 | 8000 |
| 40 | 16000 |

Notice:

- Not adding
- Multiplying by 2

This is exponential growth.

Formula:

\[
P = 1000(2)^t
\]

---

## Example 2: Virus Spread

One infected person infects 2 others.

| Day | Infected |
|-------|-------|
| 1 | 1 |
| 2 | 2 |
| 3 | 4 |
| 4 | 8 |
| 5 | 16 |

Growth becomes very rapid.

---

## Example 3: Compound Interest

You invest ₹10,000.

Bank pays 10% interest annually.

| Year | Money |
|--------|--------|
| 0 | ₹10,000 |
| 1 | ₹11,000 |
| 2 | ₹12,100 |
| 3 | ₹13,310 |

Money grows exponentially.

Formula:

\[
A=P(1+r)^t
\]

---

## Example 4: Radioactive Decay

Some materials lose half their mass every period.

| Time | Mass |
|---------|---------|
| 0 | 100 g |
| 1 | 50 g |
| 2 | 25 g |
| 3 | 12.5 g |

Mass decreases exponentially.

Formula:

\[
M=100\left(\frac12\right)^t
\]

---

# 2. The Special Number \(e\) (Euler's Number)

---

## What is \(e\)?

A very special mathematical constant:

\[
e \approx 2.718281828...
\]

Similar to:

\[
\pi = 3.14159...
\]

It continues forever without repeating.

---

## Why is \(e\) Special?

Many natural processes grow continuously.

Examples:

- Population growth
- Interest compounded continuously
- Radioactive decay
- Heat transfer
- Machine learning
- Data science

These are naturally modeled using:

\[
e^x
\]

---

## Example 1: Continuous Growth

Instead of growing once per year:

- growth happens every second

Then:

\[
A=Pe^{rt}
\]

is the best model.

---

## Example 2: Continuous Compound Interest

If ₹1000 grows at 5% continuously:

\[
A=1000e^{0.05t}
\]

After 1 year:

\[
A=1000e^{0.05}
\]

\[
A \approx ₹1051.27
\]

---

# Calculus Property of \(e\)

Most functions change when differentiated.

Example:

\[
\frac{d}{dx}(x^2)=2x
\]

But:

\[
\frac{d}{dx}(e^x)=e^x
\]

The function remains exactly the same.

---

## Example

Suppose:

\[
y=e^3
\]

Then:

\[
y=20.085
\]

Slope at that point:

\[
20.085
\]

The height and slope are identical.

---

# Graphical Meaning

For:

\[
y=e^x
\]

At every point:

\[
\text{Slope} = \text{Height}
\]

---

## Example

At:

\[
x=0
\]

\[
y=e^0=1
\]

Slope = 1

---

At:

\[
x=1
\]

\[
y=e
\]

\[
y\approx2.718
\]

Slope = 2.718

---

At:

\[
x=2
\]

\[
y=e^2
\]

\[
y\approx7.389
\]

Slope = 7.389

---

# 3. Graphical Key Points (Intercepts)

Consider:

\[
y=a^x
\]

---

## Key Point 1: Y-Intercept

Set:

\[
x=0
\]

Then:

\[
y=a^0
\]

Any non-zero number raised to 0 equals 1.

Therefore:

\[
a^0=1
\]

So every exponential graph passes through:

\[
(0,1)
\]

---

## Examples

### Example 1

\[
y=2^x
\]

\[
2^0=1
\]

Point:

\[
(0,1)
\]

---

### Example 2

\[
y=5^x
\]

\[
5^0=1
\]

Point:

\[
(0,1)
\]

---

### Example 3

\[
y=e^x
\]

\[
e^0=1
\]

Point:

\[
(0,1)
\]

---

# Key Point 2: When \(x=1\)

Substitute:

\[
x=1
\]

\[
y=a^1=a
\]

Therefore point:

\[
(1,a)
\]

---

## Examples

### Example 1

\[
y=2^x
\]

\[
(1,2)
\]

---

### Example 2

\[
y=3^x
\]

\[
(1,3)
\]

---

### Example 3

\[
y=10^x
\]

\[
(1,10)
\]

---

# Quick Memory Trick

For any:

\[
y=a^x
\]

Always remember:

\[
(0,1)
\]

and

\[
(1,a)
\]

---

# 4. Fundamental Laws of Indices (Exponents)

---

# Law 1: Negative Exponents

Formula:

\[
a^{-n}=\frac1{a^n}
\]

---

## Example 1

\[
2^{-3}
\]

\[
=\frac1{2^3}
\]

\[
=\frac18
\]

---

## Example 2

\[
10^{-2}
\]

\[
=\frac1{10^2}
\]

\[
=\frac1{100}
\]

\[
=0.01
\]

---

## Easy Memory Trick

Negative exponent means:

**"Move to denominator."**

---

# Law 2: Multiplication Rule

Formula:

\[
a^n\times a^m=a^{n+m}
\]

---

## Example 1

\[
2^3\times2^4
\]

\[
=2^{3+4}
\]

\[
=2^7
\]

\[
=128
\]

---

## Example 2

\[
5^2\times5^3
\]

\[
=5^5
\]

\[
=3125
\]

---

## Easy Memory Trick

When multiplying same bases:

**Add exponents.**

---

# Law 3: Division Rule

Formula:

\[
\frac{a^n}{a^m}=a^{n-m}
\]

---

## Example 1

\[
\frac{2^5}{2^2}
\]

\[
=2^{5-2}
\]

\[
=2^3
\]

\[
=8
\]

---

## Example 2

\[
\frac{10^7}{10^3}
\]

\[
=10^4
\]

\[
=10000
\]

---

## Easy Memory Trick

When dividing same bases:

**Subtract exponents.**

---

# Law 4: Fractional Exponents

Formula:

\[
a^{1/n}=\sqrt[n]{a}
\]

---

## Example 1

\[
16^{1/2}
\]

\[
=\sqrt{16}
\]

\[
=4
\]

---

## Example 2

\[
27^{1/3}
\]

\[
=\sqrt[3]{27}
\]

\[
=3
\]

---

## Example 3

\[
81^{1/4}
\]

\[
=\sqrt[4]{81}
\]

\[
=3
\]

---

# Easy Memory Trick

Denominator = root

\[
a^{1/2}
\]

means square root.

\[
a^{1/3}
\]

means cube root.

---

# 5. Advanced Fractional Exponents

Formula:

\[
a^{m/n}
=
(\sqrt[n]{a})^m
\]

---

## Meaning

1. Take the root first.
2. Raise result to numerator power.

---

## Example 1

\[
8^{2/3}
\]

Step 1:

\[
\sqrt[3]{8}=2
\]

Step 2:

\[
2^2=4
\]

Answer:

\[
8^{2/3}=4
\]

---

## Example 2

\[
27^{2/3}
\]

Step 1:

\[
\sqrt[3]{27}=3
\]

Step 2:

\[
3^2=9
\]

Answer:

\[
9
\]

---

## Example 3

\[
16^{3/4}
\]

Step 1:

\[
\sqrt[4]{16}=2
\]

Step 2:

\[
2^3=8
\]

Answer:

\[
8
\]

---

# Shortcut Interpretation

\[
a^{m/n}
\]

means

"nth root first, then raise to m"

or

"raise to m first, then take nth root"

Both give the same answer.

---

# 6. Algebraic Proofs and Identities

---

# Combining Exponents

Suppose:

\[
a^{n/m}
\times
a^{q/k}
\]

Using multiplication rule:

\[
=a^{n/m+q/k}
\]

---

# Finding a Common Denominator

Add fractions:

\[
\frac{n}{m}
+
\frac{q}{k}
\]

Common denominator:

\[
mk
\]

Therefore:

\[
\frac{nk+qm}{mk}
\]

---

Hence:

\[
a^{n/m+q/k}
=
a^{(nk+qm)/(mk)}
\]

---

# Numerical Example

Simplify:

\[
2^{1/2}
\times
2^{1/3}
\]

Step 1:

Add exponents:

\[
2^{1/2+1/3}
\]

---

Step 2:

Common denominator:

\[
2^{3/6+2/6}
\]

\[
2^{5/6}
\]

Answer:

\[
2^{5/6}
\]

---

# Real-Life Interpretation

Imagine:

\[
2^{1/2}
\]

represents one growth process,

and

\[
2^{1/3}
\]

represents another growth process.

Combining them means multiplying the effects together.

The laws of exponents allow us to merge them into one simpler expression.

---

# Final Summary

## Exponential Function

\[
y=a^x
\]

Models:

- Population growth
- Compound interest
- Virus spread
- Radioactive decay

---

## Euler's Number

\[
e \approx 2.718
\]

Special because:

\[
\frac{d}{dx}(e^x)=e^x
\]

Height = Slope everywhere.

---

## Important Graph Points

Always:

\[
(0,1)
\]

and

\[
(1,a)
\]

---

## Laws of Exponents

Negative exponent:

\[
a^{-n}=\frac1{a^n}
\]

Multiplication:

\[
a^n a^m=a^{n+m}
\]

Division:

\[
\frac{a^n}{a^m}=a^{n-m}
\]

Fractional exponent:

\[
a^{1/n}=\sqrt[n]{a}
\]

Advanced fractional exponent:

\[
a^{m/n}=(\sqrt[n]{a})^m
\]

Combined exponents:

\[
a^{n/m+q/k}
=
a^{(nk+qm)/(mk)}
\]

---

### One-Sentence Memory Rule

**Exponential functions model repeated multiplication, and the laws of exponents are simply shortcuts that let us combine, simplify, and solve those repeated multiplications efficiently.**