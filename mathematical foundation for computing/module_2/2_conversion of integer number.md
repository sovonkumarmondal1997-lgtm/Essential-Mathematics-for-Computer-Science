# Number Systems and Data Representation

---

# Number Bases / Radices

## Definition

A **number base** (or radix) tells us how many unique digits are available in a number system.

For example:

```text
Base 10 → 10 digits
Base 2  → 2 digits
Base 8  → 8 digits
Base 16 → 16 digits
```

---

## Common Number Systems

| Number System | Base | Digits Used |
|--------------|------|-------------|
| Binary | 2 | 0, 1 |
| Octal | 8 | 0,1,2,3,4,5,6,7 |
| Decimal | 10 | 0,1,2,3,4,5,6,7,8,9 |
| Hexadecimal | 16 | 0-9, A-F |

---

## Example

The number:

```text
101
```

has different meanings in different bases.

### Binary

```text
101₂

= (1×4)+(0×2)+(1×1)

= 5₁₀
```

### Decimal

```text
101₁₀

= 101
```

### Octal

```text
101₈

= (1×64)+(0×8)+(1×1)

= 65₁₀
```

---

# Hexadecimal System (Base 16)

## Definition

The hexadecimal system uses:

```text
0 1 2 3 4 5 6 7 8 9 A B C D E F
```

where:

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

Convert:

```text
2F₁₆
```

to decimal.

Step 1:

```text
2 × 16¹ = 32
```

Step 2:

```text
F × 16⁰

15 × 1 = 15
```

Step 3:

```text
32 + 15 = 47
```

Answer:

```text
2F₁₆ = 47₁₀
```

---

# Binary System (Base 2)

## Definition

Binary uses only:

```text
0 and 1
```

Every digit position represents a power of 2.

---

## Example

```text
1011₂
```

Position Values:

```text
8 4 2 1
```

Calculation:

```text
(1×8)+(0×4)+(1×2)+(1×1)

= 11
```

Answer:

```text
1011₂ = 11₁₀
```

---

# Decimal System (Base 10)

## Definition

Decimal uses:

```text
0,1,2,3,4,5,6,7,8,9
```

Every position represents a power of 10.

---

## Example

```text
572
```

Calculation:

```text
(5×100)+(7×10)+(2×1)

= 500+70+2

= 572
```

---

# Octal System (Base 8)

## Definition

Octal uses:

```text
0,1,2,3,4,5,6,7
```

Every position represents a power of 8.

---

## Example

```text
25₈
```

Calculation:

```text
(2×8)+(5×1)

=16+5

=21₁₀
```

---

# Hexadecimal-to-Binary Conversion

## Definition

Convert each hexadecimal digit into its corresponding 4-bit binary value.

---

## Hexadecimal Reference Table

| Hex | Binary |
|------|--------|
| 0 | 0000 |
| 1 | 0001 |
| 2 | 0010 |
| 3 | 0011 |
| 4 | 0100 |
| 5 | 0101 |
| 6 | 0110 |
| 7 | 0111 |
| 8 | 1000 |
| 9 | 1001 |
| A | 1010 |
| B | 1011 |
| C | 1100 |
| D | 1101 |
| E | 1110 |
| F | 1111 |

---

## Example 1

Convert:

```text
A3₁₆
```

Replace each digit:

```text
A = 1010

3 = 0011
```

Combine:

```text
A3₁₆ = 10100011₂
```

---

## Example 2

Convert:

```text
2F₁₆
```

Replace:

```text
2 = 0010

F = 1111
```

Combine:

```text
2F₁₆ = 00101111₂
```

---

# Decimal-to-Binary Conversion

## Definition

Find the largest power of 2 that fits into the number and work downwards.

---

## Example 1

Convert:

```text
13₁₀
```

Powers of 2:

```text
16 8 4 2 1
```

13 contains:

```text
8 → Yes

Remaining = 5

4 → Yes

Remaining = 1

2 → No

1 → Yes
```

Result:

```text
1101₂
```

---

## Example 2

Convert:

```text
22₁₀
```

Powers:

```text
16 8 4 2 1
```

22 contains:

```text
16 → Yes

Remaining = 6

8 → No

4 → Yes

Remaining = 2

2 → Yes

Remaining = 0

1 → No
```

Result:

```text
10110₂
```

---

# Binary-to-Decimal Conversion

## Definition

Add together all positional values where the binary digit is 1.

---

## Example 1

Convert:

```text
1011₂
```

Position Values:

```text
8 4 2 1
```

Use positions with 1:

```text
8 + 2 + 1
```

Answer:

```text
11₁₀
```

---

## Example 2

Convert:

```text
11001₂
```

Position Values:

```text
16 8 4 2 1
```

Use positions with 1:

```text
16 + 8 + 1
```

Answer:

```text
25₁₀
```

---

# Binary-to-Hexadecimal Conversion

## Definition

Group binary digits into groups of 4 from right to left.

Convert each group to one hexadecimal digit.

---

## Example 1

Convert:

```text
10101111₂
```

Group:

```text
1010 1111
```

Convert:

```text
1010 = A

1111 = F
```

Answer:

```text
AF₁₆
```

---

## Example 2

Convert:

```text
00101101₂
```

Group:

```text
0010 1101
```

Convert:

```text
0010 = 2

1101 = D
```

Answer:

```text
2D₁₆
```

---

# Binary-to-Octal Conversion

## Definition

Group binary digits into groups of 3 from right to left.

Convert each group into one octal digit.

---

## Binary to Octal Table

| Binary | Octal |
|----------|---------|
| 000 | 0 |
| 001 | 1 |
| 010 | 2 |
| 011 | 3 |
| 100 | 4 |
| 101 | 5 |
| 110 | 6 |
| 111 | 7 |

---

## Example 1

Convert:

```text
101101₂
```

Group:

```text
101 101
```

Convert:

```text
101 = 5

101 = 5
```

Answer:

```text
55₈
```

---

## Example 2

Convert:

```text
110011₂
```

Group:

```text
110 011
```

Convert:

```text
110 = 6

011 = 3
```

Answer:

```text
63₈
```

---

# Positional Notation / Place Value

## Definition

The value of a digit depends on both:

```text
1. The digit itself
2. Its position
```

Each position represents a power of the base.

---

## Example 1 (Decimal)

```text
573
```

Positions:

```text
5 → Hundreds

7 → Tens

3 → Ones
```

Calculation:

```text
(5×100)+(7×10)+(3×1)

=573
```

---

## Example 2 (Binary)

```text
10101₂
```

Positions:

```text
16 8 4 2 1
```

Calculation:

```text
16+4+1

=21
```

---

# Data Representation in Computers

## Definition

Computers store and process all information using binary digits:

```text
0 and 1
```

Everything inside a computer eventually becomes binary.

---

# Example 1: Storing Numbers

Decimal:

```text
13
```

Stored as:

```text
1101₂
```

---

# Example 2: Storing Characters

Letter:

```text
A
```

ASCII Value:

```text
65
```

Binary:

```text
01000001
```

Computer stores:

```text
01000001
```

not the character directly.

---

# Example 3: Storing Colors

A web color:

```text
#FF0000
```

represents:

```text
Red = FF

Green = 00

Blue = 00
```

This is hexadecimal.

Equivalent binary:

```text
11111111 00000000 00000000
```

---

# Example 4: Memory Addresses

Computer memory often uses hexadecimal:

```text
0x1A2F
```

instead of long binary numbers like:

```text
0001101000101111
```

because hexadecimal is easier for humans to read.

---

# Why Binary and Hexadecimal Are Important

## Binary

Used by:

```text
CPU
RAM
Storage
Network Communication
Machine Instructions
```

---

## Hexadecimal

Used by:

```text
Memory Addresses
Color Codes
Debugging
Machine Code
Computer Architecture
```

because:

```text
1 Hex Digit = 4 Binary Bits
```

which makes binary much easier to read.

---

# Quick Revision Table

| System | Base | Digits |
|----------|---------|---------|
| Binary | 2 | 0,1 |
| Octal | 8 | 0-7 |
| Decimal | 10 | 0-9 |
| Hexadecimal | 16 | 0-9,A-F |

---

# Most Important Memory Tricks

```text
Binary → Groups of 1s and 0s
```

```text
1 Hex Digit = 4 Binary Bits
```

```text
1 Octal Digit = 3 Binary Bits
```

```text
Binary → Group by 4 → Hex
```

```text
Binary → Group by 3 → Octal
```

```text
Binary to Decimal → Add place values
```

```text
Decimal to Binary → Use powers of 2
```