# Combinatorics and Counting Techniques

## What is Combinatorics?

### Simple Definition

**Combinatorics** is the branch of mathematics that deals with **counting**, **arranging**, and **selecting** objects.

It helps answer questions like:

- How many different passwords can be created?
- How many ways can students sit in a row?
- How many different teams can be formed?
- How many possible lottery tickets exist?

Instead of listing every possibility one by one, combinatorics provides shortcuts and formulas to count efficiently.

---

## Why Do We Need Combinatorics?

Imagine you want to create a 6-digit PIN.

Possible PINs:

```text
000000
000001
000002
...
999999
```

There are 1,000,000 possibilities.

Listing all of them would take a long time.

Combinatorics lets us calculate the answer instantly.

---

# Product Rule of Counting
## (Fundamental Counting Principle)

### Simple Definition

If a task consists of multiple steps, and:

- Step 1 can be done in **m ways**
- Step 2 can be done in **n ways**

Then the entire task can be done in:

\[
m \times n
\]

ways.

In simple words:

> When choices happen one after another, multiply.

---

## Example 1: Choosing Clothes

Suppose you have:

- 3 shirts
- 4 pants

How many outfits can you make?

### Step 1

Choose a shirt:

```text
3 choices
```

### Step 2

Choose a pant:

```text
4 choices
```

Total:

\[
3 \times 4 = 12
\]

### Answer

```text
12 outfits
```

---

## Example 2: Ice Cream

Choose:

- 2 flavors
- 3 cone types

Total possibilities:

\[
2 \times 3 = 6
\]

### Answer

```text
6 possible ice creams
```

---

## Example 3: Coin and Die

You toss:

- 1 coin (2 outcomes)
- 1 die (6 outcomes)

Total outcomes:

\[
2 \times 6 = 12
\]

Examples:

```text
(H,1)
(H,2)
(H,3)
...
(T,6)
```

### Answer

```text
12 outcomes
```

---

## Example 4: Creating a Password

Password format:

```text
Letter + Digit
```

Choices:

- 26 letters
- 10 digits

Total passwords:

\[
26 \times 10 = 260
\]

### Answer

```text
260 passwords
```

---

# Why Multiplication Works

Imagine:

```text
Shirt A → 4 pants
Shirt B → 4 pants
Shirt C → 4 pants
```

Each shirt can pair with every pant.

Therefore:

```text
4 + 4 + 4 = 12
```

which is:

\[
3 \times 4 = 12
\]

---

# Generalized Product Rule

## Simple Definition

The Product Rule can be extended to any number of steps.

If:

- Task 1 has \(n_1\) choices
- Task 2 has \(n_2\) choices
- Task 3 has \(n_3\) choices
- ...
- Task k has \(n_k\) choices

Then total possibilities are:

\[
n_1 \times n_2 \times n_3 \times \cdots \times n_k
\]

---

## Easy Way to Remember

For multiple independent steps:

```text
Multiply all choices together
```

---

## Example 1: Meal Selection

Choose:

- 2 drinks
- 3 burgers
- 4 desserts

Total meals:

\[
2 \times 3 \times 4 = 24
\]

### Answer

```text
24 meal combinations
```

---

## Example 2: Student ID

Format:

```text
Letter + Letter + Digit + Digit
```

Choices:

```text
26 × 26 × 10 × 10
```

Calculation:

\[
26^2 \times 10^2
\]

\[
676 \times 100
\]

\[
67,600
\]

### Answer

```text
67,600 IDs
```

---

## Example 3: Car Number

Format:

```text
ABC-123
```

Choices:

```text
26 × 26 × 26 × 10 × 10 × 10
```

\[
26^3 \times 10^3
\]

\[
17,576,000
\]

### Answer

```text
17,576,000 possible numbers
```

---

# Permutations with Repetition
## (Counting Sequences)

### Simple Definition

A permutation with repetition means:

```text
Objects can be used again and again.
```

Each position can choose from the same set of options.

---

## Formula

If:

- n choices available
- r positions to fill

Then:

\[
n^r
\]

---

## Why?

Because every slot has n choices.

Using the Product Rule:

\[
n \times n \times n \times \cdots
\]

(r times)

which becomes:

\[
n^r
\]

---

# Example 1: Five-Letter Words

Suppose:

- 26 letters
- 5 positions

Letters may repeat.

Examples:

```text
APPLE
AAAAA
HELLO
ZZZZZ
```

Total possibilities:

\[
26^5
\]

Calculation:

\[
11,881,376
\]

### Answer

```text
11,881,376 possible words
```

---

# Example 2: Four-Digit PIN

Digits:

```text
0-9
```

Total choices:

```text
10 choices per position
```

Four positions:

\[
10^4
\]

\[
10,000
\]

Examples:

```text
0000
1234
9999
5555
```

### Answer

```text
10,000 PINs
```

---

# Example 3: Binary Strings

Binary digits:

```text
0,1
```

Length:

```text
8
```

Total possibilities:

\[
2^8
\]

\[
256
\]

### Answer

```text
256 binary strings
```

---

# Example 4: License Plate

Format:

```text
LLLDDD
```

Where:

```text
L = Letter
D = Digit
```

Total:

\[
26^3 \times 10^3
\]

\[
17,576,000
\]

### Answer

```text
17,576,000 plates
```

---

# Sum Rule of Counting

## Simple Definition

If a task can be done in:

- m ways OR
- n ways

and both choices cannot happen simultaneously,

then total ways are:

\[
m+n
\]

---

## Easy Way to Remember

### Product Rule

```text
AND → Multiply
```

### Sum Rule

```text
OR → Add
```

---

# Example 1: Choosing a Drink

Available:

```text
5 juices
OR
3 soft drinks
```

Total choices:

\[
5+3=8
\]

### Answer

```text
8 choices
```

---

# Example 2: Traveling

You can travel by:

```text
Bus (4 routes)
OR
Train (2 routes)
```

Total possibilities:

\[
4+2=6
\]

### Answer

```text
6 routes
```

---

# Example 3: Selecting a Student

Choose:

```text
A boy OR a girl
```

Suppose:

```text
12 boys
8 girls
```

Total:

\[
12+8=20
\]

### Answer

```text
20 students
```

---

# Example 4: Vowels or Digits

Choose one character.

Available:

```text
5 vowels
OR
10 digits
```

Total:

\[
5+10=15
\]

### Answer

```text
15 choices
```

---

# Product Rule vs Sum Rule

| Situation | Rule |
|------------|--------|
| Shirt AND Pant | Multiply |
| Letter AND Digit | Multiply |
| Coin AND Die | Multiply |
| Tea OR Coffee | Add |
| Bus OR Train | Add |
| Boy OR Girl | Add |

---

# Quick Summary

## Combinatorics

Study of counting, arranging, and selecting objects.

---

## Product Rule

If tasks happen one after another:

\[
m \times n
\]

Remember:

```text
AND = Multiply
```

---

## Generalized Product Rule

For multiple steps:

\[
n_1 \times n_2 \times n_3 \times \cdots \times n_k
\]

Remember:

```text
Multiply all independent choices
```

---

## Permutations with Repetition

When objects can be reused:

\[
n^r
\]

where:

- n = available choices
- r = positions

Examples:

```text
Passwords
PINs
Binary strings
License plates
```

---

## Sum Rule

If choices are mutually exclusive:

\[
m+n
\]

Remember:

```text
OR = Add
```

---

# Golden Rule for Counting Problems

Ask yourself:

### Are the choices connected by AND?

Example:

```text
Choose a shirt AND pant
Choose a letter AND digit
```

Use:

\[
\text{Multiply}
\]

---

### Are the choices connected by OR?

Example:

```text
Tea OR Coffee
Bus OR Train
```

Use:

\[
\text{Add}
\]

This simple idea solves a large percentage of beginner combinatorics problems.