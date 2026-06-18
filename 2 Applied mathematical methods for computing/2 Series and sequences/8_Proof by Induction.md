# Proof by Induction: Complete Beginner Guide

---

# 1. Proof by Induction

## Definition

**Proof by Induction** is a mathematical technique used to prove that a statement, formula, or property is true for **all positive integers**.

Instead of checking:

P(1)
P(2)
P(3)
P(4)
...

one by one forever,

we prove only two things:

1. The first case is true.
2. If one case is true, the next case must also be true.

Then the statement is true for all positive integers.

---

## Domino Analogy

Imagine an infinite row of dominoes.

If:

- The first domino falls.
- Every domino knocks down the next domino.

Then:

All dominoes fall.

This is exactly how induction works.

---

## General Structure

### Step 1

Basis Step (Base Case)

Show:

P(1)

is true.

---

### Step 2

Inductive Hypothesis

Assume:

P(k)

is true.

---

### Step 3

Inductive Step

Show:

P(k+1)

is true.

---

### Conclusion

P(n)

is true for all positive integers.

---

## Example

Claim:

1 + 2 + 3 + ... + n

= n(n+1)/2

for all positive integers.

This can be proven by induction.

---

# 2. Sum of Arithmetic Series (Formula Proof via Induction)

## Statement

Prove:

Σ(i=1 to n) i

= n(n+1)/2

---

## Step 1: Base Case

Let:

n = 1

Left side:

1

Right side:

1(1+1)/2

= 1

Both sides equal.

True.

---

## Step 2: Inductive Hypothesis

Assume:

1 + 2 + ... + k

= k(k+1)/2

This is our assumption.

---

## Step 3: Inductive Step

Need to show:

1 + 2 + ... + k + (k+1)

= (k+1)(k+2)/2

Start from the left side:

= k(k+1)/2 + (k+1)

Factor:

= (k+1)[k/2 + 1]

= (k+1)(k+2)/2

which equals the right side.

Therefore true for k+1.

---

## Conclusion

The formula is true for all positive integers.

---

## Example Verification

n = 5

Left side:

1+2+3+4+5

= 15

Formula:

5(6)/2

= 15

Correct.

---

# 3. Basis Step / Base Case

## Definition

The **Base Case** is the first step of induction.

It verifies that the statement works for the starting value.

Usually:

n = 1

Sometimes:

n = 0

or

n = 5

or another starting point.

---

## Why It Matters

Without the first domino falling,

nothing starts.

---

## Example 1

Claim:

n² ≥ n

Check:

n=1

1² = 1

True.

---

## Example 2

Claim:

2ⁿ ≥ n+1

Check:

n=1

2¹ = 2

1+1 = 2

True.

---

## Example 3

Claim:

1+3+5+...+(2n−1)=n²

Check:

n=1

1 = 1²

True.

---

## Counterexample

Claim:

n² > n

Check:

n=1

1 > 1

False.

Base case fails.

Induction cannot start.

---

# 4. Inductive Step

## Definition

The **Inductive Step** proves:

If the statement works for k,

then it must work for k+1.

---

## Purpose

Keeps the chain reaction moving forever.

---

## Template

Assume:

P(k)

Show:

P(k+1)

---

## Example 1

Claim:

1+2+...+n

= n(n+1)/2

Assume true for k.

Add:

k+1

to both sides.

Simplify.

Result becomes:

(k+1)(k+2)/2

Thus true for k+1.

---

## Example 2

Claim:

1+3+5+...+(2n−1)

= n²

Assume:

k²

Add next odd number:

2k+1

Then:

k²+(2k+1)

= (k+1)²

True.

---

## Example 3

Suppose:

You can climb stair k.

Show:

You can also climb stair k+1.

Then all stairs become reachable.

---

# 5. Inductive Hypothesis

## Definition

The **Inductive Hypothesis** is the temporary assumption that:

P(k)

is true.

It acts as a tool for proving:

P(k+1)

---

## Important Rule

You do NOT prove P(k).

You assume it.

---

## Example 1

Assume:

1+2+...+k

= k(k+1)/2

Use this to prove:

P(k+1)

---

## Example 2

Assume:

1+3+5+...+(2k−1)

= k²

Use it to prove:

(k+1)²

---

## Example 3

Assume:

2ᵏ ≥ k+1

Use this assumption to prove:

2ᵏ⁺¹ ≥ k+2

---

## Bridge Analogy

Inductive Hypothesis

acts like a bridge

between

P(k)

and

P(k+1).

---

# 6. Inequality Proof via Induction

## Definition

Induction can prove inequalities.

Not just equations.

---

## Example

Prove:

3ⁿ < n!

for all

n ≥ 7

---

# Understanding Factorials First

7!

= 7×6×5×4×3×2×1

= 5040

3⁷

= 2187

Therefore:

2187 < 5040

Base case works.

---

## Base Case

n=7

3⁷ = 2187

7! = 5040

2187 < 5040

True.

---

## Inductive Hypothesis

Assume:

3ᵏ < k!

for some

k ≥ 7

---

## Inductive Step

Need to prove:

3ᵏ⁺¹ < (k+1)!

Start:

3ᵏ⁺¹

= 3·3ᵏ

Using hypothesis:

< 3·k!

Since:

k ≥ 7

Therefore:

k+1 ≥ 8

and:

3 < k+1

Thus:

3·k! < (k+1)k!

= (k+1)!

Hence:

3ᵏ⁺¹ < (k+1)!

True.

---

## Conclusion

3ⁿ < n!

for all

n ≥ 7

---

# 7. Factorial (n!)

## Definition

Factorial means:

Multiply all positive integers up to n.

Notation:

n!

---

## Formula

n!

= n(n−1)(n−2)...3·2·1

---

## Examples

### Example 1

3!

= 3×2×1

= 6

---

### Example 2

5!

= 5×4×3×2×1

= 120

---

### Example 3

7!

= 5040

---

## Special Case

0!

= 1

By definition.

---

## Why Factorials Matter

Used in:

- Permutations
- Combinations
- Probability
- Algorithms
- Induction proofs

---

# 8. Divisibility Proof via Induction

## Definition

Induction can prove that expressions are always divisible by a number.

---

## Example

Prove:

6ⁿ + 4

is divisible by 5.

---

## Base Case

n=1

6¹ + 4

= 10

Divisible by 5.

True.

---

## Inductive Hypothesis

Assume:

6ᵏ + 4

is divisible by 5.

Meaning:

6ᵏ + 4 = 5m

for some integer m.

---

## Inductive Step

Need:

6ᵏ⁺¹ + 4

Start:

= 6(6ᵏ)+4

Add and subtract 24:

= 6(6ᵏ+4)-20

Using hypothesis:

= 6(5m)-20

= 30m-20

= 5(6m-4)

Multiple of 5.

Therefore true.

---

## Conclusion

6ⁿ + 4

is divisible by 5

for all positive integers n.

---

# 9. Incorrect Induction / Fallacious Proof

## Definition

A **Fallacious Induction Proof** is an induction argument that looks correct but contains a hidden mistake.

---

## Common Mistake

Skipping the base case.

---

## Example

Suppose someone claims:

Every positive integer is negative.

---

### Fake Inductive Step

Assume:

k is negative.

Then claim:

k+1 is negative.

The algebra may look convincing.

---

### Problem

Base case:

1 is negative

is false.

Therefore the proof collapses.

---

## Example 2

Claim:

All cats have the same color.

A famous fake induction proof exists.

The error occurs when moving from:

1 animal

to

2 animals.

The overlap assumption fails.

---

## Lesson

Even perfect algebra cannot save a proof if the induction setup is wrong.

---

# 10. Logical Implication of False Assumptions

## Definition

In logic:

Starting from a false premise can lead to false conclusions.

---

## Simple Idea

If your starting point is wrong,

everything built on it becomes unreliable.

---

## Example 1

Premise:

"All birds are elephants."

False.

Then:

A sparrow is a bird.

Therefore:

A sparrow is an elephant.

The conclusion is nonsense because the premise was false.

---

## Example 2

Assume:

2 = 3

Multiply:

2×5 = 3×5

10 = 15

False conclusion caused by false assumption.

---

## Example 3

Suppose a programmer writes:

Assume every input is positive.

If a negative value arrives,

the program may crash.

Wrong assumption → wrong result.

---

## Relation to Induction

If:

- Base case is false
- Hypothesis is invalid
- Inductive step is broken

then the final conclusion cannot be trusted.

---

# Complete Induction Workflow

Step 1

Base Case

Verify first value.

↓

Step 2

Inductive Hypothesis

Assume true for k.

↓

Step 3

Inductive Step

Prove true for k+1.

↓

Conclusion

True for all integers in the domain.

---

# Quick Summary Table

| Concept | Simple Meaning |
|----------|---------------|
| Proof by Induction | Prove a statement for all integers |
| Base Case | Verify first value |
| Inductive Hypothesis | Assume true for k |
| Inductive Step | Show k implies k+1 |
| Arithmetic Sum Proof | Proves 1+2+...+n=n(n+1)/2 |
| Inequality Induction | Proves inequalities like 3ⁿ<n! |
| Factorial | Product of all positive integers up to n |
| Divisibility Induction | Shows expressions are always divisible by a number |
| Incorrect Induction | Looks valid but contains a flaw |
| False Assumptions | Wrong premises can produce wrong conclusions |

---

# Final Mental Model

Proof by Induction

Base Case
      ↓
Inductive Hypothesis
      ↓
Inductive Step
      ↓
P(1)
      ↓
P(2)
      ↓
P(3)
      ↓
P(4)
      ↓
...
      ↓
All Positive Integers

Think:

Push First Domino
      ↓
Each Domino Pushes Next
      ↓
Infinite Chain Reaction
      ↓
Statement Proven Forever