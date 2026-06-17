# Binary Subtraction

---

# Binary Subtraction

## Definition

**Binary Subtraction** is the process of subtracting one binary number from another using only the digits:

```text
0 and 1
```

Just like decimal subtraction, binary subtraction is performed column by column from right to left.

---

## Basic Binary Subtraction Rules

| Subtraction | Result |
|------------|---------|
| 0 - 0 | 0 |
| 1 - 0 | 1 |
| 1 - 1 | 0 |
| 0 - 1 | Borrow Required |

---

## Example 1

Subtract:

```text
101₂ - 001₂
```

Calculation:

```text
  101
- 001
-----
  100
```

Verification:

```text
101₂ = 5

001₂ = 1

100₂ = 4
```

Check:

```text
5 - 1 = 4
```

Correct.

---

## Example 2

Subtract:

```text
111₂ - 010₂
```

Calculation:

```text
  111
- 010
-----
  101
```

Verification:

```text
111₂ = 7

010₂ = 2

101₂ = 5
```

Check:

```text
7 - 2 = 5
```

Correct.

---

## Example 3

Subtract:

```text
1100₂ - 0011₂
```

Calculation:

```text
 1100
-0011
-----
 1001
```

Verification:

```text
1100₂ = 12

0011₂ = 3

1001₂ = 9
```

Check:

```text
12 - 3 = 9
```

Correct.

---

# Borrowing in Binary (Regrouping)

## Definition

**Borrowing** occurs when the top digit is smaller than the bottom digit.

Example:

```text
0 - 1
```

This cannot be done directly.

So we borrow:

```text
1
```

from the next higher column.

---

## Important Idea

When we borrow:

```text
1
```

from the next binary column, it becomes:

```text
10₂
```

which equals:

```text
2₁₀
```

---

## Example 1

```text
 10
-01
---
```

Rightmost column:

```text
0 - 1
```

Cannot do.

Borrow from the left.

```text
10₂ becomes

0 10
```

Now:

```text
10₂ - 1₂

=
1₂
```

Result:

```text
01₂
```

Answer:

```text
10₂ - 01₂ = 01₂
```

Verification:

```text
2 - 1 = 1
```

Correct.

---

## Example 2

```text
100₂ - 001₂
```

Rightmost:

```text
0 - 1
```

Need borrow.

Borrow from middle column.

Result:

```text
011₂
```

Verification:

```text
4 - 1 = 3
```

Correct.

---

## Example 3

```text
1010₂ - 0001₂
```

Result:

```text
1001₂
```

Verification:

```text
10 - 1 = 9
```

Correct.

---

# The Subtraction Rule

# 10₂ - 1₂ = 1₂

## Definition

This is the most important borrowing rule in binary subtraction.

---

## Why?

```text
10₂
```

equals:

```text
2₁₀
```

Therefore:

```text
2 - 1 = 1
```

So:

```text
10₂ - 1₂ = 1₂
```

---

## Example 1

```text
10₂ - 1₂
```

Decimal:

```text
2 - 1 = 1
```

Answer:

```text
1₂
```

---

## Example 2

```text
110₂ - 001₂
```

Borrowing creates:

```text
10₂ - 1₂
```

which becomes:

```text
1₂
```

Result:

```text
101₂
```

Verification:

```text
6 - 1 = 5
```

Correct.

---

## Example 3

```text
100₂ - 010₂
```

Result:

```text
010₂
```

Verification:

```text
4 - 2 = 2
```

Correct.

---

# Sequential / Long-Distance Borrowing

## Definition

**Sequential borrowing** occurs when several consecutive zeros block access to a borrow.

The borrow must travel across multiple columns until it reaches a column containing a 1.

---

# Example 1

Subtract:

```text
1000₂ - 0001₂
```

Start:

```text
 1000
-0001
------
```

Rightmost:

```text
0 - 1
```

Need borrow.

Next column:

```text
0
```

Cannot borrow.

Next column:

```text
0
```

Cannot borrow.

Next column:

```text
1
```

Borrow from here.

---

Borrow chain:

```text
1000

↓

0111
```

Now:

```text
111₂
```

Result:

```text
0111₂
```

Verification:

```text
8 - 1 = 7
```

Correct.

---

# Example 2

Subtract:

```text
10000₂ - 00001₂
```

Borrow travels across:

```text
0
0
0
0
```

until reaching:

```text
1
```

Result:

```text
01111₂
```

Verification:

```text
16 - 1 = 15
```

Correct.

---

# Example 3

Subtract:

```text
100000₂ - 000001₂
```

Borrow chain:

```text
100000

↓

011111
```

Result:

```text
011111₂
```

Verification:

```text
32 - 1 = 31
```

Correct.

---

# Visualizing Long-Distance Borrowing

Example:

```text
10000₂ - 1₂
```

Before Borrow:

```text
1 0 0 0 0
```

Borrow travels left to right:

```text
0 1 1 1 10
```

Now subtraction becomes easy.

Result:

```text
1111₂
```

---

# Binary-to-Decimal Cross-Checking

## Definition

After performing binary subtraction, convert all values into decimal numbers.

If decimal subtraction produces the same answer, the binary subtraction is correct.

---

# Example 1

Binary:

```text
101₂ - 010₂ = 011₂
```

Convert:

```text
101₂ = 5

010₂ = 2

011₂ = 3
```

Check:

```text
5 - 2 = 3
```

Correct.

---

# Example 2

Binary:

```text
1100₂ - 0011₂ = 1001₂
```

Convert:

```text
1100₂ = 12

0011₂ = 3

1001₂ = 9
```

Check:

```text
12 - 3 = 9
```

Correct.

---

# Example 3

Binary:

```text
10000₂ - 00001₂ = 01111₂
```

Convert:

```text
10000₂ = 16

00001₂ = 1

01111₂ = 15
```

Check:

```text
16 - 1 = 15
```

Correct.

---

# Complete Worked Example

Subtract:

```text
10110₂ - 00101₂
```

Step 1

```text
 10110
-00101
------
```

Rightmost:

```text
0 - 1

Borrow required
```

Borrow:

```text
10₂ - 1₂

= 1₂
```

Continue:

```text
Result = 10001₂
```

---

## Verification

Convert:

```text
10110₂

=
22
```

Convert:

```text
00101₂

=
5
```

Convert Answer:

```text
10001₂

=
17
```

Check:

```text
22 - 5 = 17
```

Correct.

---

# Quick Comparison

## Decimal Borrowing

```text
10 - 7

Borrow 1 ten

Convert to 10 ones
```

---

## Binary Borrowing

```text
0 - 1

Borrow 1 binary digit

Convert to 10₂
```

---

# Quick Revision Sheet

| Concept | Meaning |
|----------|---------|
| Binary Subtraction | Subtracting binary numbers |
| Borrowing | Taking value from higher column |
| 10₂ - 1₂ | 1₂ |
| Long-Distance Borrowing | Borrowing across multiple zero columns |
| Cross-Checking | Verify using decimal conversion |
| Binary Digits | 0 and 1 only |
| Borrowed 1 | Becomes 10₂ in current column |

---

# Important Binary Subtraction Rules

| Rule | Result |
|--------|---------|
| 0 - 0 | 0 |
| 1 - 0 | 1 |
| 1 - 1 | 0 |
| 0 - 1 | Borrow Required |
| 10₂ - 1₂ | 1₂ |

---

# Memory Tricks

```text
Binary subtraction works exactly like decimal subtraction.
```

```text
Whenever 0 - 1 appears,
borrow from the next column.
```

```text
A borrowed 1 becomes 10₂.
```

```text
10₂ - 1₂ = 1₂
```

```text
Always verify answers
by converting binary numbers
to decimal.
```