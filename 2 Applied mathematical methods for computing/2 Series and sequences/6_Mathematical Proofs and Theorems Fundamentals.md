# Mathematical Proofs and Theorems Fundamentals

---

# 1. Proof

## Definition

A **Proof** is a logical argument that shows a mathematical statement is true.

Think of it as:

> "A step-by-step explanation that leaves no doubt."

A proof is built using:

- Variables
- Predicates
- Quantifiers
- Logical laws
- Rules of inference
- Previously proven results

---

## Real-Life Analogy

Imagine a detective solving a case.

Claim:

"The suspect committed the crime."

A detective cannot simply say:

"Trust me."

They must show evidence.

Similarly, mathematicians cannot simply say:

"This formula is true."

They must prove it.

---

## Example 1

Claim:

The sum of two even numbers is even.

Proof:

Let:

a = 2m

b = 2n

where m and n are integers.

Then:

a + b

= 2m + 2n

= 2(m+n)

Since (m+n) is an integer,

a+b is divisible by 2.

Therefore:

a+b is even.

Proved.

---

## Example 2

Claim:

5 + 7 = 12

Proof:

Using ordinary arithmetic:

5 + 7

= 12

Proved.

---

## Example 3

Claim:

All squares are non-negative.

Proof:

For any real number x:

x² = x × x

A number multiplied by itself cannot be negative.

Therefore:

x² ≥ 0

Proved.

---

## Why Proofs Matter

Without proofs:

Mathematics becomes guessing.

With proofs:

Mathematics becomes certainty.

---

# 2. Theorem

## Definition

A **Theorem** is a mathematical statement that has been proven true.

Think of it as:

> "A proven mathematical fact."

---

## Example 1

Theorem:

The sum of two even numbers is even.

Since it can be proven,

it is a theorem.

---

## Example 2

Theorem:

1 + 2 + 3 + ... + n

= n(n+1)/2

This can be proven by induction.

Therefore it is a theorem.

---

## Example 3

:contentReference[oaicite:0]{index=0} Theorem:

For a right triangle:

a² + b² = c²

This is a famous theorem.

---

## Real-Life Analogy

A theorem is like a court verdict.

After all evidence is presented,

the conclusion becomes accepted.

---

# 3. Axiom

## Definition

An **Axiom** is a statement accepted as true without proof.

It serves as a starting point.

Think of it as:

> "The foundation on which everything else is built."

---

## Example 1

Axiom:

If A = B and B = C

then A = C.

We simply accept this.

---

## Example 2

Axiom:

For any number a:

a = a

Everything equals itself.

---

## Example 3

In geometry:

Through any two distinct points,

exactly one straight line exists.

This is an axiom.

---

## House Analogy

Building a house:

Foundation → Axioms

Walls → Lemmas

Rooms → Theorems

Decorations → Corollaries

Without a foundation,

the house collapses.

---

# 4. Lemma

## Definition

A **Lemma** is a small proven result used to prove a larger theorem.

Think of it as:

> "A helper theorem."

---

## Example 1

Goal:

Prove a large theorem.

First prove:

Lemma:

Every even number can be written as 2k.

Then use that lemma later.

---

## Example 2

Before proving a theorem about triangles,

we may first prove:

Lemma:

The angles on a straight line add to 180°.

---

## Example 3

Before proving a complex algorithm,

we may prove:

Lemma:

The algorithm always terminates.

Then use it in the main proof.

---

## Construction Analogy

Building a bridge:

Small support beams = Lemmas

Entire bridge = Theorem

---

# 5. Corollary

## Definition

A **Corollary** is a result that follows almost immediately from a theorem.

Think of it as:

> "A free bonus result."

---

## Example 1

Theorem:

The sum of two even numbers is even.

Corollary:

The sum of four even numbers is even.

No major proof needed.

---

## Example 2

Theorem:

Every multiple of 4 is even.

Corollary:

100 is even.

Since:

100 = 4 × 25

---

## Example 3

Theorem:

All squares are non-negative.

Corollary:

25 is non-negative.

Since:

25 = 5²

---

## Tree Analogy

Theorem = Tree trunk

Corollaries = Branches

---

# 6. Formalization of a Theorem

## Definition

Formalization means translating ordinary language into mathematical logic.

---

## Example 1

English:

Every even number is divisible by 2.

Formal:

∀n ∈ ℤ

Even(n) → DivisibleBy2(n)

---

## Example 2

English:

If a number is divisible by 4,
then it is divisible by 2.

Formal:

∀n

(4 | n) → (2 | n)

---

## Example 3

English:

Every human is mortal.

Formal:

∀x

Human(x) → Mortal(x)

---

## Why Formalization Matters

Natural language can be ambiguous.

Formal logic removes ambiguity.

---

# 7. Direct Proof

## Definition

Direct proof proves:

p → q

by assuming p is true

and showing q must be true.

---

## Template

Assume p.

Use logic.

Reach q.

Done.

---

## Example 1

Prove:

If n is even,

then n² is even.

Assume:

n = 2k

Then:

n²

= (2k)²

= 4k²

= 2(2k²)

Therefore n² is even.

Proved.

---

## Example 2

Prove:

If a number is divisible by 10,

then it is divisible by 5.

Assume:

n = 10k

Then:

n = 5(2k)

Therefore divisible by 5.

---

## Example 3

Prove:

If n is divisible by 6,

then n is divisible by 3.

Assume:

n = 6k

= 3(2k)

Therefore divisible by 3.

---

# 8. Universal Generalization

## Definition

Universal Generalization says:

If a property is true for an arbitrary element,

then it is true for all elements.

---

## Example 1

Suppose:

x is any real number.

Show:

x + 0 = x

Since x was arbitrary,

we conclude:

∀x

x + 0 = x

---

## Example 2

Let n be any integer.

Show:

n² ≥ 0

Since n was arbitrary,

the statement holds for all integers.

---

## Example 3

Let x be any human.

Show:

x has a biological parent.

Therefore:

All humans have biological parents.

---

## Classroom Analogy

Check one arbitrary student.

If reasoning never depended on who the student was,

it works for every student.

---

# 9. Proof by Contraposition (Contrapositive)

## Definition

Instead of proving:

p → q

we prove:

¬q → ¬p

because the two statements are logically equivalent.

---

## Example 1

Statement:

If n² is even,

then n is even.

Direct proof is harder.

Use contrapositive.

Contrapositive:

If n is odd,

then n² is odd.

Assume:

n = 2k+1

Then:

n²

= (2k+1)²

= 4k²+4k+1

= 2(2k²+2k)+1

Odd.

Therefore contrapositive is true.

Hence original statement is true.

---

## Example 2

Statement:

If a number is divisible by 6,

then it is divisible by 3.

Contrapositive:

If not divisible by 3,

then not divisible by 6.

Easy to prove.

---

## Example 3

Statement:

If a student gets full marks,

then the student passed.

Contrapositive:

If the student failed,

then the student did not get full marks.

---

# 10. Proof by Contradiction

## Definition

To prove statement P:

1. Assume P is false.
2. Follow logic.
3. Reach an impossibility.
4. Therefore assumption was wrong.
5. P must be true.

---

## Example 1

Claim:

√2 is irrational.

Assume opposite:

√2 is rational.

Then:

√2 = a/b

where a and b have no common factors.

After algebra:

Both a and b become even.

This contradicts:

"No common factors."

Therefore assumption is false.

√2 is irrational.

Proved.

---

## Example 2

Claim:

There is no largest positive integer.

Assume:

There is a largest integer N.

Then:

N+1 is larger.

Contradiction.

Therefore no largest integer exists.

---

## Example 3

Claim:

A triangle cannot have four sides.

Assume it can.

Then a triangle would have both:

3 sides and 4 sides.

Impossible.

Contradiction.

---

# 11. Euclid's Theorem on the Infinitude of Primes

## Statement

There are infinitely many prime numbers.

Proven by

:contentReference[oaicite:1]{index=1}
over 2000 years ago.

---

## What Does It Mean?

Prime numbers never end.

Examples:

2, 3, 5, 7, 11, 13, 17, ...

There is always another prime.

---

## Proof by Contradiction

Assume opposite.

Suppose only finitely many primes exist.

List them:

p₁, p₂, p₃, ..., pₙ

---

### Construct a New Number

C = (p₁ × p₂ × ... × pₙ) + 1

---

### Example

Suppose all primes were:

2, 3, 5

Then:

C

= (2×3×5)+1

= 31

31 is prime.

But 31 was not in the list.

Contradiction.

---

### Another Example

Suppose primes were:

2,3,5,7

C

= (2×3×5×7)+1

= 211

211 is prime.

Again not in the list.

Contradiction.

---

### Why Contradiction Happens

When dividing C by any listed prime:

remainder = 1

So none of the listed primes can divide C.

Therefore:

Either

- C is prime

or

- C has a prime factor not in the list

Both contradict the claim that the list contained all primes.

---

## Conclusion

The assumption of finitely many primes is impossible.

Therefore:

There must be infinitely many prime numbers.

Proved.

---

# Quick Summary Table

| Concept | Simple Meaning |
|----------|---------------|
| Proof | Logical argument showing something is true |
| Theorem | Proven mathematical statement |
| Axiom | Accepted truth without proof |
| Lemma | Small helper theorem |
| Corollary | Immediate consequence of a theorem |
| Formalization | Converting English into mathematical logic |
| Direct Proof | Assume p and show q |
| Universal Generalization | True for arbitrary element ⇒ true for all |
| Contrapositive Proof | Prove ¬q ⇒ ¬p |
| Contradiction Proof | Assume opposite and reach impossibility |
| Euclid's Theorem | Prime numbers never end |

---

# Final Mental Model

Axioms
   ↓
Lemmas
   ↓
Theorems
   ↓
Corollaries

Proof Methods:

Direct Proof
      ↓
Contrapositive
      ↓
Contradiction
      ↓
Mathematical Truth

Goal:

Start with assumptions,
apply logic,
reach a conclusion,
and establish certainty.