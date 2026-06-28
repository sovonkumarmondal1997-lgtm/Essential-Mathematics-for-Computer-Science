# Logical Formula Simplification and Evaluation - Simple Notes

# 1. Tautology

A tautology is a logical statement that is **always True**, no matter
what values the variables have.

## Example

P ∨ ¬P

If P=True → True∨False=True

If P=False → False∨True=True

Always True.

Another Example

If today rains OR today does not rain.

One of them must always be true.

------------------------------------------------------------------------

# 2. Consistent Formula

A consistent formula is true in **at least one** situation.

It does not have to be true all the time.

Example

P ∧ Q

  P   Q   Result
  --- --- --------
  T   T   T
  T   F   F
  F   T   F
  F   F   F

Since one row is True, it is consistent.

Another Example

P

If P=True, then the formula is True.

------------------------------------------------------------------------

# 3. Inconsistent Formula (Contradiction)

A contradiction is always False.

Example

P ∧ ¬P

If P=True

True AND False=False

If P=False

False AND True=False

Always False.

Real-life example

"It is raining and it is not raining."

Impossible.

------------------------------------------------------------------------

# 4. Tautology Substitution

Whenever you see an always-true expression, replace it with True.

Known tautology

P ∨ ¬P = True

Example

(P ∨ ¬P) ∧ Q

↓

True ∧ Q

↓

Q

Another Example

(P ∨ ¬P) ∨ R

↓

True ∨ R

↓

True

------------------------------------------------------------------------

# 5. Contradiction Substitution

Replace known contradictions with False.

Known contradiction

P ∧ ¬P = False

Example

(P ∧ ¬P) ∨ Q

↓

False ∨ Q

↓

Q

Example

(P ∧ ¬P) ∧ R

↓

False ∧ R

↓

False

------------------------------------------------------------------------

# 6. Disjunction (OR) Rules

Important Rules

True ∨ Anything = True

False ∨ Q = Q

Examples

True ∨ False=True

True ∨ P=True

False ∨ P=P

False ∨ (P∧Q)=P∧Q

Think:

Once one side is already True, OR is satisfied.

------------------------------------------------------------------------

# 7. Conjunction (AND) Rules

Important Rules

False ∧ Anything=False

True ∧ Q=Q

Examples

False ∧ P=False

False ∧ True=False

True ∧ P=P

True ∧ (P∨Q)=P∨Q

Think:

One False immediately makes AND False.

------------------------------------------------------------------------

# 8. Conditional (Implication) Rules

Rule 1

True → False=False

Rule 2

False → Anything=True

Examples

If pigs fly then Earth is round.

False premise.

Automatically True.

Example

If 2+2=5 then Paris is in France.

False premise.

True implication.

Example

True → False

If I studied then I passed.

Suppose I studied but failed.

Promise broken.

False.

------------------------------------------------------------------------

# 9. Identity Law for OR

Formula

Q ∨ False = Q

Examples

Rain OR False

↓

Rain

P ∨ False=P

(P∧Q)∨False=P∧Q

------------------------------------------------------------------------

# 10. Identity Law for AND

Formula

Q ∧ True=Q

Examples

Rain AND True

↓

Rain

P∧True=P

(P∨Q)∧True=P∨Q

------------------------------------------------------------------------

# 11. Dominance Law for AND

Formula

Q ∧ False=False

False dominates everything.

Examples

Rain AND False=False

P∧False=False

(P∨Q)∧False=False

------------------------------------------------------------------------

# 12. Algebraic Evaluation

Instead of building a full truth table, simplify step by step.

Example

(P∨¬P)∧Q

↓

True∧Q

↓

Q

Since Q can be True or False,

Formula is consistent.

Example

(P∧¬P)∨Q

↓

False∨Q

↓

Q

Again consistent.

Example

(P∨¬P)

↓

True

Tautology.

Example

(P∧¬P)

↓

False

Contradiction.

------------------------------------------------------------------------

# 13. Self-Implication Tautology

Formula

Q→Q

Meaning

Anything implies itself.

Always True.

Examples

If today is Monday,

then today is Monday.

Always True.

If Python is a language,

then Python is a language.

Always True.

------------------------------------------------------------------------

# 14. False Premise Implication

Formula

False→Anything

Always True.

Examples

If 1=2,

then Earth revolves around Sun.

Premise is already False.

So implication is True.

Another Example

If pigs can code,

then Python is popular.

Premise False.

Whole implication True.

------------------------------------------------------------------------

# Quick Summary

  Concept   Always Result
  --------- ---------------
  P∨¬P      True
  P∧¬P      False
  Q∨False   Q
  Q∧True    Q
  Q∧False   False
  True∨Q    True
  False∨Q   Q
  False→Q   True
  Q→Q       True

------------------------------------------------------------------------

# Memory Tricks

Tautology → Always True

Contradiction → Always False

Consistent → True at least once

OR → One True is enough

AND → One False ruins everything

Implication → Broken only by True→False

These logical laws are widely used in Boolean algebra, Python
conditions, SQL query optimization, compiler design, theorem proving,
digital circuits, artificial intelligence, and database systems.
