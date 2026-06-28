# Propositional Equivalences and Logical Identities

## 1. Propositional Equivalences

Two logical formulas are **equivalent** if they always produce the same
truth value for every possible input.

**Symbol:** `≡`

### Examples

-   `P → Q ≡ ¬P ∨ Q`
-   `¬¬P ≡ P`

Think of it like mathematics: - `2 + 3 = 5` - In logic: `P → Q` and
`¬P ∨ Q` behave exactly the same.

------------------------------------------------------------------------

## 2. Equivalence Proof by Truth Table

Steps: 1. Build one truth table. 2. Evaluate both formulas. 3. Compare
the last columns. 4. If every value matches, the formulas are
equivalent.

Example:

  P   Q   P→Q   ¬P∨Q
  --- --- ----- ------
  T   T   T     T
  T   F   F     F
  F   T   T     T
  F   F   T     T

Since the last columns match, `P→Q ≡ ¬P∨Q`.

------------------------------------------------------------------------

## 3. Double Negation Law

**Formula**

`¬¬P ≡ P`

Negating twice returns the original statement.

Examples: - "It is not true that it is not raining." = "It is
raining." - `¬¬(5>2)` = `5>2`

------------------------------------------------------------------------

## 4. De Morgan's Laws

### Law 1

`¬(P ∧ Q) ≡ ¬P ∨ ¬Q`

Example: - NOT(Both doors are open) - At least one door is closed.

### Law 2

`¬(P ∨ Q) ≡ ¬P ∧ ¬Q`

Example: - NOT(Raining or Snowing) - Not raining AND not snowing.

------------------------------------------------------------------------

## 5. Implication as a Disjunction

`P → Q ≡ ¬P ∨ Q`

Example: "If I study, then I pass."

Equivalent: "Either I do not study OR I pass."

------------------------------------------------------------------------

## 6. Contrapositive

`P → Q ≡ ¬Q → ¬P`

Examples: - If it rains, roads are wet. - If roads are not wet, then it
did not rain.

Another: - If you graduate, you completed the course. - If you did not
complete the course, you did not graduate.

------------------------------------------------------------------------

## 7. Functional Completeness

All logical operators can be built from a small set of basic operators.

Example:

`P∨Q ≡ ¬(¬P∧¬Q)`

`P→Q ≡ ¬(P∧¬Q)`

Computers often reduce logic to NOT and AND.

------------------------------------------------------------------------

## 8. Expressing OR via AND

`P∨Q ≡ ¬(¬P∧¬Q)`

Example:

Tea OR Coffee

Equivalent:

NOT(No Tea AND No Coffee)

------------------------------------------------------------------------

## 9. Expressing Implication via AND

`P→Q ≡ ¬(P∧¬Q)`

Meaning: The only impossible case is:

P=True and Q=False.

Example:

If you study then pass

Equivalent:

NOT(Study AND Not Pass)

------------------------------------------------------------------------

## 10. Quantifier Negation Law

`¬∃x P(x) ≡ ∀x ¬P(x)`

Meaning:

"It is not true that there exists..."

becomes

"For every..."

Example:

"It is not true that some student failed."

Equivalent:

"Every student passed."

Also:

`¬∀x P(x) ≡ ∃x ¬P(x)`

Meaning: Not everyone satisfies the property.

------------------------------------------------------------------------

## 11. Quantified De Morgan Application

Example:

`¬∃x(P(x)∧Q(x))`

Step 1

`∀x ¬(P(x)∧Q(x))`

Step 2

`∀x(¬P(x)∨¬Q(x))`

Meaning:

No person has both properties.

Equivalent:

Everyone lacks at least one property.

------------------------------------------------------------------------

# Summary

  Law                   Formula
  --------------------- -------------------
  Double Negation       ¬¬P ≡ P
  De Morgan 1           ¬(P∧Q) ≡ ¬P∨¬Q
  De Morgan 2           ¬(P∨Q) ≡ ¬P∧¬Q
  Implication           P→Q ≡ ¬P∨Q
  Contrapositive        P→Q ≡ ¬Q→¬P
  OR via AND            P∨Q ≡ ¬(¬P∧¬Q)
  Implication via AND   P→Q ≡ ¬(P∧¬Q)
  Quantifier Negation   ¬∃xP(x) ≡ ∀x¬P(x)

------------------------------------------------------------------------

# Memory Tricks

-   Equivalent = Same truth table.
-   Double NOT cancels.
-   De Morgan swaps AND/OR and negates each part.
-   Implication = NOT premise OR conclusion.
-   Contrapositive = Reverse + Negate.
-   Quantifier negation swaps ∃ and ∀.
