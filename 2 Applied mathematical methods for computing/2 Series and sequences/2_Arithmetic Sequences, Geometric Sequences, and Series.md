# Arithmetic Sequences, Geometric Sequences, and Series Fundamentals

---

# Introduction

In the previous chapter, we learned:

- Sequences
- Terms
- Natural Numbers
- Explicit Formulas
- Even Numbers
- Odd Numbers
- Perfect Squares
- First Differences

Now we will study two of the most important sequence types in mathematics:

1. Arithmetic Sequences
2. Geometric Sequences

These concepts are used in:

- Mathematics
- Computer Science
- Finance
- Data Science
- Machine Learning
- Population Growth Models
- Compound Interest Calculations

---

# 1. Prime Numbers Sequence

## Simple Definition

A **Prime Number** is a number greater than 1 that has exactly two positive divisors:

- 1
- Itself

---

## Prime Numbers Sequence

\[
2,3,5,7,11,13,17,19,23,29,\dots
\]

---

## Why Are They Special?

Prime numbers cannot be broken into smaller multiplication factors.

---

## Example 1

\[
7
\]

Divisors:

\[
1,\;7
\]

Prime ✔

---

## Example 2

\[
13
\]

Divisors:

\[
1,\;13
\]

Prime ✔

---

## Example 3

\[
12
\]

Divisors:

\[
1,2,3,4,6,12
\]

Not Prime ✘

---

## Real-Life Example

Prime numbers are heavily used in:

- Internet Security
- Cryptography
- Password Encryption
- Banking Systems

---

## Interesting Observation

The gaps between primes are irregular.

Example:

\[
2,3,5,7,11,13
\]

Differences:

\[
1,2,2,4,2
\]

No simple repeating pattern.

---

# 2. Arithmetic Sequence / Arithmetic Progression (AP)

## Simple Definition

An arithmetic sequence is a sequence where the difference between consecutive terms is always the same.

---

## General Pattern

\[
2,5,8,11,14,\dots
\]

---

Differences:

\[
+3,+3,+3,+3
\]

---

Same difference every time.

Therefore:

Arithmetic Sequence ✔

---

## Example 1

\[
1,4,7,10,13,\dots
\]

Difference:

\[
+3
\]

---

## Example 2

\[
10,20,30,40,50,\dots
\]

Difference:

\[
+10
\]

---

## Example 3

\[
100,95,90,85,80,\dots
\]

Difference:

\[
-5
\]

Still arithmetic.

---

## Real-Life Example

Monthly savings:

```
₹100
₹200
₹300
₹400
₹500
```

Increase:

\[
+100
\]

every month.

---

# Why Important?

Arithmetic sequences model:

- Fixed salary increases
- Equal savings plans
- Regular payments

---

# 3. First Term (a)

## Simple Definition

The first term is the starting value of a sequence.

---

Notation:

\[
a
\]

---

## Example 1

\[
5,8,11,14,\dots
\]

First term:

\[
a=5
\]

---

## Example 2

\[
100,110,120,130,\dots
\]

\[
a=100
\]

---

## Example 3

\[
-2,1,4,7,\dots
\]

\[
a=-2
\]

---

## Real-Life Example

Starting bank balance.

If you initially have:

\[
₹1000
\]

then:

\[
a=1000
\]

---

# Why Important?

The entire sequence begins from this value.

---

# 4. Common Difference (d)

## Simple Definition

The common difference is the fixed amount added (or subtracted) each time.

---

Notation:

\[
d
\]

---

## Formula

\[
d=u_2-u_1
\]

---

## Example 1

\[
2,5,8,11,\dots
\]

Difference:

\[
5-2=3
\]

\[
d=3
\]

---

## Example 2

\[
100,90,80,70,\dots
\]

Difference:

\[
90-100=-10
\]

\[
d=-10
\]

---

## Example 3

\[
1,1.5,2,2.5,\dots
\]

Difference:

\[
0.5
\]

---

## Real-Life Example

Weekly allowance increases by:

\[
₹50
\]

Then:

\[
d=50
\]

---

# 5. General nth Term Formula for Arithmetic Sequence

## Formula

\[
u_n=a+(n-1)d
\]

---

## Meaning

\[
a
\]

Starting value.

---

\[
(n-1)
\]

Number of jumps.

---

\[
d
\]

Size of each jump.

---

# Example 1

Sequence:

\[
2,5,8,11,\dots
\]

---

\[
a=2
\]

\[
d=3
\]

---

Find:

\[
u_{10}
\]

---

\[
u_{10}=2+(10-1)(3)
\]

\[
=2+27
\]

\[
=29
\]

---

# Example 2

\[
10,20,30,40,\dots
\]

---

\[
a=10
\]

\[
d=10
\]

---

\[
u_{15}
=
10+(14)(10)
\]

\[
=150
\]

---

# Example 3

\[
100,95,90,\dots
\]

---

\[
a=100
\]

\[
d=-5
\]

---

\[
u_6
=
100+5(-5)
\]

\[
=75
\]

---

# Why Useful?

Directly calculate any term.

No need to generate the entire sequence.

---

# 6. Geometric Sequence / Geometric Progression (GP)

## Simple Definition

A geometric sequence is formed by multiplying each term by the same number.

---

## Example

\[
2,4,8,16,32,\dots
\]

---

Multiplication:

\[
\times2
\]

every time.

---

## Example 1

\[
3,6,12,24,\dots
\]

Ratio:

\[
\times2
\]

---

## Example 2

\[
5,15,45,135,\dots
\]

Ratio:

\[
\times3
\]

---

## Example 3

\[
100,50,25,12.5,\dots
\]

Ratio:

\[
\times0.5
\]

---

## Real-Life Example

Compound interest.

Money grows by a percentage.

---

# Arithmetic vs Geometric

Arithmetic:

```
+3
+3
+3
```

---

Geometric:

```
×3
×3
×3
```

---

# 7. Common Ratio (r)

## Simple Definition

The common ratio is the constant multiplier.

---

Notation:

\[
r
\]

---

## Formula

\[
r=
\frac{u_2}{u_1}
\]

---

## Example 1

\[
2,4,8,16
\]

---

\[
r=2
\]

---

## Example 2

\[
3,9,27,81
\]

---

\[
r=3
\]

---

## Example 3

\[
100,50,25,12.5
\]

---

\[
r=0.5
\]

---

## Real-Life Example

Investment grows:

10%

each year.

Then:

\[
r=1.1
\]

---

# 8. General nth Term Formula for Geometric Sequence

## Formula

\[
u_n=ar^{n-1}
\]

---

## Meaning

\[
a
\]

First term.

---

\[
r
\]

Common ratio.

---

\[
n-1
\]

Number of multiplications.

---

# Example 1

\[
2,4,8,16,\dots
\]

---

\[
a=2
\]

\[
r=2
\]

---

\[
u_8
=
2(2^7)
\]

\[
=256
\]

---

# Example 2

\[
3,9,27,\dots
\]

---

\[
u_5
=
3(3^4)
\]

\[
=243
\]

---

# Example 3

\[
100,50,25,\dots
\]

---

\[
u_6
=
100(0.5)^5
\]

\[
=3.125
\]

---

# Why Useful?

Find very large terms instantly.

---

# 9. Binary Powers of Two

## Simple Definition

A special geometric sequence generated by powers of 2.

---

## Sequence

\[
2^0,2^1,2^2,2^3,2^4,\dots
\]

---

Values:

\[
1,2,4,8,16,32,\dots
\]

---

## Example 1

\[
2^5=32
\]

---

## Example 2

\[
2^8=256
\]

---

## Example 3

\[
2^{10}=1024
\]

---

# Why Important in Computing?

Computers use binary.

Everything is based on powers of 2.

---

Examples:

```
8 bits
16 bits
32 bits
64 bits
```

---

Memory sizes:

```
1024 Bytes
1024 KB
1024 MB
```

---

# Real-Life Example

Chessboard Rice Problem.

Grains double on every square.

Growth becomes enormous.

---

# 10. Summing / Series

## Simple Definition

A sequence is a list.

A series is the sum of that list.

---

## Sequence Example

\[
1,2,3,4,5
\]

---

## Series Example

\[
1+2+3+4+5
\]

---

Result:

\[
15
\]

---

# Example 1

Arithmetic Series

Sequence:

\[
2,5,8,11
\]

Series:

\[
2+5+8+11
\]

\[
=26
\]

---

# Example 2

Geometric Series

Sequence:

\[
1,2,4,8
\]

Series:

\[
1+2+4+8
\]

\[
=15
\]

---

# Example 3

Squares

Sequence:

\[
1,4,9,16
\]

Series:

\[
1+4+9+16
\]

\[
=30
\]

---

# Why Important?

Series help calculate:

- Total savings
- Total distance
- Total profit
- Total interest
- Probability calculations

---

# Complete Big Picture

## Prime Numbers

\[
2,3,5,7,11,\dots
\]

Numbers divisible only by:

- 1
- Themselves

---

## Arithmetic Sequence

Constant difference.

\[
u_n=a+(n-1)d
\]

---

## First Term

\[
a
\]

Starting value.

---

## Common Difference

\[
d
\]

Fixed amount added.

---

## Geometric Sequence

Constant multiplier.

\[
u_n=ar^{n-1}
\]

---

## Common Ratio

\[
r
\]

Fixed multiplication factor.

---

## Binary Powers of Two

\[
1,2,4,8,16,\dots
\]

Foundation of computing.

---

## Series

The sum of sequence terms.

---

Arithmetic Sequence:

```
Add constant amount
```

---

Geometric Sequence:

```
Multiply by constant ratio
```

---

These concepts form the foundation for:

- Mathematical Induction
- Recurrence Relations
- Algorithm Analysis
- Dynamic Programming
- Compound Interest
- Population Growth
- Probability Theory
- Machine Learning
- Time-Series Forecasting
- Financial Modeling
- Computer Science

where recognizing patterns and understanding growth is essential.