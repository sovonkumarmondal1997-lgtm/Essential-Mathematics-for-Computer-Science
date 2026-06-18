# Solving Linear Homogeneous Recurrence Relations and Strong Induction

---

# 1. Solving Linear Homogeneous Recurrence Relations

## Definition

A **Linear Homogeneous Recurrence Relation** is a recurrence relation where:

- Each term depends on previous terms.
- No extra function like +5 or +n appears.
- The sequence is defined using linear combinations of earlier terms.

Example:

aₙ = 3aₙ₋₁ − 2aₙ₋₂

---

## Goal

We want to find a:

**Closed-Form Formula**

that allows us to compute a term directly.

Instead of:

a₁ → a₂ → a₃ → a₄ → ...

we want:

aₙ = formula

---

## Analogy

Imagine climbing stairs.

Recursive approach:

Step 1 → Step 2 → Step 3 → ...

Closed form:

Take an elevator directly to the floor.

---

## Example 1

Given:

aₙ = 2aₙ₋₁

a₀ = 1

Terms:

1, 2, 4, 8, 16, ...

Closed form:

aₙ = 2ⁿ

---

## Example 2

Given:

aₙ = 3aₙ₋₁

a₀ = 2

Terms:

2, 6, 18, 54, ...

Closed form:

aₙ = 2·3ⁿ

---

## Example 3

Fibonacci:

fₙ = fₙ₋₁ + fₙ₋₂

Finding the direct formula is more difficult.

We need:

- Geometric sequence ansatz
- Characteristic equation
- Initial conditions

---

# 2. Geometric Sequence Ansatz

## Definition

"Ansatz" means:

> An educated guess or trial solution.

For linear recurrences, we guess:

aₙ = rⁿ

where r is an unknown number.

---

## Why Guess This?

Because geometric sequences behave nicely when shifted.

Example:

aₙ = rⁿ

aₙ₋₁ = rⁿ⁻¹

aₙ₋₂ = rⁿ⁻²

All terms contain powers of r.

This makes algebra easier.

---

## Example 1

Recurrence:

aₙ = 2aₙ₋₁

Try:

aₙ = rⁿ

Substitute:

rⁿ = 2rⁿ⁻¹

Divide by rⁿ⁻¹

r = 2

Solution:

aₙ = 2ⁿ

---

## Example 2

Recurrence:

aₙ = 3aₙ₋₁

Substitute:

rⁿ = 3rⁿ⁻¹

r = 3

Solution:

aₙ = 3ⁿ

---

## Example 3

Recurrence:

aₙ = aₙ₋₁ + aₙ₋₂

Substitute:

rⁿ = rⁿ⁻¹ + rⁿ⁻²

This leads to a characteristic equation.

---

## Analogy

Like trying a key in a lock.

If it fits, the door opens.

The geometric sequence is the "trial key."

---

# 3. Characteristic Equation

## Definition

The **Characteristic Equation** is the polynomial obtained after substituting:

aₙ = rⁿ

into a recurrence relation.

Its roots determine the closed-form solution.

---

## General Form

Recurrence:

aₙ = c₁aₙ₋₁ + c₂aₙ₋₂ + ... + cₖaₙ₋ₖ

Characteristic equation:

rᵏ − c₁rᵏ⁻¹ − c₂rᵏ⁻² − ... − cₖ = 0

---

## Example 1

Recurrence:

aₙ = 2aₙ₋₁

Substitute:

rⁿ = 2rⁿ⁻¹

Characteristic equation:

r − 2 = 0

Root:

r = 2

---

## Example 2

Recurrence:

aₙ = 3aₙ₋₁ − 2aₙ₋₂

Characteristic equation:

r² − 3r + 2 = 0

Factor:

(r−1)(r−2)=0

Roots:

1 and 2

---

## Example 3

Fibonacci:

fₙ = fₙ₋₁ + fₙ₋₂

Characteristic equation:

r² − r − 1 = 0

---

## Why Important?

The roots tell us the shape of the final formula.

---

# 4. Root Multiplicity (p)

## Definition

Root multiplicity tells us:

> How many times the same root appears.

---

## Example 1

Equation:

(r−2)² = 0

Root:

2

appears twice.

Multiplicity = 2

---

## Example 2

Equation:

(r−3)³ = 0

Root:

3

appears three times.

Multiplicity = 3

---

## Example 3

Equation:

(r−5)(r−1)

Both roots appear once.

Multiplicity = 1

---

# Why Multiplicity Matters

Repeated roots require extra factors.

---

## Distinct Root Solution

Roots:

r₁, r₂

Solution:

aₙ = αr₁ⁿ + βr₂ⁿ

---

## Repeated Root Solution

Root:

r

Multiplicity = 2

Solution:

aₙ = (α + βn)rⁿ

---

## Triple Root

Multiplicity = 3

Solution:

aₙ = (α + βn + γn²)rⁿ

---

## Example

Characteristic equation:

(r−2)²=0

General solution:

aₙ=(α+βn)2ⁿ

---

# 5. Fibonacci Recurrence Relation Solution

## Recurrence

fₙ = fₙ₋₁ + fₙ₋₂

---

## Step 1

Assume:

fₙ = rⁿ

---

## Step 2

Substitute:

rⁿ = rⁿ⁻¹ + rⁿ⁻²

Divide by rⁿ⁻²

r² = r + 1

---

## Step 3

Characteristic Equation

r² − r − 1 = 0

---

## Step 4

Solve

Using quadratic formula:

r = (1 ± √5)/2

Roots:

φ = (1 + √5)/2

≈ 1.618

and

ψ = (1 − √5)/2

≈ −0.618

---

## Step 5

General Solution

fₙ = αφⁿ + βψⁿ

---

## Step 6

Use Initial Conditions

f₀ = 0

f₁ = 1

to find α and β.

Result:

fₙ = (φⁿ − ψⁿ)/√5

This is called:

**Binet's Formula**

---

## Example

f₅

= 5

f₆

= 8

f₇

= 13

---

# 6. Distinct Roots

## Definition

Distinct roots are roots that are different from one another.

---

## Example 1

r²−3r+2=0

Roots:

1 and 2

Distinct.

---

## Solution Form

aₙ

= α(1)ⁿ + β(2)ⁿ

---

## Example 2

r²−5r+6=0

Roots:

2 and 3

Distinct.

Solution:

aₙ = α2ⁿ + β3ⁿ

---

## Example 3

r²−7r+12=0

Roots:

3 and 4

Distinct.

Solution:

aₙ = α3ⁿ + β4ⁿ

---

## Rule

Distinct roots

→ separate exponential terms.

---

# 7. Initial Conditions

## Definition

Initial conditions are the starting values of the sequence.

They determine the constants:

α, β, γ, ...

---

## Why Needed?

The characteristic equation gives:

General solution.

Initial conditions give:

Exact solution.

---

## Example 1

aₙ = α2ⁿ

Given:

a₀ = 5

Then:

5 = α

Solution:

aₙ = 5·2ⁿ

---

## Example 2

aₙ = α2ⁿ + β3ⁿ

Given:

a₀ = 4

a₁ = 7

Solve:

α + β = 4

2α + 3β = 7

Find α and β.

---

## Example 3

Fibonacci

Given:

f₀=0

f₁=1

These determine α and β in Binet's Formula.

---

## Analogy

Characteristic equation gives:

Blueprint.

Initial conditions give:

Exact dimensions.

---

# 8. Strong Induction / Complete Induction

## Definition

Strong induction is a variation of ordinary induction.

Instead of assuming:

P(k)

we assume:

P(1), P(2), P(3), ..., P(k)

all hold.

Then prove:

P(k+1)

---

## Ordinary Induction

Assume:

P(k)

Prove:

P(k+1)

---

## Strong Induction

Assume:

P(1)

P(2)

P(3)

...

P(k)

all true.

Prove:

P(k+1)

---

## Why Needed?

Sometimes a statement depends on many earlier cases.

Not just the immediate previous case.

---

# Example 1: Every Integer >1 Has a Prime Factor

Claim:

Every integer n > 1

has a prime factor.

---

### Strong Induction Hypothesis

Assume every number:

2 through k

has a prime factor.

---

### Prove for k+1

Case 1:

k+1 is prime.

Done.

Case 2:

k+1 is composite.

Then:

k+1 = ab

where:

a,b < k+1

By hypothesis:

a has a prime factor.

Therefore:

k+1 has a prime factor.

Proved.

---

# Example 2: Climbing Stairs

Suppose:

You may climb:

1 step

or

2 steps

at a time.

To prove any stair can be reached,

you need information about several earlier stairs.

Strong induction works naturally.

---

# Example 3: Money Problem

Suppose:

You can make amounts using:

₹4 and ₹5 coins.

To prove large amounts are possible,

you often use strong induction.

---

# Strong Induction vs Ordinary Induction

| Ordinary Induction | Strong Induction |
|-------------------|------------------|
| Assume P(k) | Assume P(1)...P(k) |
| Use one previous case | Use all previous cases |
| Simpler | More powerful |
| Often sufficient | Needed for many recursive proofs |

---

# Quick Summary Table

| Concept | Simple Meaning |
|----------|---------------|
| Solving Linear Homogeneous Recurrences | Finding a direct formula for a recursive sequence |
| Geometric Sequence Ansatz | Guessing aₙ=rⁿ |
| Characteristic Equation | Polynomial equation whose roots determine the solution |
| Root Multiplicity | Number of times a root repeats |
| Distinct Roots | Different roots leading to separate exponential terms |
| Fibonacci Solution | Solving fₙ=fₙ₋₁+fₙ₋₂ using characteristic roots |
| Initial Conditions | Starting values used to determine constants |
| Strong Induction | Assume all previous cases are true |

---

# Final Mental Model

Recurrence Relation

aₙ = c₁aₙ₋₁ + c₂aₙ₋₂ + ...

↓

Guess

aₙ = rⁿ

↓

Characteristic Equation

rᵏ − c₁rᵏ⁻¹ − ...

↓

Find Roots

↓

Build General Solution

↓

Apply Initial Conditions

↓

Get Exact Closed Formula

Example:

Fibonacci

fₙ = fₙ₋₁ + fₙ₋₂

↓

r²−r−1=0

↓

Roots:

φ and ψ

↓

Binet's Formula

fₙ=(φⁿ−ψⁿ)/√5

Strong Induction:

Assume ALL previous cases
      ↓
Use them together
      ↓
Prove next case
      ↓
Statement true forever