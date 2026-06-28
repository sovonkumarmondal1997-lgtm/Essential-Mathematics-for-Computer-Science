# Predicate Logic Inference Rules - Beginner Friendly Notes

# 1. Universal Instantiation (UI)

## Meaning

If a statement is true for **every object**, then it must also be true
for any particular object.

Rule:

∀x P(x) ⇒ P(c)

where c is a specific member of the domain.

### Example 1

All humans are mortal.

∀x(Human(x) → Mortal(x))

Alice is a human.

Therefore,

Human(Alice) → Mortal(Alice)

### Example 2

All even numbers are divisible by 2.

Therefore,

8 is divisible by 2.

------------------------------------------------------------------------

# 2. Universal Generalization (UG)

## Meaning

If you prove a statement for an **arbitrary object**, then it is true
for all objects.

Rule:

P(c) ⇒ ∀x P(x)

Important:

The object c must be arbitrary, not specially chosen.

### Example

Suppose c is any positive number.

You prove:

c² ≥ 0

Since c was arbitrary,

∀x(x² ≥ 0)

------------------------------------------------------------------------

# 3. Existential Instantiation (EI)

## Meaning

If at least one object satisfies a property, you may temporarily give
that object a name.

Rule:

∃x P(x)

⇒

P(c)

where c is a new temporary object.

### Example 1

Some student scored 100.

∃x PerfectScore(x)

Choose a temporary student:

Alice

Now work with

PerfectScore(Alice)

We do not know who Alice actually is.

She is just a temporary placeholder.

------------------------------------------------------------------------

# 4. Existential Generalization (EG)

## Meaning

If a property is true for one known object, then at least one object has
that property.

Rule:

P(c)

⇒

∃x P(x)

### Example 1

Alice is a programmer.

Therefore,

Someone is a programmer.

### Example 2

7 is prime.

Therefore,

There exists a prime number.

------------------------------------------------------------------------

# 5. Universal Modus Ponens

This combines Universal Instantiation with Modus Ponens.

Rule:

∀x(P(x) → Q(x))

P(a)

Therefore,

Q(a)

### Example 1

All birds have wings.

Sparrow is a bird.

Therefore,

Sparrow has wings.

### Example 2

Every employee has an ID.

Bob is an employee.

Therefore,

Bob has an ID.

------------------------------------------------------------------------

# 6. Universal Modus Tollens

This combines Universal Instantiation with Modus Tollens.

Rule:

∀x(P(x) → Q(x))

¬Q(a)

Therefore,

¬P(a)

### Example 1

All programmers know programming.

Tom does not know programming.

Therefore,

Tom is not a programmer.

### Example 2

Every square has four sides.

Shape A does not have four sides.

Therefore,

Shape A is not a square.

------------------------------------------------------------------------

# 7. Nested Quantifier Translation

Complex English sentences often contain multiple quantifiers.

Translate step by step.

## Example 1

Every student knows some programming language.

Step 1

Every student

↓

∀x Student(x)

Step 2

Some programming language

↓

∃y Language(y)

Step 3

Connect them

∀x(Student(x) → ∃y(Language(y) ∧ Knows(x,y)))

------------------------------------------------------------------------

## Example 2

Every positive number has a larger positive number.

∀x(Positive(x) → ∃y(Positive(y) ∧ y\>x))

------------------------------------------------------------------------

## Example 3

Every person has a mother.

∀x(Person(x) → ∃y(MotherOf(y,x)))

------------------------------------------------------------------------

# 8. Domain-Dependent Quantification

The logical formula depends on the universe of discourse.

## Broad Domain

Suppose the universe is "all objects."

Statement:

All students study.

We must first identify students.

∀x(Student(x) → Studies(x))

Notice the implication (→).

------------------------------------------------------------------------

## Narrow Domain

Suppose the universe contains only students.

Now we already know every object is a student.

The formula becomes

∀x Studies(x)

No implication is needed.

------------------------------------------------------------------------

## Existential Example (Broad Domain)

Some students play football.

Universe:

All people

Formula

∃x(Student(x) ∧ PlaysFootball(x))

Notice the conjunction (∧).

Both conditions must describe the same object.

------------------------------------------------------------------------

## Existential Example (Narrow Domain)

Universe:

Only students

Formula

∃x PlaysFootball(x)

No Student(x) predicate is necessary.

------------------------------------------------------------------------

# Summary Table

  -----------------------------------------------------------------------
  Rule              Formula                    Meaning
  ----------------- -------------------------- --------------------------
  Universal         ∀xP(x) ⇒ P(c)              Choose one object
  Instantiation                                

  Universal         P(c) ⇒ ∀xP(x)              Generalize from arbitrary
  Generalization                               object

  Existential       ∃xP(x) ⇒ P(c)              Give unknown object a
  Instantiation                                temporary name

  Existential       P(c) ⇒ ∃xP(x)              One example proves
  Generalization                               existence

  Universal Modus   ∀x(P→Q), P(a) ⇒ Q(a)       Apply implication to one
  Ponens                                       object

  Universal Modus   ∀x(P→Q), ¬Q(a) ⇒ ¬P(a)     Reject the premise for one
  Tollens                                      object
  -----------------------------------------------------------------------

------------------------------------------------------------------------

# Memory Tricks

-   UI: All → One.
-   UG: Arbitrary One → All.
-   EI: Someone → Temporary Name.
-   EG: One Example → Someone Exists.
-   Universal Modus Ponens = UI + Modus Ponens.
-   Universal Modus Tollens = UI + Modus Tollens.
-   Broad domains usually need → for universal statements.
-   Broad domains usually need ∧ for existential statements.

These inference rules are widely used in mathematics, database theory,
SQL, formal proofs, artificial intelligence, theorem proving, and logic
programming.
