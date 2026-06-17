# Binary Arithmetic

---

# Binary Arithmetic

## Definition

**Binary Arithmetic** is the process of performing mathematical operations using binary numbers (base 2), which contain only the digits:

```text
0 and 1
```

Just like decimal arithmetic uses:

```text
0,1,2,3,4,5,6,7,8,9
```

binary arithmetic uses only:

```text
0 and 1
```

Computers perform all calculations using binary arithmetic.

---

## Example 1

Decimal:

```text
5 + 3 = 8
```

Binary:

```text
101₂ + 011₂ = 1000₂
```

Verification:

```text
101₂ = 5

011₂ = 3

1000₂ = 8
```

---

## Example 2

Decimal:

```text
2 + 6 = 8
```

Binary:

```text
10₂ + 110₂ = 1000₂
```

---

# Binary Addition

## Definition

**Binary Addition** is the process of adding binary numbers column by column, starting from the rightmost bit.

It works exactly like decimal column addition, except the base is:

```text
2 instead of 10
```

---

# Basic Binary Addition Rules

| Addition | Result |
|-----------|---------|
| 0 + 0 | 0 |
| 0 + 1 | 1 |
| 1 + 0 | 1 |
| 1 + 1 | 10 |

---

## Example 1

```text
  101
+ 010
-----
  111
```

Verification:

```text
101₂ = 5

010₂ = 2

111₂ = 7
```

And:

```text
5 + 2 = 7
```

Correct.

---

## Example 2

```text
  110
+ 001
-----
  111
```

Verification:

```text
110₂ = 6

001₂ = 1

111₂ = 7
```

Correct.

---

## Example 3

```text
  1011
+ 0101
------
 10000
```

Verification:

```text
1011₂ = 11

0101₂ = 5

10000₂ = 16
```

Correct.

---

# Carry-over / Carry Bit

## Definition

A **carry bit** occurs when the sum of a binary column becomes:

```text
2 or more
```

Since binary can only store:

```text
0 or 1
```

the extra value must be carried into the next column.

---

# Example 1

```text
1 + 1
```

Decimal Value:

```text
1 + 1 = 2
```

Binary Representation of 2:

```text
10₂
```

Result:

```text
Write 0

Carry 1
```

---

### Visual Representation

```text
Carry: 1

  1
+ 1
----
 10
```

---

# Example 2

```text
  11
+ 01
----
```

Step 1

```text
1 + 1 = 10

Write 0

Carry 1
```

Step 2

```text
1 + 0 + Carry(1)

= 10
```

Final Answer:

```text
100₂
```

Verification:

```text
3 + 1 = 4
```

Correct.

---

# Example 3

```text
 111
+001
----
```

Step-by-step:

```text
1+1 = 10

Write 0

Carry 1
```

Next:

```text
1+0+1

=10

Write 0

Carry 1
```

Next:

```text
1+0+1

=10
```

Result:

```text
1000₂
```

Verification:

```text
7 + 1 = 8
```

Correct.

---

# Binary Sum Rules

---

## Rule 1

```text
1₂ + 1₂ = 10₂
```

Explanation:

```text
1 + 1 = 2
```

Binary representation of 2:

```text
10₂
```

---

## Example

```text
1 + 1 = 10
```

---

## Rule 2

```text
1₂ + 1₂ + 1₂ = 11₂
```

Explanation:

```text
1 + 1 + 1 = 3
```

Binary representation of 3:

```text
11₂
```

---

## Example

```text
1

1

1

↓

11₂
```

---

# Extended Binary Sum Rules

| Binary Addition | Result |
|----------------|---------|
| 0 + 0 | 0 |
| 0 + 1 | 1 |
| 1 + 0 | 1 |
| 1 + 1 | 10 |
| 1 + 1 + 1 | 11 |
| 1 + 1 + 1 + 1 | 100 |

---

## Example

```text
1+1+1+1
```

Decimal:

```text
4
```

Binary:

```text
100₂
```

---

# Digital / Computer Constraints

## Definition

Computers are digital devices that use only two electrical states:

```text
OFF = 0

ON = 1
```

Because of this, computers can only directly work with:

```text
0 and 1
```

---

# Example 1

A light switch:

```text
OFF → 0

ON  → 1
```

---

# Example 2

Computer Memory

A single bit can store only:

```text
0

or

1
```

Not:

```text
2

3

4
```

---

# Example 3

CPU Logic Circuits

Voltage:

```text
0V → 0

5V → 1
```

This is why binary is fundamental to computing.

---

# Positional Place Values in Binary Columns

## Definition

Each binary position represents a power of 2.

---

## Binary Place Value Table

| Position | Value |
|-----------|---------|
| 2⁰ | 1 |
| 2¹ | 2 |
| 2² | 4 |
| 2³ | 8 |
| 2⁴ | 16 |
| 2⁵ | 32 |
| 2⁶ | 64 |

---

# Example 1

Binary Number:

```text
101₂
```

Positions:

```text
4   2   1
```

Calculation:

```text
(1×4)

+
(0×2)

+
(1×1)

=
5
```

---

# Example 2

Binary Number:

```text
1101₂
```

Positions:

```text
8 4 2 1
```

Calculation:

```text
8 + 4 + 0 + 1

=
13
```

---

# Example 3

Binary Number:

```text
10010₂
```

Positions:

```text
16 8 4 2 1
```

Calculation:

```text
16 + 2

=
18
```

---

# Binary-to-Decimal Conversion Verification

## Definition

After performing binary arithmetic, we can verify the answer by converting all binary numbers into decimal.

If both decimal calculations match, the binary answer is correct.

---

# Example 1

Binary Addition:

```text
101₂

+
011₂

=

1000₂
```

Convert:

```text
101₂ = 5

011₂ = 3

1000₂ = 8
```

Check:

```text
5 + 3 = 8
```

Correct.

---

# Example 2

Binary Addition:

```text
110₂

+
010₂

=

1000₂
```

Convert:

```text
110₂ = 6

010₂ = 2

1000₂ = 8
```

Check:

```text
6 + 2 = 8
```

Correct.

---

# Example 3

Binary Addition:

```text
111₂

+
001₂

=

1000₂
```

Convert:

```text
111₂ = 7

001₂ = 1

1000₂ = 8
```

Check:

```text
7 + 1 = 8
```

Correct.

---

# Complete Binary Addition Example

Add:

```text
1011₂

+
1101₂
```

Step 1

```text
1+1 = 10

Write 0

Carry 1
```

Step 2

```text
1+0+1

=10

Write 0

Carry 1
```

Step 3

```text
0+1+1

=10

Write 0

Carry 1
```

Step 4

```text
1+1+1

=11

Write 1

Carry 1
```

Final Result:

```text
11000₂
```

---

## Verification

Convert:

```text
1011₂ = 11

1101₂ = 13

11000₂ = 24
```

Check:

```text
11 + 13 = 24
```

Correct.

---

# Quick Revision Sheet

| Concept | Meaning |
|----------|---------|
| Binary Arithmetic | Mathematical operations in base 2 |
| Binary Addition | Adding binary numbers column by column |
| Carry Bit | Extra value transferred to next column |
| 1 + 1 | 10₂ |
| 1 + 1 + 1 | 11₂ |
| Binary Digits | 0 and 1 only |
| Binary Place Values | Powers of 2 |
| Verification | Convert binary answers to decimal and check |

---

# Important Binary Place Values

```text
2⁰ = 1

2¹ = 2

2² = 4

2³ = 8

2⁴ = 16

2⁵ = 32

2⁶ = 64
```

---

# Memory Tricks

```text
Binary uses only 0 and 1
```

```text
1 + 1 = 10
```

```text
1 + 1 + 1 = 11
```

```text
Whenever a column reaches 2,
carry 1 to the next column.
```

```text
To verify binary arithmetic,
convert everything to decimal.
```