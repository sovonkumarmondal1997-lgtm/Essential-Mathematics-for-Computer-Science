# Principle of Mathematical Induction and Cardinality of Subsets

---

# 1. Principle of Mathematical Induction

## Definition

The **Principle of Mathematical Induction** is a proof technique used to show that a statement is true for:

- All positive integers
- All natural numbers
- All integers greater than some starting value

Instead of checking infinitely many cases one by one, induction proves all of them at once.

---

## Simple Idea

Suppose we want to prove:

P(1)
P(2)
P(3)
P(4)
...

Instead of checking every number forever:

We prove:

1. The first statement is true.
2. If one statement is true, then the next one is true.

Then all statements must be true.

---

## Real-Life Analogy

Imagine an infinite row of dominoes.

If:

- The first domino falls.
- Every domino knocks down the next domino.

Then:

All dominoes will eventually fall.

---

## Example 1

Claim:

1 + 2 + 3 + ... + n

= n(n+1)/2

for all positive integers n.

Using induction:

- Verify n = 1
- Show if true for k
- Then true for k+1

Therefore true for all n.

---

## Example 2

Claim:

2ⁿ ≥ n+1

for all positive integers n.

Again:

- Verify first case
- Show one case implies the next

Therefore true forever.

---

## Example 3

Claim:

1 + 3 + 5 + ... + (2n−1)

= n²

Induction proves this for every positive integer.

---

## Why Induction Is Powerful

Without induction:

Need infinitely many proofs.

With induction:

Need only two proofs.

---

# 2. Rule of Inference for Induction

## Formal Statement

If:

P(1)

is true

and

∀k (P(k) → P(k+1))

is true

then:

∀n P(n)

is true.

---

## Translation into Simple English

If:

1. The first case works.
2. Every case causes the next case to work.

Then:

All cases work.

---

## Structure

Step 1:

P(1)

True

Step 2:

P(1) → P(2)

P(2) → P(3)

P(3) → P(4)

...

Therefore:

P(n)

is true for all n.

---

## Example

Suppose:

P(n):

"The sum of first n numbers is n(n+1)/2"

If:

P(1) is true

and

P(k) implies P(k+1)

Then:

P(n) is true for every positive integer.

---

## Ladder Analogy

Imagine climbing a ladder.

You must show:

- You can stand on the first rung.
- From any rung, you can reach the next rung.

Then:

You can reach every rung.

---

# 3. Domino Effect Intuition

## Definition

The Domino Effect is the intuitive explanation of induction.

Think of an endless row of dominoes.

---

## Visual Representation

Domino 1
↓
Domino 2
↓
Domino 3
↓
Domino 4
↓
Domino 5
↓
...

---

## Two Requirements

### Requirement 1

First domino falls.

(Base Case)

### Requirement 2

Every domino knocks down the next.

(Inductive Step)

---

## Example 1

Suppose:

P(1) is true.

And:

P(k) → P(k+1)

Then:

P(2) becomes true.

Then:

P(3) becomes true.

Then:

P(4) becomes true.

Forever.

---

## Example 2

Think of chain reactions.

Match 1 lights Match 2.

Match 2 lights Match 3.

Match 3 lights Match 4.

Once the first match burns,

the entire chain burns.

---

## Example 3

Think of company promotions.

Employee 1 trains Employee 2.

Employee 2 trains Employee 3.

Employee 3 trains Employee 4.

If the first employee knows the process,

eventually everyone learns it.

---

## Why This Matters

The domino effect explains WHY induction works.

---

# 4. Base Case / Basic Step

## Definition

The Base Case is the first step in induction.

We verify that the statement works for the starting value.

Usually:

n = 1

but sometimes:

n = 0

or

n = 5

or another starting value.

---

## Purpose

Starts the domino chain.

Without it:

Nothing begins.

---

## Example 1

Claim:

1 + 2 + ... + n

= n(n+1)/2

Check:

n = 1

Left:

1

Right:

1(2)/2

= 1

True.

---

## Example 2

Claim:

2ⁿ ≥ n+1

Check:

n = 1

2¹ = 2

1+1 = 2

True.

---

## Example 3

Claim:

1 + 3 + 5 + ... + (2n−1)

= n²

Check:

n = 1

1 = 1²

True.

---

## Domino Interpretation

Base Case:

Push Domino #1.

---

# 5. Inductive Step

## Definition

The Inductive Step proves:

If the statement works for k,

then it must work for k+1.

---

## Purpose

Shows the chain reaction continues forever.

---

## General Structure

Assume:

P(k)

Show:

P(k+1)

---

## Example 1

Claim:

1 + 2 + ... + n

= n(n+1)/2

Assume:

1 + 2 + ... + k

= k(k+1)/2

Add:

(k+1)

to both sides.

After simplification:

(k+1)(k+2)/2

Therefore true for k+1.

---

## Example 2

Claim:

1 + 3 + 5 + ... + (2n−1)

= n²

Assume:

1 + 3 + 5 + ... + (2k−1)

= k²

Add next odd number:

2k+1

Then:

k² + (2k+1)

= (k+1)²

True.

---

## Example 3

Suppose:

A staircase can be climbed to step k.

Show:

Step k+1 can also be reached.

Then every step becomes reachable.

---

## Domino Interpretation

Domino k falls.

Therefore Domino k+1 falls.

---

# 6. Inductive Hypothesis

## Definition

The Inductive Hypothesis is the temporary assumption that:

P(k)

is true.

It is used only during the inductive step.

---

## Important Point

We do NOT prove P(k).

We assume it.

Then use it to prove P(k+1).

---

## Example 1

Claim:

1 + 2 + ... + n

= n(n+1)/2

Hypothesis:

1 + 2 + ... + k

= k(k+1)/2

---

## Example 2

Claim:

1 + 3 + 5 + ... + (2n−1)

= n²

Hypothesis:

1 + 3 + 5 + ... + (2k−1)

= k²

---

## Example 3

Claim:

2ⁿ ≥ n+1

Hypothesis:

2ᵏ ≥ k+1

Use this assumption to prove:

2ᵏ⁺¹ ≥ k+2

---

## Bridge Analogy

Think of the hypothesis as a bridge.

You stand on:

P(k)

and use it to reach:

P(k+1)

---

# Complete Induction Workflow

To prove P(n):

Step 1:

Base Case

Verify:

P(1)

Step 2:

Inductive Hypothesis

Assume:

P(k)

Step 3:

Inductive Step

Show:

P(k+1)

Conclusion:

P(n) is true for all positive integers.

---

# 7. Cardinality of Subsets

## Definition

Cardinality means:

"The number of elements in a set."

---

## Example 1

Set:

A = {1,2,3}

Cardinality:

|A| = 3

because there are three elements.

---

## Example 2

Set:

B = {a,b,c,d,e}

Cardinality:

|B| = 5

---

## Example 3

Empty Set:

∅

Cardinality:

|∅| = 0

---

# Cardinality of Subsets

A subset is a set formed from elements of another set.

---

## Example

Set:

A = {1,2}

Subsets:

∅

{1}

{2}

{1,2}

Total:

4 subsets

---

## Example

Set:

A = {a,b,c}

Subsets:

∅

{a}

{b}

{c}

{a,b}

{a,c}

{b,c}

{a,b,c}

Total:

8 subsets

---

# Pattern

| Number of Elements | Number of Subsets |
|-------------------|------------------|
| 1 | 2 |
| 2 | 4 |
| 3 | 8 |
| 4 | 16 |
| 5 | 32 |

Pattern:

2ⁿ

---

# Why Induction Is Used Here

We can prove:

A set with n elements has exactly:

2ⁿ subsets

using mathematical induction.

---

## Small Example

n = 1

Set:

{a}

Subsets:

∅

{a}

Total:

2 = 2¹

---

## Next Example

n = 2

Set:

{a,b}

Subsets:

∅

{a}

{b}

{a,b}

Total:

4 = 2²

---

## General Induction Idea

Assume:

A set with k elements has:

2ᵏ subsets.

Add one new element.

Every old subset now creates:

1. A version without the new element.
2. A version with the new element.

Therefore:

2 × 2ᵏ

= 2ᵏ⁺¹

Thus:

A set with k+1 elements has:

2ᵏ⁺¹ subsets.

Proved.

---

# Quick Summary Table

| Concept | Simple Meaning |
|----------|---------------|
| Principle of Induction | Technique for proving statements for all integers |
| Rule of Inference | First case true + each case implies next ⇒ all cases true |
| Domino Effect | First domino falls and knocks down all others |
| Base Case | Verify starting value |
| Inductive Hypothesis | Assume statement true for k |
| Inductive Step | Show k implies k+1 |
| Cardinality | Number of elements in a set |
| Cardinality of Subsets | Number of subsets of an n-element set is 2ⁿ |

---

# Final Mental Model

Mathematical Induction

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

Domino Version:

Push Domino #1
      ↓
Each Domino Pushes Next
      ↓
Infinite Chain Reaction

Set Theory Application:

n Elements
      ↓
2ⁿ Subsets
      ↓
Proven Using Induction