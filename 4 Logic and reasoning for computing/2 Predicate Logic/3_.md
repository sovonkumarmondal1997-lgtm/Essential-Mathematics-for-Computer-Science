# Quantifier Negation - Beginner Friendly Notes

# 1. Quantifier Negation Intuition

Quantifier negation tells us how to correctly negate statements
involving **all** or **there exists**.

A simple way to remember it is:

-   To prove **"All" is false**, you only need **one exception**.
-   To prove **"There exists" is false**, you must show **every object
    fails**.

Think about these English sentences.

## Example 1

Statement:

All students passed.

To prove this is false, you only need one student who failed.

Example:

Alice passed.

Bob passed.

Charlie failed.

Since Charlie failed, "All students passed" is false.

------------------------------------------------------------------------

## Example 2

Statement:

There exists a flying elephant.

To prove this is false, you must show that **every elephant cannot
fly**.

One elephant not flying is not enough.

Every elephant must fail the property.

------------------------------------------------------------------------

## Example 3

Statement:

Every number is even.

Finding one odd number (3) disproves the statement.

------------------------------------------------------------------------

## Example 4

Statement:

There exists a prime number greater than 100.

Finding one such number (101) proves it.

To disprove it, you would have to show **every number greater than 100
is not prime**, which is false.

------------------------------------------------------------------------

# 2. De Morgan's Laws for Quantifiers

These laws are the predicate logic version of De Morgan's Laws.

Whenever a NOT passes through a quantifier:

-   The quantifier changes.
-   The predicate is negated.

Think of it as:

NOT changes

∀ ↔ ∃

AND

Predicate becomes NOT Predicate.

## Rules

¬∀x P(x)

≡

∃x ¬P(x)

and

¬∃x P(x)

≡

∀x ¬P(x)

------------------------------------------------------------------------

# 3. Negating a Universal Quantifier

## Rule

¬∀x P(x)

≡

∃x ¬P(x)

Meaning

"It is NOT true that everyone satisfies P"

becomes

"There exists someone who does NOT satisfy P."

------------------------------------------------------------------------

### Example 1

Original

All students passed.

Logic

∀x Passed(x)

Negation

∃x ¬Passed(x)

Meaning

At least one student failed.

------------------------------------------------------------------------

### Example 2

Original

Every bird flies.

Negation

Some bird does not fly.

Penguins provide the counterexample.

------------------------------------------------------------------------

### Example 3

Original

Every number is positive.

Negation

There exists a number that is not positive.

Example:

0

or

-3

------------------------------------------------------------------------

# 4. Negating an Existential Quantifier

## Rule

¬∃x P(x)

≡

∀x ¬P(x)

Meaning

"It is NOT true that someone satisfies P"

becomes

"Everyone fails P."

------------------------------------------------------------------------

### Example 1

Original

Some student failed.

Logic

∃x Failed(x)

Negation

∀x ¬Failed(x)

Meaning

Every student passed.

------------------------------------------------------------------------

### Example 2

Original

There exists a blue apple.

Negation

Every apple is not blue.

------------------------------------------------------------------------

### Example 3

Original

There exists an odd even number.

Negation

Every even number is not odd.

------------------------------------------------------------------------

# 5. Nested Quantifier Negation

Sometimes more than one quantifier appears.

Negate them one at a time from left to right.

Each time:

-   Flip ∀ to ∃.
-   Flip ∃ to ∀.
-   Push the NOT inward.

Finally, negate the predicate.

------------------------------------------------------------------------

## Example 1

Original

¬∀x ∃y Loves(x,y)

Step 1

Change

∀

to

∃

↓

∃x ¬∃y Loves(x,y)

Step 2

Change

∃

to

∀

↓

∃x ∀y ¬Loves(x,y)

Meaning

There exists a person who loves nobody.

------------------------------------------------------------------------

## Example 2

Original

¬∃x ∀y Friend(x,y)

Step 1

↓

∀x ¬∀y Friend(x,y)

Step 2

↓

∀x ∃y ¬Friend(x,y)

Meaning

Every person has someone who is not their friend.

------------------------------------------------------------------------

## Example 3

Original

¬∀x ∀y Greater(x,y)

Step 1

↓

∃x ¬∀y Greater(x,y)

Step 2

↓

∃x ∃y ¬Greater(x,y)

Meaning

There exists at least one pair where the first is not greater than the
second.

------------------------------------------------------------------------

# Summary Table

  Original Statement    Negation
  --------------------- ----------------------
  ∀x P(x)               ∃x ¬P(x)
  ∃x P(x)               ∀x ¬P(x)
  All students passed   Some student failed
  Some student passed   Every student failed

------------------------------------------------------------------------

# Memory Tricks

-   "All" is broken by **one exception**.
-   "There exists" is broken only when **everything fails**.
-   Every NOT crossing a quantifier flips:
    -   ∀ ↔ ∃
-   After flipping the quantifier, negate the predicate.
-   For nested quantifiers, work **left to right**, flipping one
    quantifier at a time until the NOT reaches the predicate.

These rules are fundamental in mathematical proofs, predicate logic,
database query reasoning, artificial intelligence, theorem proving, and
formal verification.
