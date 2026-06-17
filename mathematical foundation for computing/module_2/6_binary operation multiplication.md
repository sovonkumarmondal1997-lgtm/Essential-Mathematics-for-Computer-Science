# Binary Multiplication

---

# Binary Multiplication

## Definition

**Binary Multiplication** is the process of multiplying two binary numbers (base 2) using only the digits:

```text
0 and 1
```

It works very similarly to decimal multiplication, except there are only four multiplication rules.

---

# Binary Multiplication Rules

| Multiplication | Result |
|---------------|---------|
| 0 × 0 | 0 |
| 0 × 1 | 0 |
| 1 × 0 | 0 |
| 1 × 1 | 1 |

---

## Example 1

Multiply:

```text
1₂ × 1₂
```

Result:

```text
1₂
```

Verification:

```text
1 × 1 = 1
```

---

## Example 2

Multiply:

```text
10₂ × 1₂
```

Result:

```text
10₂
```

Verification:

```text
2 × 1 = 2
```

---

## Example 3

Multiply:

```text
11₂ × 10₂
```

Verification:

```text
11₂ = 3

10₂ = 2
```

Result:

```text
110₂
```

Check:

```text
3 × 2 = 6

110₂ = 6
```

Correct.

---

# Partial Products

## Definition

**Partial Products** are the intermediate multiplication results obtained by multiplying the multiplicand by each bit of the multiplier.

These partial products are later added together.

---

## Decimal Analogy

Decimal:

```text
 23
×12
---
 46
230
---
276
```

Here:

```text
46

230
```

are partial products.

---

## Binary Example 1

Multiply:

```text
101₂ × 11₂
```

Step 1

Multiply by rightmost bit:

```text
101 × 1

= 101
```

Partial Product 1:

```text
101
```

Step 2

Multiply by second bit:

```text
101 × 1

= 101
```

Shift left one place:

```text
1010
```

Partial Product 2:

```text
1010
```

---

## Example 2

Multiply:

```text
110₂ × 101₂
```

Multiplier:

```text
101
```

Generate partial products:

```text
110

000

11000
```

These are the partial products.

---

# Bit Shifting / Placeholder Zeros

## Definition

When multiplying by a bit in a higher position, we shift the partial product left by adding zeros.

Each shift corresponds to a power of 2.

---

## Important Rule

| Position | Shift |
|-----------|---------|
| 2⁰ column | 0 shifts |
| 2¹ column | 1 shift |
| 2² column | 2 shifts |
| 2³ column | 3 shifts |

---

# Example 1

```text
101 × 10₂
```

The multiplier bit is in the:

```text
2¹ column
```

Shift one position:

```text
1010
```

---

# Example 2

```text
101 × 100₂
```

The multiplier bit is in:

```text
2² column
```

Shift two positions:

```text
10100
```

---

# Example 3

```text
111 × 1000₂
```

The multiplier bit is in:

```text
2³ column
```

Shift three positions:

```text
111000
```

---

# Understanding Why Shifting Works

Decimal Example:

```text
25 × 10

= 250
```

You add one zero.

Similarly:

```text
101₂ × 10₂

= 1010₂
```

You shift left one position.

---

# Zero Multiplication Property

## Definition

Any number multiplied by zero equals zero.

---

## Formula

```text
A × 0 = 0
```

---

## Example 1

```text
101₂ × 0

= 0
```

---

## Example 2

```text
1111₂ × 0

= 0
```

---

## Example 3

```text
100101₂ × 0

= 0
```

---

# Why This Is Important

During multiplication:

```text
1 → Generate partial product

0 → Generate nothing
```

or simply:

```text
0000...
```

---

## Example

Multiply:

```text
101 × 101
```

Multiplier:

```text
101
```

Middle bit:

```text
0
```

Therefore:

```text
000
```

can be skipped.

---

# Binary Addition with Carrying

## Definition

After generating all partial products, we add them together using binary addition rules.

---

## Binary Addition Rules

| Addition | Result |
|-----------|---------|
| 0 + 0 | 0 |
| 0 + 1 | 1 |
| 1 + 0 | 1 |
| 1 + 1 | 10 |
| 1 + 1 + 1 | 11 |

---

# Example 1

Multiply:

```text
101₂ × 11₂
```

Step 1: Generate Partial Products

```text
   101
×   11
------
   101
+1010
------
```

Step 2: Add

```text
   0101
+ 1010
-------
   1111
```

Result:

```text
1111₂
```

Verification:

```text
101₂ = 5

11₂ = 3

1111₂ = 15
```

Check:

```text
5 × 3 = 15
```

Correct.

---

# Example 2

Multiply:

```text
110₂ × 101₂
```

Partial Products:

```text
     110
    000
+11000
------
```

Add:

```text
00110
00000
11000
-----
11110
```

Result:

```text
11110₂
```

Verification:

```text
6 × 5 = 30
```

And:

```text
11110₂ = 30
```

Correct.

---

# Complete Multiplication Example

Multiply:

```text
1011₂ × 110₂
```

---

## Step 1: Generate Partial Products

Rightmost bit:

```text
1011 × 0

= 0000
```

---

Second bit:

```text
1011 × 1

= 1011

Shift 1 place

= 10110
```

---

Third bit:

```text
1011 × 1

= 1011

Shift 2 places

= 101100
```

---

## Step 2: Add

```text
  000000
  010110
+101100
--------
 1000010
```

---

## Final Answer

```text
1000010₂
```

---

# Arithmetic Verification via Base Conversion

## Definition

After binary multiplication, convert all binary values to decimal.

If the decimal multiplication matches, the binary multiplication is correct.

---

# Example 1

Binary:

```text
101₂ × 11₂ = 1111₂
```

Convert:

```text
101₂ = 5

11₂ = 3

1111₂ = 15
```

Check:

```text
5 × 3 = 15
```

Correct.

---

# Example 2

Binary:

```text
110₂ × 101₂ = 11110₂
```

Convert:

```text
110₂ = 6

101₂ = 5

11110₂ = 30
```

Check:

```text
6 × 5 = 30
```

Correct.

---

# Example 3

Binary:

```text
100₂ × 11₂ = 1100₂
```

Convert:

```text
100₂ = 4

11₂ = 3

1100₂ = 12
```

Check:

```text
4 × 3 = 12
```

Correct.

---

# Full Workflow Summary

## Step 1

Multiply by each bit.

```text
Generate partial products
```

---

## Step 2

Shift left according to bit position.

```text
Add placeholder zeros
```

---

## Step 3

Add all partial products.

```text
Binary addition
```

---

## Step 4

Obtain final binary answer.

---

## Step 5

Verify using decimal conversion.

---

# Quick Revision Sheet

| Concept | Meaning |
|----------|---------|
| Binary Multiplication | Multiplication in base 2 |
| Partial Product | Intermediate multiplication result |
| Bit Shift | Move left by adding zeros |
| Shift 1 Position | ×2 |
| Shift 2 Positions | ×4 |
| Shift 3 Positions | ×8 |
| Zero Multiplication | Any number × 0 = 0 |
| Binary Addition | Sum all partial products |
| Verification | Convert to decimal and check |

---

# Important Binary Multiplication Rules

| Rule | Result |
|--------|---------|
| 0 × 0 | 0 |
| 0 × 1 | 0 |
| 1 × 0 | 0 |
| 1 × 1 | 1 |

---

# Memory Tricks

```text
Binary multiplication is repeated binary addition.
```

```text
A 1 bit copies the multiplicand.
```

```text
A 0 bit contributes nothing.
```

```text
Each left shift multiplies by 2.
```

```text
Shift 1 place → ×2

Shift 2 places → ×4

Shift 3 places → ×8
```

```text
Always verify by converting to decimal.
```