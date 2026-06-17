# Function Properties: Injection, Surjection, Bijection and Related Concepts

---

# 1. Function Properties

## Definition

Function properties describe the behavior of a function and how elements of one set connect to elements of another set.

These properties help us answer questions like:

- Does every input have a unique output?
- Does every output get used?
- Can the function be reversed?

The three most important properties are:

1. Injective (One-to-One)
2. Surjective (Onto)
3. Bijective (Both Injective and Surjective)

---

## Visual Idea

Domain → Co-domain

Different properties describe how arrows connect between the two sets.

---

## Example

Domain:

A = {1,2,3}

Co-domain:

B = {a,b,c}

Mappings:

1 → a

2 → b

3 → c

This function is:

- Injective
- Surjective
- Bijective

---

# 2. Injection / Injective Function / One-to-One

## Definition

A function is injective if different inputs always produce different outputs.

In simple words:

No two inputs are allowed to share the same output.

---

## Mathematical Definition

If

a ≠ b

then

f(a) ≠ f(b)

---

## Example 1

f(x)=2x

Domain:

{1,2,3}

Outputs:

1 → 2

2 → 4

3 → 6

Every output is unique.

Therefore:

Injective

---

## Example 2

Student ID → Student Name

101 → Rahul

102 → Priya

103 → Amit

Each ID identifies exactly one student.

Injective.

---

## Not Injective Example

f(x)=x²

5 → 25

-5 → 25

Two inputs produce the same output.

Not injective.

---

# 3. Mathematical Proof of Injection via Contrapositive

## Definition

To prove a function is injective, assume:

f(a)=f(b)

Then prove:

a=b

---

## Example

Function:

f(x)=3x+2

Assume:

f(a)=f(b)

Substitute:

3a+2 = 3b+2

Subtract 2:

3a = 3b

Divide by 3:

a=b

Since equality of outputs forces equality of inputs:

Function is injective.

---

## Simple Meaning

Same output

↓

Same input

↓

Injective

---

# 4. Mathematical Proof of Injection via Direct Implication

## Definition

Show that:

a ≠ b

implies

f(a) ≠ f(b)

---

## Example

Function:

f(x)=5x

Suppose:

a ≠ b

Multiply both sides by 5:

5a ≠ 5b

Therefore:

f(a) ≠ f(b)

Hence:

Injective

---

## Simple Meaning

Different inputs

↓

Different outputs

↓

Injective

---

# 5. Counterexample Verification

## Definition

A mathematical statement is disproved by finding one example where it fails.

Only one failure is enough.

---

## Example 1

Claim:

f(x)=x² is injective.

Check:

f(5)=25

f(-5)=25

Different inputs

Same output

Claim is false.

---

## Example 2

Claim:

All birds can fly.

Counterexample:

Penguin

Claim disproved.

---

## Real-Life Example

Claim:

Every student scored above 80%.

Find one student who scored 75%.

Claim becomes false.

---

# 6. Domain Restriction

## Definition

Sometimes a function is not injective.

We can restrict the domain to make it injective.

---

## Example

Function:

f(x)=x²

Domain:

ℝ

Not injective because:

5²=(-5)²

---

## Restrict Domain

Use only positive numbers:

ℝ⁺

Domain:

{0,1,2,3,...}

Now:

No positive and negative pair exists.

Function becomes injective.

---

## Example

Original:

-3 → 9

3 → 9

Not injective.

Restricted Domain:

Only positive numbers.

3 → 9

No conflict.

Injective.

---

## Real-Life Example

Suppose two students have the same nickname.

Restricting to student IDs removes ambiguity.

---

# 7. Surjection / Surjective Function / Onto

## Definition

A function is surjective if every element in the co-domain receives at least one arrow.

Every output must be used.

---

## Mathematical Definition

Range = Co-domain

---

## Example

Domain:

{1,2,3}

Co-domain:

{a,b,c}

Mappings:

1 → a

2 → b

3 → c

All outputs are used.

Surjective.

---

## Example 2

f(x)=x

Domain:

ℝ

Co-domain:

ℝ

Every real number appears as an output.

Surjective.

---

## Not Surjective Example

Domain:

{1,2,3}

Co-domain:

{a,b,c,d}

Mappings:

1 → a

2 → b

3 → c

Output d is unused.

Not surjective.

---

# 8. Equivalence of Range and Co-domain

## Definition

A function is surjective when:

Range = Co-domain

---

## Example

Domain:

{1,2,3}

Co-domain:

{2,4,6}

Function:

f(x)=2x

Range:

{2,4,6}

Co-domain:

{2,4,6}

They are identical.

Surjective.

---

## Non-Surjective Example

Range:

{2,4}

Co-domain:

{2,4,6}

Range ≠ Co-domain

Not surjective.

---

# 9. Pre-image Existence Proof

## Definition

To prove surjection:

1. Let output be y.
2. Solve f(x)=y.
3. Show a valid x always exists.

---

## Example

Function:

f(x)=x+5

Let:

y=x+5

Solve:

x=y−5

For every y, a valid x exists.

Therefore:

Surjective.

---

## Example

f(x)=2x

Let:

y=2x

Solve:

x=y/2

Every y has a corresponding x.

Surjective.

---

## Simple Idea

Can we always find an input?

Yes → Surjective

No → Not Surjective

---

# 10. Surjection Disproof via Range Deficit

## Definition

A function is not surjective if some elements of the co-domain never appear.

---

## Example

f(x)=x²

Domain:

ℝ

Co-domain:

ℝ

Outputs:

0,1,4,9,...

Never:

-1,-2,-3,...

Negative numbers are missing.

Therefore:

Not surjective.

---

## Example

Co-domain:

{1,2,3,4}

Range:

{1,2,3}

4 is missing.

Not surjective.

---

## Simple Meaning

Unused output

↓

Not surjective

---

# 11. Bijective Combinations

## Definition

Functions can be classified into four categories.

---

## Case 1: Injective but Not Surjective

Domain:

{1,2,3}

Co-domain:

{a,b,c,d}

Mappings:

1 → a

2 → b

3 → c

Unique outputs.

Injective.

Output d unused.

Not surjective.

---

## Case 2: Surjective but Not Injective

Domain:

{1,2,3}

Co-domain:

{a,b}

Mappings:

1 → a

2 → a

3 → b

All outputs used.

Surjective.

Two inputs share output a.

Not injective.

---

## Case 3: Bijective

Domain:

{1,2,3}

Co-domain:

{a,b,c}

Mappings:

1 → a

2 → b

3 → c

Injective ✔

Surjective ✔

Bijective ✔

---

## Case 4: Neither

Domain:

{1,2,3,4}

Co-domain:

{a,b,c,d}

Mappings:

1 → a

2 → a

3 → b

4 → b

Not injective.

Not surjective.

Neither.

---

# 12. Function Validity Constraint

## Definition

A relation is NOT a function if one input has multiple outputs.

This is the most important function rule.

---

## Valid Function

1 → A

2 → B

3 → C

Every input has one output.

Valid function.

---

## Invalid Function

1 → A

1 → B

Input 1 points to two outputs.

Not a function.

---

## Example

Student Roll Number

101 → Rahul

Valid

---

## Invalid Example

101 → Rahul

101 → Priya

One roll number identifies two students.

Invalid.

---

# Complete Summary Table

| Property | Meaning |
|-----------|----------|
| Injective | Different inputs produce different outputs |
| Surjective | Every output is used |
| Bijective | Both injective and surjective |
| Counterexample | One failure disproves a claim |
| Domain Restriction | Reduce inputs to improve function properties |
| Range = Co-domain | Condition for surjection |
| Pre-image Proof | Solve f(x)=y |
| Range Deficit | Missing outputs prove non-surjection |
| Function Validity | One input cannot have multiple outputs |

---

# Visual Learning Flow

Set
↓
Relation
↓
Function
↓
Function Validity
↓
Injective (One-to-One)
↓
Injection Proofs
↓
Counterexamples
↓
Domain Restriction
↓
Surjective (Onto)
↓
Range = Co-domain
↓
Pre-image Proofs
↓
Surjection Disproof
↓
Bijective Functions
↓
Invertible Functions

Key Facts:

1. Every bijective function is injective and surjective.
2. Injective means no repeated outputs.
3. Surjective means no unused outputs.
4. Bijective means perfect matching between domain and co-domain.
5. A function becomes reversible only when it is bijective.

These concepts form the foundation of advanced mathematics, linear algebra, calculus, probability theory, machine learning, cryptography, databases, and computer science.