# First-Order Logic (Predicate Logic) - Simple Notes

# 1. First-Order Logic (Predicate Logic)

Propositional logic can only tell whether a whole statement is True or
False.

First-Order Logic (also called Predicate Logic) goes one step further.
It talks about **objects**, their **properties**, and the
**relationships** between them.

Think of it as asking: - Who? - What object? - Which person? - Which
number?

instead of only asking whether a complete sentence is true.

## Example

Propositional Logic: - "Alice is tall."

Predicate Logic: - Tall(x)

If x = Alice → Tall(Alice)

If x = Bob → Tall(Bob)

Now the truth depends on the object.

------------------------------------------------------------------------

# 2. Predicate

A predicate is like a function that becomes a True/False statement after
supplying one or more objects.

Examples

Odd(x)

Even(x)

Student(x)

Likes(x, IceCream)

Equal(x, y)

If x = 7

Odd(7) = True

If x = 8

Odd(8) = False

Another example

Likes(Alice, Pizza)

may be True.

Likes(Bob, Pizza)

may be False.

------------------------------------------------------------------------

# 3. Domain

The domain is the collection of objects from which variables are chosen.

Examples

Numbers

Domain = {1,2,3,4,5}

Students

Domain = {Alice, Bob, Charlie}

Animals

Domain = {Dog, Cat, Cow}

Without knowing the domain, predicates can be ambiguous.

------------------------------------------------------------------------

# 4. Existential Quantifier (∃)

Symbol

∃

Meaning

"There exists at least one."

Example

∃x Odd(x)

Meaning

There exists at least one odd number.

Example

∃x Student(x)

Meaning

At least one student exists.

One example is enough.

------------------------------------------------------------------------

# 5. Universal Quantifier (∀)

Symbol

∀

Meaning

"For every object."

Example

∀x Human(x) → Mortal(x)

Meaning

Every human is mortal.

Another example

∀x Even(x)

would mean

Every object in the domain is even.

------------------------------------------------------------------------

# 6. Universal Affirmative

English

All P are Q.

Logic

∀x (P(x) → Q(x))

Examples

All birds have wings.

∀x(Bird(x) → HasWings(x))

All students have ID cards.

∀x(Student(x) → HasID(x))

------------------------------------------------------------------------

# 7. Universal Negative

English

No P are Q.

Logic

∀x(P(x) → ¬Q(x))

Examples

No cats are reptiles.

∀x(Cat(x) → ¬Reptile(x))

No squares are circles.

∀x(Square(x) → ¬Circle(x))

------------------------------------------------------------------------

# 8. Existential Affirmative

English

Some P are Q.

Logic

∃x(P(x) ∧ Q(x))

Examples

Some students play football.

∃x(Student(x) ∧ FootballPlayer(x))

Some fruits are sweet.

∃x(Fruit(x) ∧ Sweet(x))

------------------------------------------------------------------------

# 9. Existential Negative

English

Some P are not Q.

Logic

∃x(P(x) ∧ ¬Q(x))

Examples

Some birds cannot fly.

∃x(Bird(x) ∧ ¬CanFly(x))

Some students are not present.

∃x(Student(x) ∧ ¬Present(x))

------------------------------------------------------------------------

# 10. Counter-example Disproof

To disprove a universal statement, find one object where it fails.

Example

Claim

All birds fly.

Counter-example

Penguin.

Since penguins do not fly, the statement is false.

Another example

Claim

All numbers are even.

Counter-example

3

One counter-example is enough.

------------------------------------------------------------------------

# 11. Quantifier Expansion via Connectives

Works only for finite domains.

Suppose

Domain={1,2,3}

Universal

∀x P(x)

expands to

P(1) ∧ P(2) ∧ P(3)

Existential

∃x P(x)

expands to

P(1) ∨ P(2) ∨ P(3)

Examples

All students passed

Passed(Alice) ∧ Passed(Bob) ∧ Passed(Charlie)

Some student passed

Passed(Alice) ∨ Passed(Bob) ∨ Passed(Charlie)

------------------------------------------------------------------------

# 12. Quantifier Negation Laws

Law 1

¬∃x P(x)

≡

∀x ¬P(x)

Meaning

"It is not true that someone..."

becomes

"Everyone does not..."

Example

No student failed.

¬∃x Failed(x)

≡

∀x ¬Failed(x)

------------------------------------------------------------------------

Law 2

¬∀x P(x)

≡

∃x ¬P(x)

Meaning

Not everyone satisfies the property.

Someone does not satisfy it.

Example

Not every student passed.

¬∀x Passed(x)

≡

∃x ¬Passed(x)

------------------------------------------------------------------------

# Summary Table

  English            Logic
  ------------------ ----------
  All P are Q        ∀x(P→Q)
  No P are Q         ∀x(P→¬Q)
  Some P are Q       ∃x(P∧Q)
  Some P are not Q   ∃x(P∧¬Q)
  There exists       ∃
  For all            ∀

------------------------------------------------------------------------

# Memory Tricks

-   Predicate = Property or relationship.
-   Domain = Collection of objects.
-   ∀ = Every object.
-   ∃ = At least one object.
-   To disprove "All", find one counter-example.
-   ∀ expands using AND.
-   ∃ expands using OR.
-   Negating ∀ changes it to ∃.
-   Negating ∃ changes it to ∀.

These concepts are the foundation of mathematical proofs, databases,
SQL, knowledge representation, artificial intelligence, formal
verification, and logic programming.
