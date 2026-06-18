# Arithmetic and Geometric Series, and Mathematical Induction

---

# 1. Sum of an Arithmetic Progression Formula

## Definition

An **Arithmetic Progression (AP)** is a sequence where the difference between consecutive terms is always the same.

Example:

2, 5, 8, 11, 14, ...

The common difference is:

d = 3

The sum of the first n terms is:

Sₙ = n/2 × [2a + (n − 1)d]

where:

- Sₙ = sum of first n terms
- a = first term
- d = common difference
- n = number of terms

---

## Example 1

Find:

2 + 5 + 8 + 11 + 14

Here:

a = 2

d = 3

n = 5

Using formula:

S₅ = 5/2 × [2(2) + (5 − 1)(3)]

= 5/2 × [4 + 12]

= 5/2 × 16

= 40

Answer:

40

Verification:

2 + 5 + 8 + 11 + 14 = 40

---

## Example 2

Find:

10 + 20 + 30 + 40 + 50

a = 10

d = 10

n = 5

S₅ = 5/2 × [20 + 40]

= 5/2 × 60

= 150

Answer:

150

---

## Example 3

Find:

1 + 4 + 7 + ... + 28

a = 1

d = 3

Last term:

28

Find n:

28 = 1 + (n − 1)3

27 = 3(n − 1)

n = 10

Now:

S₁₀ = 10/2 × [2(1) + 9(3)]

= 5 × (2 + 27)

= 145

Answer:

145

---

## Real-Life Example

Suppose you save:

Week 1 = ₹100

Week 2 = ₹150

Week 3 = ₹200

Week 4 = ₹250

Week 5 = ₹300

AP:

100, 150, 200, 250, 300

Total savings:

S₅ = 1000

---

# 2. Proof by Mathematical Induction

## Definition

Mathematical induction is a technique used to prove that a statement is true for all natural numbers.

Think of a row of dominoes.

If:

1. The first domino falls.
2. Every domino knocks down the next one.

Then:

All dominoes fall.

---

## Three Steps

### Step 1

Base Case

Show formula works for n = 1.

### Step 2

Inductive Hypothesis

Assume formula works for n = k.

### Step 3

Inductive Step

Using the assumption, prove it works for n = k + 1.

---

## Example

Prove:

1 + 2 + ... + n = n(n+1)/2

for all n.

---

# 3. Base Case (Induction)

## Definition

The base case is the first domino.

We check whether the formula works for the smallest value.

Usually:

n = 1

---

## Example 1

Formula:

1 + 2 + ... + n = n(n+1)/2

Check n = 1

Left side:

1

Right side:

1(1+1)/2

= 1

Both sides equal.

Base case is true.

---

## Example 2

Formula:

1 + 3 + 5 + ... + (2n−1) = n²

Check n = 1

Left side:

1

Right side:

1² = 1

True.

---

## Example 3

Formula:

2ⁿ ≥ n+1

Check n = 1

Left side:

2¹ = 2

Right side:

1+1 = 2

True.

---

## Why Base Case Matters

Without proving the first case, induction cannot start.

No first domino.

No chain reaction.

---

# 4. Inductive Hypothesis

## Definition

In this step we temporarily assume the statement is true for some number k.

This assumption is called the inductive hypothesis.

We do NOT prove it.

We assume it.

---

## Example 1

Suppose:

1 + 2 + ... + n = n(n+1)/2

Assume true for n = k

Then:

1 + 2 + ... + k

= k(k+1)/2

This is the inductive hypothesis.

---

## Example 2

Assume:

1 + 3 + 5 + ... + (2k−1)

= k²

This becomes our hypothesis.

---

## Example 3

Assume:

2ᵏ ≥ k+1

This is our hypothesis.

---

## Why Do We Assume?

Because induction says:

"If it's true for one case, prove it's true for the next."

The assumption acts as a bridge.

---

# 5. Inductive Step

## Definition

Now we prove:

If formula works for k,

then it must work for k+1.

This is the heart of induction.

---

## Example

Prove:

1 + 2 + ... + n

= n(n+1)/2

---

### Hypothesis

Assume:

1 + 2 + ... + k

= k(k+1)/2

---

### Consider k+1

Left side becomes:

1 + 2 + ... + k + (k+1)

Using hypothesis:

= k(k+1)/2 + (k+1)

Factor:

= (k+1)[k/2 + 1]

= (k+1)(k+2)/2

This is exactly the formula with n = k+1.

Therefore true.

---

## Domino Interpretation

Base case:

Domino 1 falls.

Inductive step:

If domino k falls,
then domino k+1 falls.

Therefore all dominoes fall.

---

# 6. Sum of a Geometric Progression Formula

## Definition

A geometric progression (GP) is a sequence where each term is obtained by multiplying by the same number.

That number is called the common ratio.

Example:

2, 4, 8, 16, 32

Ratio:

r = 2

---

## Formula

Sₙ = a(1 − rⁿ)/(1 − r)

where:

- a = first term
- r = common ratio
- n = number of terms

---

## Example 1

Find:

1 + 2 + 4 + 8 + 16

a = 1

r = 2

n = 5

S₅ = 1(1−2⁵)/(1−2)

= (1−32)/(-1)

= 31

Answer:

31

Verification:

1+2+4+8+16=31

---

## Example 2

Find:

3 + 6 + 12 + 24

a = 3

r = 2

n = 4

S₄ = 3(1−2⁴)/(1−2)

= 3(-15)/(-1)

= 45

Answer:

45

---

## Example 3

Find:

5 + 10 + 20 + 40 + 80

a = 5

r = 2

n = 5

S₅ = 5(1−32)/(1−2)

= 155

Answer:

155

---

# 7. Proof by Multiplying and Subtracting

## Definition

This is the classic proof for geometric series.

The trick is:

1. Write the sum.
2. Multiply entire sum by r.
3. Subtract.
4. Almost all middle terms cancel.

---

## Example

Consider:

S = 1 + 2 + 4 + 8 + 16

Multiply by 2:

2S = 2 + 4 + 8 + 16 + 32

Subtract:

2S − S

= (2+4+8+16+32)

− (1+2+4+8+16)

Everything cancels except:

S = 32 − 1

S = 31

Answer:

31

---

## General Proof

Start:

Sₙ = a + ar + ar² + ... + arⁿ⁻¹

Multiply by r:

rSₙ = ar + ar² + ar³ + ... + arⁿ

Subtract:

Sₙ − rSₙ

= a − arⁿ

Factor:

Sₙ(1−r)

= a(1−rⁿ)

Divide:

Sₙ = a(1−rⁿ)/(1−r)

Proved.

---

# 8. Undefined / Boundary Case for Geometric Series (r = 1)

## Why It Is Special

Formula:

Sₙ = a(1−rⁿ)/(1−r)

contains:

1 − r

in the denominator.

If:

r = 1

then:

1 − r = 0

Division by zero is undefined.

Therefore the standard formula cannot be used.

---

## Example 1

Sequence:

5, 5, 5, 5, 5

r = 1

Sum:

5 + 5 + 5 + 5 + 5

= 25

Simply:

Sₙ = n × a

S₅ = 5 × 5

= 25

---

## Example 2

Sequence:

10, 10, 10, 10

r = 1

S₄ = 4 × 10

= 40

---

## Example 3

Sequence:

100, 100, 100, 100, 100, 100

S₆ = 6 × 100

= 600

---

## Why This Works

When r = 1

Every term is identical.

So:

a + a + a + ... + a

(n times)

equals:

n × a

---

# Quick Comparison Table

| Topic | Main Idea |
|---------|---------|
| Arithmetic Progression (AP) | Add a fixed difference each time |
| AP Sum Formula | Sₙ = n/2 × [2a + (n−1)d] |
| Mathematical Induction | Prove a statement for all natural numbers |
| Base Case | Verify first value |
| Inductive Hypothesis | Assume true for k |
| Inductive Step | Prove true for k+1 |
| Geometric Progression (GP) | Multiply by a fixed ratio |
| GP Sum Formula | Sₙ = a(1−rⁿ)/(1−r) |
| Multiply & Subtract Proof | Causes cancellation of middle terms |
| Special Case r=1 | Use Sₙ = n×a |

---

# Final Mental Model

Arithmetic Progression:

2, 5, 8, 11, 14

↓

Common Difference:

d = 3

↓

Sum Formula:

Sₙ = n/2 × [2a + (n−1)d]

---

Geometric Progression:

2, 4, 8, 16, 32

↓

Common Ratio:

r = 2

↓

Sum Formula:

Sₙ = a(1−rⁿ)/(1−r)

---

Mathematical Induction:

Base Case
    ↓
Inductive Hypothesis
    ↓
Inductive Step
    ↓
True for all natural numbers

Like a chain of dominoes:

First domino falls
+
Every domino knocks down the next
=
All dominoes fall.