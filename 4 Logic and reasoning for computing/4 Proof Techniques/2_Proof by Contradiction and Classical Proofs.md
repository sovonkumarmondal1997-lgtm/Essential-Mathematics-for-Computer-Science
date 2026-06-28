# Proof by Contradiction and Classical Proofs

# 1. Proof by Contradiction (Indirect Proof)

## What is Proof by Contradiction?

Proof by contradiction is a proof technique where we:

1.  Assume the statement we want to prove is **false**.
2.  Use logical reasoning based on that assumption.
3.  Reach an impossible situation (a contradiction).
4.  Conclude that our assumption must be wrong.
5.  Therefore, the original statement is true.

Think of it like solving a mystery:

Suppose your friend says, "The key is **not** in the drawer."

You search everywhere else and eventually discover that the only
possible place left is the drawer.

Your assumption was impossible, so the key must be in the drawer.

------------------------------------------------------------------------

## Example 1

Claim:

There is no largest positive integer.

Assume the opposite.

Suppose the largest positive integer is N.

Then N + 1 is also a positive integer.

But N + 1 \> N.

This contradicts the assumption that N was the largest.

Therefore,

There is no largest positive integer.

------------------------------------------------------------------------

## Example 2

Claim:

A person cannot be both completely asleep and completely awake at the
same time.

Assume someone is both asleep and awake.

This contradicts the definitions of asleep and awake.

Therefore, the assumption is impossible.

------------------------------------------------------------------------

# 2. Rational Number Framework

## What is a Rational Number?

A rational number is any number that can be written as

p/q

where:

-   p and q are integers.
-   q ≠ 0.
-   The fraction is in its simplest form (no common factors except 1).

Examples:

1/2

3/4

-7/5

10/1

All are rational.

Examples of numbers that are **not** rational:

√2

π

e

These cannot be written as a fraction of two integers.

------------------------------------------------------------------------

## Simplest Form

Example:

6/8

is not in simplest form.

Divide by 2:

6/8 = 3/4

Now it is irreducible.

This idea is essential for contradiction proofs involving rational
numbers.

------------------------------------------------------------------------

# 3. Irrationality of √2

## Claim

√2 is irrational.

## Step 1

Assume the opposite.

Suppose

√2 = p/q

where p/q is already in lowest terms.

------------------------------------------------------------------------

## Step 2

Square both sides.

2 = p²/q²

Multiply both sides by q².

p² = 2q²

So p² is even.

If p² is even,

then p is also even.

Write

p = 2k

------------------------------------------------------------------------

## Step 3

Substitute.

(2k)² = 2q²

4k² = 2q²

2k² = q²

So q² is even.

Therefore q is even.

------------------------------------------------------------------------

## Step 4

Now both

p

and

q

are even.

Both are divisible by 2.

But we assumed

p/q

was already in lowest terms.

Contradiction.

Therefore,

√2 cannot be rational.

It must be irrational.

------------------------------------------------------------------------

## Simple Intuition

We assumed the fraction was already fully simplified.

The mathematics forced both numbers to still be divisible by 2.

That is impossible.

So the original assumption was wrong.

------------------------------------------------------------------------

# 4. Infinitude of Prime Numbers

## Claim

There are infinitely many prime numbers.

## Step 1

Assume the opposite.

Suppose there are only finitely many primes.

List them:

2, 3, 5, 7, 11

Assume this is the complete list.

------------------------------------------------------------------------

## Step 2

Create a new number.

N = (2 × 3 × 5 × 7 × 11) + 1

N = 2311

------------------------------------------------------------------------

## Step 3

Try dividing N by every listed prime.

2311 ÷ 2

remainder 1

2311 ÷ 3

remainder 1

2311 ÷ 5

remainder 1

2311 ÷ 7

remainder 1

2311 ÷ 11

remainder 1

Every division leaves remainder 1.

Therefore,

N is not divisible by any prime in our list.

------------------------------------------------------------------------

## Step 4

Every integer greater than 1 is either:

-   Prime, or
-   Has a prime factor.

If N is prime,

our list was incomplete.

If N is composite,

its prime factor is missing from our list.

Either way,

our original list cannot contain every prime.

Contradiction.

Therefore,

there are infinitely many prime numbers.

------------------------------------------------------------------------

# Real-Life Applications

## Programming

Proofs help verify algorithms always work correctly.

## Cryptography

Prime numbers are the foundation of RSA encryption.

## Computer Science

Contradiction proofs verify correctness and impossibility results.

## Mathematics

Many famous theorems use contradiction as their main proof technique.

------------------------------------------------------------------------

# Summary Table

  -----------------------------------------------------------------------
  Concept                           Key Idea
  --------------------------------- -------------------------------------
  Proof by Contradiction            Assume false → derive contradiction →
                                    conclude true

  Rational Number                   p/q where p and q are integers, q ≠
                                    0, fraction in lowest terms

  √2 Irrationality                  Assuming √2 is rational forces
                                    numerator and denominator to both be
                                    even

  Infinite Primes                   Finite list + 1 construction always
                                    creates a new prime or new prime
                                    factor
  -----------------------------------------------------------------------

# Memory Tricks

-   Contradiction = "Assume the opposite."
-   Reach something impossible.
-   Therefore the assumption is false.
-   Rational = Fraction in simplest form.
-   √2 proof = Both numerator and denominator become even.
-   Infinite primes = Multiply all known primes and add 1.
