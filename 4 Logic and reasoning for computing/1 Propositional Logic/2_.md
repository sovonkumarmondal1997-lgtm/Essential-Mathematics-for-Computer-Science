# Truth Tables and Logical Operators - Simple Notes

# 1. Truth Table

A truth table is a table that shows every possible combination of True
(T) and False (F) values for propositions and the result after applying
logical operators.

Think of it as a calculator for logic.

## Example 1

P = "It is raining."

  P
  ---
  T
  F

## Example 2

P = "It is raining."

Q = "I have an umbrella."

  P   Q   P AND Q
  --- --- ---------
  T   T   T
  T   F   F
  F   T   F
  F   F   F

------------------------------------------------------------------------

# 2. Truth Table Size Rule (2\^n)

If there are n different propositions, the truth table contains exactly
2\^n rows.

## Examples

1 proposition

2\^1 = 2 rows

  P
  ---
  T
  F

2 propositions

2\^2 = 4 rows

3 propositions

2\^3 = 8 rows

4 propositions

2\^4 = 16 rows

Quick Reference

  Number of propositions   Rows
  ------------------------ ------
  1                        2
  2                        4
  3                        8
  4                        16
  5                        32

------------------------------------------------------------------------

# 3. Operator Precedence

When parentheses are missing, solve operators in this order.

1.  NOT (¬)
2.  AND (∧)
3.  OR (∨)
4.  Implication (→)
5.  Bi-conditional (↔)

Example

¬P ∨ Q ∧ R

Step 1

¬P

Step 2

Q ∧ R

Step 3

¬P ∨ (Q ∧ R)

Example 2

P ∨ Q → R

Evaluate

P ∨ Q

Then

(P ∨ Q) → R

------------------------------------------------------------------------

# 4. Negation (NOT)

Symbol

¬P

Meaning

Reverse the truth value.

Simple Formula

¬P = 1 - P

Truth Table

  P   ¬P
  --- ----
  T   F
  F   T

Examples

P: Today is Sunday.

¬P: Today is not Sunday.

P: The light is ON.

¬P: The light is OFF.

------------------------------------------------------------------------

# 5. Conjunction (AND)

Symbol

P ∧ Q

Meaning

Both statements must be true.

Think like multiplication.

P × Q

Truth Table

  P   Q   P∧Q
  --- --- -----
  T   T   T
  T   F   F
  F   T   F
  F   F   F

Examples

You receive a certificate only if

-   Assignment submitted AND
-   Project submitted

Example 2

Laptop works only if

Battery charged AND Power button works

------------------------------------------------------------------------

# 6. Disjunction (OR)

Symbol

P ∨ Q

Meaning

At least one must be true.

Think like MAX(P,Q)

Truth Table

  P   Q   P∨Q
  --- --- -----
  T   T   T
  T   F   T
  F   T   T
  F   F   F

Examples

You can enter if

Student ID OR Faculty ID

Example 2

Weekend plan

Movie OR Shopping

Either is enough.

------------------------------------------------------------------------

# 7. Conditional (Implication)

Symbol

P → Q

Meaning

"If P happens, then Q must happen."

Promise interpretation

Only broken when

P = True

Q = False

Mathematical View

P ≤ Q

Truth Table

  P   Q   P→Q
  --- --- -----
  T   T   T
  T   F   F
  F   T   T
  F   F   T

Examples

If you study

then you pass.

Broken only when someone studies but does not pass.

Example 2

If alarm rings

then wake up.

Alarm rings but person does not wake up.

Promise broken.

------------------------------------------------------------------------

# 8. Bi-conditional (IFF)

Symbol

P ↔ Q

Meaning

Both statements must have identical truth values.

Think like equality.

P = Q

Truth Table

  P   Q   P↔Q
  --- --- -----
  T   T   T
  T   F   F
  F   T   F
  F   F   T

Examples

Door opens iff correct password entered.

Password correct → Door opens

Password incorrect → Door stays closed

Example 2

You graduate iff all degree requirements are completed.

------------------------------------------------------------------------

# 9. Exclusive OR (XOR)

Symbol

P ⊕

Meaning

Exactly one statement is true.

Opposite of Bi-conditional.

Truth Table

  P   Q   P⊕Q
  --- --- -----
  T   T   F
  T   F   T
  F   T   T
  F   F   F

Examples

Tea or Coffee

Exactly one.

Example 2

Winner or Loser

A person cannot be both simultaneously.

------------------------------------------------------------------------

# Comparison of Operators

  Operator         Symbol   True When
  ---------------- -------- ------------------------------
  NOT              ¬        Opposite of original
  AND              ∧        Both true
  OR               ∨        At least one true
  Implication      →        Everything except True→False
  Bi-conditional   ↔        Both have same truth value
  XOR              ⊕        Exactly one true

------------------------------------------------------------------------

# Memory Tricks

NOT → Opposite

AND → Both

OR → At least one

Implication → Promise

Bi-conditional → Equality

XOR → Only one

------------------------------------------------------------------------

These concepts are heavily used in Python if-statements, SQL WHERE
clauses, Boolean algebra, digital circuits, databases, machine learning
decision logic, and AI reasoning systems.
