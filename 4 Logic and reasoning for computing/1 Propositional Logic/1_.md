# Propositional Logic -- Simple Notes

# 1. Propositional Logic

Propositional Logic is the branch of mathematics that studies statements
that are either **True (T)** or **False (F)**.

It helps computers, programmers, AI systems, databases, and digital
circuits make logical decisions.

## Examples

  Statement                           True/False
  ----------------------------------- ------------
  2 + 3 = 5                           True
  The Earth is flat.                  False
  Python is a programming language.   True

------------------------------------------------------------------------

# 2. Algebra of Propositions

Think of propositional logic as **Boolean Algebra for sentences**.

Just as numbers use +, --, ×, logical statements use logical operators.

Example:

P = "It is raining."

Q = "I have an umbrella."

Then:

-   P AND Q → It is raining **and** I have an umbrella.
-   P OR Q → Either it is raining or I have an umbrella.
-   NOT P → It is not raining.

------------------------------------------------------------------------

# 3. Proposition (Statement)

A proposition is a sentence that has **exactly one truth value**.

## Examples

✔ 5 \> 2 (True)

✔ Delhi is in India. (True)

✔ 10 is an odd number. (False)

Not allowed:

-   Both true and false
-   Neither true nor false

------------------------------------------------------------------------

# 4. Non-Propositions

These cannot be assigned one definite truth value.

## Questions

-   What is your name?
-   Are you hungry?

## Commands

-   Close the door.
-   Study Python.

## Variable statements

-   x \> 5
-   y + 2 = 10

Without knowing x or y, we cannot say True or False.

------------------------------------------------------------------------

# 5. Specific Statements

Specific statements have known truth values.

Traditionally written using capital letters.

P = "Python is easy."

Q = "5 is even."

R = "India is in Asia."

Example:

P = True

Q = False

R = True

------------------------------------------------------------------------

# 6. General Statements (Propositional Variables)

Lowercase letters represent any proposition.

Example:

p = any statement

q = another statement

Example proof:

If p is true and p → q,

then q must be true.

------------------------------------------------------------------------

# 7. Atomic and Compound Propositions

## Atomic

Cannot be broken into smaller logical statements.

Examples

-   It is raining.
-   I am hungry.
-   Today is Monday.

## Compound

Made by joining atomic propositions.

Examples

P: It is raining.

Q: I have an umbrella.

P AND Q

P OR Q

NOT P

P → Q

------------------------------------------------------------------------

# 8. Logical NOT (Negation)

Symbol:

¬P

Meaning:

Reverse the truth value.

Examples

P: The light is ON.

¬P: The light is NOT ON.

Truth Table

  P   ¬P
  --- ----
  T   F
  F   T

------------------------------------------------------------------------

# 9. Logical OR (Disjunction)

Symbol:

P ∨ Q

Meaning:

At least one statement is true.

Truth Table

  P   Q   P∨Q
  --- --- -----
  T   T   T
  T   F   T
  F   T   T
  F   F   F

Example

You pass if

-   assignment is submitted OR
-   project is submitted.

Submitting either one is enough.

------------------------------------------------------------------------

# 10. Logical AND (Conjunction)

Symbol

P ∧ Q

Meaning

Both must be true.

Truth Table

  P   Q   P∧Q
  --- --- -----
  T   T   T
  T   F   F
  F   T   F
  F   F   F

Example

To enter a lab you need

-   ID card AND
-   Lab permission.

Missing one means no entry.

------------------------------------------------------------------------

# 11. Conditional (If-Then)

Symbol

P → Q

Meaning

If P happens, then Q should happen.

It is false only when P is true but Q is false.

Truth Table

  P   Q   P→Q
  --- --- -----
  T   T   T
  T   F   F
  F   T   T
  F   F   T

Example

If you study, then you pass.

Only fails when someone studies but still does not pass.

------------------------------------------------------------------------

# 12. Bi-conditional (If and Only If)

Symbol

P ↔ Q

Meaning

Both statements must have the same truth value.

Truth Table

  P   Q   P↔Q
  --- --- -----
  T   T   T
  T   F   F
  F   T   F
  F   F   T

Example

You can vote iff you are an eligible voter.

Both conditions must match.

------------------------------------------------------------------------

# 13. Exclusive OR (XOR)

Symbol

P ⊕

Meaning

Exactly one statement is true.

Truth Table

  P   Q   P⊕Q
  --- --- -----
  T   T   F
  T   F   T
  F   T   T
  F   F   F

Examples

Choose Tea OR Coffee (not both).

Switch control: - Switch A ON and B OFF → Light ON - Switch A OFF and B
ON → Light ON - Both ON or both OFF → Light OFF

------------------------------------------------------------------------

# Quick Summary

  Operator         Symbol   Meaning
  ---------------- -------- ------------------------------
  NOT              ¬        Opposite truth value
  AND              ∧        Both true
  OR               ∨        At least one true
  IF-THEN          →        False only when True → False
  IF AND ONLY IF   ↔        Same truth values
  XOR              ⊕        Exactly one true

These concepts form the foundation of programming conditions, Boolean
algebra, SQL WHERE clauses, digital logic, AI reasoning, databases, and
mathematical proofs.
