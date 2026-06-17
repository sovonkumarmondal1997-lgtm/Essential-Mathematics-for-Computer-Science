# Fractional Number Systems and Radix Point

---

# Radix Point / Decimal Point

## Definition

A **radix point** is the symbol used to separate the whole-number part from the fractional part of a number.

In base 10, it is commonly called the **decimal point**.

Example:

```text
25.75
```

Here:

```text
25  → Whole Number Part

.   → Radix Point

75  → Fractional Part
```

---

## Example 1

```text
12.34
```

Meaning:

```text
12 + 0.34
```

---

## Example 2

```text
101.101₂
```

Meaning:

```text
101₂ + 0.101₂
```

The radix point works exactly like the decimal point but in binary.

---

# Decimal Fractional Representation

## Definition

Digits to the right of the decimal point represent **negative powers of 10**.

| Position | Power | Value |
|-----------|---------|---------|
| First Digit | 10⁻¹ | 0.1 |
| Second Digit | 10⁻² | 0.01 |
| Third Digit | 10⁻³ | 0.001 |
| Fourth Digit | 10⁻⁴ | 0.0001 |

---

## Example 1

```text
0.5
```

Calculation:

```text
5 × 10⁻¹

= 5 × 0.1

= 0.5
```

---

## Example 2

```text
0.25
```

Calculation:

```text
2 × 10⁻¹
+
5 × 10⁻²

=
0.2 + 0.05

=
0.25
```

---

## Example 3

```text
0.375
```

Calculation:

```text
3 × 10⁻¹
+
7 × 10⁻²
+
5 × 10⁻³

=
0.3 + 0.07 + 0.005

=
0.375
```

---

# Positional Notation / Place Value for Fractions

## Definition

For fractions, each position to the right of the radix point represents a negative power of the base.

---

## Example 1 (Decimal)

```text
24.37
```

Position Values:

```text
2 → 10¹

4 → 10⁰

3 → 10⁻¹

7 → 10⁻²
```

Calculation:

```text
(2×10)

+
(4×1)

+
(3×0.1)

+
(7×0.01)

=
20 + 4 + 0.3 + 0.07

=
24.37
```

---

## Example 2 (Binary)

```text
101.11₂
```

Position Values:

```text
4  2  1 . 1/2 1/4
```

Calculation:

```text
(1×4)

+
(0×2)

+
(1×1)

+
(1×0.5)

+
(1×0.25)

=
5.75
```

---

# Binary Fractional Representation

## Definition

Digits to the right of the binary radix point represent negative powers of 2.

---

## Binary Fractional Place Values

| Position | Power | Decimal Value |
|-----------|---------|---------|
| First | 2⁻¹ | 0.5 |
| Second | 2⁻² | 0.25 |
| Third | 2⁻³ | 0.125 |
| Fourth | 2⁻⁴ | 0.0625 |
| Fifth | 2⁻⁵ | 0.03125 |

---

## Example 1

```text
0.1₂
```

Calculation:

```text
1 × 2⁻¹

=
0.5
```

Answer:

```text
0.1₂ = 0.5₁₀
```

---

## Example 2

```text
0.11₂
```

Calculation:

```text
(1×0.5)

+
(1×0.25)

=
0.75
```

Answer:

```text
0.11₂ = 0.75₁₀
```

---

## Example 3

```text
0.101₂
```

Calculation:

```text
(1×0.5)

+
(0×0.25)

+
(1×0.125)

=
0.625
```

Answer:

```text
0.101₂ = 0.625₁₀
```

---

# Binary Fractional to Decimal Conversion

## Definition

Multiply each binary digit by its corresponding negative power of 2 and add the results.

---

## Example 1

Convert:

```text
0.101₂
```

Calculation:

```text
(1×0.5)

+
(0×0.25)

+
(1×0.125)

=
0.625
```

Answer:

```text
0.101₂ = 0.625₁₀
```

---

## Example 2

Convert:

```text
1.011₂
```

Calculation:

```text
1

+
(0×0.5)

+
(1×0.25)

+
(1×0.125)
```

```text
=
1 + 0 + 0.25 + 0.125

=
1.375
```

Answer:

```text
1.011₂ = 1.375₁₀
```

---

# Hexadecimal Fractional to Binary Fractional Conversion

## Definition

Convert each hexadecimal digit directly into a 4-bit binary group, including digits after the radix point.

---

## Example 1

Convert:

```text
A.F₁₆
```

Convert digits:

```text
A = 1010

F = 1111
```

Result:

```text
1010.1111₂
```

---

## Example 2

Convert:

```text
2.C₁₆
```

Convert digits:

```text
2 = 0010

C = 1100
```

Result:

```text
0010.1100₂
```

---

## Example 3

Convert:

```text
3.A5₁₆
```

Convert digits:

```text
3 = 0011

A = 1010

5 = 0101
```

Result:

```text
0011.10100101₂
```

---

# Binary Fractional to Octal Fractional Conversion

## Definition

Group binary digits into groups of three starting from the radix point and moving outward.

---

## Example 1

Convert:

```text
101.110₂
```

Group:

```text
101 . 110
```

Convert:

```text
101 = 5

110 = 6
```

Answer:

```text
5.6₈
```

---

## Example 2

Convert:

```text
1101.101₂
```

Add leading zeros:

```text
001 101 . 101
```

Convert:

```text
001 = 1

101 = 5

101 = 5
```

Answer:

```text
15.5₈
```

---

## Example 3

Convert:

```text
10.011₂
```

Group:

```text
010 . 011
```

Convert:

```text
010 = 2

011 = 3
```

Answer:

```text
2.3₈
```

---

# Decimal Fractional to Binary Fractional Conversion

## Definition

Represent the decimal fraction as a sum of negative powers of 2.

---

## Common Binary Fraction Values

| Binary Value | Decimal Value |
|-------------|---------------|
| 2⁻¹ | 0.5 |
| 2⁻² | 0.25 |
| 2⁻³ | 0.125 |
| 2⁻⁴ | 0.0625 |
| 2⁻⁵ | 0.03125 |

---

## Example 1

Convert:

```text
0.625₁₀
```

Break it into powers of 2:

```text
0.625

=
0.5 + 0.125
```

Place bits:

```text
0.5   → 1

0.25  → 0

0.125 → 1
```

Result:

```text
0.101₂
```

Verification:

```text
0.5 + 0 + 0.125

=
0.625
```

---

## Example 2

Convert:

```text
0.75₁₀
```

Break apart:

```text
0.75

=
0.5 + 0.25
```

Place bits:

```text
0.5  → 1

0.25 → 1
```

Result:

```text
0.11₂
```

Verification:

```text
0.5 + 0.25

=
0.75
```

---

## Example 3

Convert:

```text
0.375₁₀
```

Break apart:

```text
0.375

=
0.25 + 0.125
```

Place bits:

```text
0.5   → 0

0.25  → 1

0.125 → 1
```

Result:

```text
0.011₂
```

Verification:

```text
0 + 0.25 + 0.125

=
0.375
```

---

# Quick Revision Table

| Concept | Meaning |
|----------|---------|
| Radix Point | Separates whole and fractional parts |
| Decimal Fraction | Uses negative powers of 10 |
| Binary Fraction | Uses negative powers of 2 |
| Binary → Decimal | Add place values containing 1 |
| Hex → Binary | Replace each hex digit with 4 bits |
| Binary → Octal | Group bits in sets of 3 |
| Decimal Fraction → Binary | Express as powers of 2 |

---

# Important Fractional Place Values

## Decimal

```text
10⁻¹ = 0.1

10⁻² = 0.01

10⁻³ = 0.001
```

---

## Binary

```text
2⁻¹ = 0.5

2⁻² = 0.25

2⁻³ = 0.125

2⁻⁴ = 0.0625
```

---

# Memory Tricks

```text
Decimal fractions use powers of 10
```

```text
Binary fractions use powers of 2
```

```text
Hex digit = 4 binary bits
```

```text
Octal digit = 3 binary bits
```

```text
Move left of radix point → Positive powers

Move right of radix point → Negative powers
```