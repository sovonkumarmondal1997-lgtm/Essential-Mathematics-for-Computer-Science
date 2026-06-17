# Number Systems and Binary Numbers

---

# What is a Number Base?

## Definition

A **number base** (or radix) is the number of unique digits used to represent numbers in a number system.

### Formula

```text
Base = Total number of unique symbols available
```

---

# Understanding Number Bases

We use different number systems in mathematics and computers.

| Number System | Base | Digits Used |
|--------------|------|-------------|
| Binary | 2 | 0, 1 |
| Octal | 8 | 0-7 |
| Decimal | 10 | 0-9 |
| Hexadecimal | 16 | 0-9, A-F |

---

# Why Do We Need Different Number Bases?

Humans naturally use:

```text
Decimal (Base 10)
```

because we have ten fingers.

Computers use:

```text
Binary (Base 2)
```

because electronic circuits have only two states:

```text
ON  = 1
OFF = 0
```

---

# Decimal Number System (Base 10)

## Digits Used

```text
0,1,2,3,4,5,6,7,8,9
```

### Example

```text
538
```

Expanded Form:

```text
538

= (5 × 10²) + (3 × 10¹) + (8 × 10⁰)

= (5 × 100) + (3 × 10) + (8 × 1)

= 500 + 30 + 8

= 538
```

---

# Binary Number System (Base 2)

## Digits Used

```text
0 and 1
```

### Example

```text
1011₂
```

Expanded Form:

```text
1011₂

= (1 × 2³)
+ (0 × 2²)
+ (1 × 2¹)
+ (1 × 2⁰)
```

```text
= 8 + 0 + 2 + 1

= 11₁₀
```

---

# Octal Number System (Base 8)

## Digits Used

```text
0,1,2,3,4,5,6,7
```

### Example

```text
347₈
```

Expanded Form:

```text
347₈

= (3 × 8²)
+ (4 × 8¹)
+ (7 × 8⁰)

= (3 × 64)
+ (4 × 8)
+ (7 × 1)

= 192 + 32 + 7

= 231₁₀
```

---

# Hexadecimal Number System (Base 16)

## Digits Used

```text
0,1,2,3,4,5,6,7,8,9,A,B,C,D,E,F
```

Where:

```text
A = 10
B = 11
C = 12
D = 13
E = 14
F = 15
```

---

## Example

```text
2F₁₆
```

Expanded Form:

```text
2F₁₆

= (2 × 16¹)
+ (15 × 16⁰)

= (2 × 16)
+ (15 × 1)

= 32 + 15

= 47₁₀
```

---

# Binary Number System (Detailed)

## Definition

A **binary number system** is a base-2 number system that uses only two digits:

```text
0 and 1
```

Every position represents a power of 2.

---

# Binary Example 1

Binary Number:

```text
10101₂
```

Place Values:

```text
1     0     1     0     1
↓     ↓     ↓     ↓     ↓
2⁴   2³   2²   2¹   2⁰
```

Substitute Values:

```text
(1 × 16)
+
(0 × 8)
+
(1 × 4)
+
(0 × 2)
+
(1 × 1)
```

Calculation:

```text
16 + 0 + 4 + 0 + 1

= 21
```

Therefore:

```text
10101₂ = 21₁₀
```

---

# Binary Example 2

Binary Number:

```text
110110₂
```

Place Values:

```text
1   1   0   1   1   0
↓   ↓   ↓   ↓   ↓   ↓
32 16  8   4   2   1
```

Calculation:

```text
32 + 16 + 0 + 4 + 2 + 0

= 54
```

Therefore:

```text
110110₂ = 54₁₀
```

---

# Binary to Decimal Conversion

## Definition

To convert binary to decimal:

```text
Multiply each binary digit by its power of 2 and add the results.
```

---

# Binary to Decimal Example 1

Convert:

```text
1011₂
```

Step 1: Write Powers of 2

```text
1    0    1    1
↓    ↓    ↓    ↓
2³  2²  2¹  2⁰
```

Step 2: Multiply

```text
(1 × 8)
+
(0 × 4)
+
(1 × 2)
+
(1 × 1)
```

Step 3: Add

```text
8 + 0 + 2 + 1

= 11
```

Answer:

```text
1011₂ = 11₁₀
```

---

# Binary to Decimal Example 2

Convert:

```text
11001₂
```

Step 1:

```text
1    1    0    0    1
↓    ↓    ↓    ↓    ↓
16   8    4    2    1
```

Step 2:

```text
16 + 8 + 0 + 0 + 1
```

Step 3:

```text
= 25
```

Answer:

```text
11001₂ = 25₁₀
```

---

# Decimal to Binary Conversion

## Definition

To convert decimal to binary:

```text
Repeatedly divide the number by 2 and write down the remainders.
```

Read the remainders from bottom to top.

---

# Decimal to Binary Example 1

Convert:

```text
13₁₀
```

Step 1: Divide by 2

| Division | Quotient | Remainder |
|-----------|-----------|-----------|
| 13 ÷ 2 | 6 | 1 |
| 6 ÷ 2 | 3 | 0 |
| 3 ÷ 2 | 1 | 1 |
| 1 ÷ 2 | 0 | 1 |

Step 2: Read Bottom to Top

```text
1101₂
```

Answer:

```text
13₁₀ = 1101₂
```

---

# Decimal to Binary Example 2

Convert:

```text
25₁₀
```

Step 1: Divide by 2

| Division | Quotient | Remainder |
|-----------|-----------|-----------|
| 25 ÷ 2 | 12 | 1 |
| 12 ÷ 2 | 6 | 0 |
| 6 ÷ 2 | 3 | 0 |
| 3 ÷ 2 | 1 | 1 |
| 1 ÷ 2 | 0 | 1 |

Step 2: Read Bottom to Top

```text
11001₂
```

Answer:

```text
25₁₀ = 11001₂
```

---

# Quick Binary Place Value Table

| Power of 2 | Value |
|------------|--------|
| 2⁰ | 1 |
| 2¹ | 2 |
| 2² | 4 |
| 2³ | 8 |
| 2⁴ | 16 |
| 2⁵ | 32 |
| 2⁶ | 64 |
| 2⁷ | 128 |
| 2⁸ | 256 |
| 2⁹ | 512 |

---

# Quick Revision Sheet

| Conversion | Method |
|------------|---------|
| Binary → Decimal | Multiply digits by powers of 2 and add |
| Decimal → Binary | Repeatedly divide by 2 and read remainders bottom-up |
| Binary Digits | 0,1 |
| Binary Base | 2 |
| Decimal Digits | 0-9 |
| Decimal Base | 10 |
| Octal Digits | 0-7 |
| Octal Base | 8 |
| Hexadecimal Digits | 0-9, A-F |
| Hexadecimal Base | 16 |

---

# Important Formulas

## Binary to Decimal

```text
Number

=
(dₙ × 2ⁿ)
+
(dₙ₋₁ × 2ⁿ⁻¹)
+
...
+
(d₀ × 2⁰)
```

---

## Decimal to Binary

```text
Repeatedly divide by 2

Store remainders

Read remainders from bottom to top
```

---

# Memory Trick

```text
Binary → Multiply and Add

Decimal → Divide and Collect Remainders
```

This single rule solves most binary conversion problems.