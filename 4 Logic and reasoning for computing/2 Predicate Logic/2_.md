# Quantification in Predicate Logic - Beginner Friendly Notes

# 1. Quantification

## What is Quantification?

A predicate such as:

P(x): x is even

is **not complete** because we do not know which values of x we are
talking about.

**Quantification** tells us **how many objects in a domain satisfy a
predicate**.

It answers questions like:

-   Is the statement true for **every** object?
-   Is it true for **at least one** object?
-   Is it true for **exactly one** object?

Think of quantification as putting words like **all**, **some**, or
**exactly one** in front of a predicate.

### Example 1

Predicate:

Even(x)

Without quantification:

Even(x)

We do not know what x is.

With quantification:

∀x Even(x)

Meaning:

Every object is even.

With another quantifier:

∃x Even(x)

Meaning:

At least one object is even.

### Example 2

Predicate:

Student(x)

Quantifications:

∀x Student(x)

Every object is a student.

∃x Student(x)

At least one object is a student.

------------------------------------------------------------------------

# 2. Universe of Discourse

## What is the Universe of Discourse?

The **Universe of Discourse** (also called the **Domain**) is the
collection of all objects that variables are allowed to represent.

Before evaluating a predicate, we must know the universe.

Without a universe, the meaning of a predicate can change.

### Example 1

Universe:

{1,2,3,4,5}

Predicate:

Even(x)

Possible values:

Even(1)

Even(2)

Even(3)

Even(4)

Even(5)

### Example 2

Universe:

{Alice, Bob, Charlie}

Predicate:

Student(x)

Now x can only be:

Alice

Bob

Charlie

### Example 3

Universe:

All countries

Predicate:

InAsia(x)

India → True

Brazil → False

------------------------------------------------------------------------

# 3. Universal Quantifier (∀)

## Meaning

Symbol:

∀x

Read as:

"For every x"

or

"For all x"

The predicate must be true for **every object** in the universe.

### Think of it as a Continuous AND

Suppose

Universe = {1,2,3}

Statement:

∀x Positive(x)

Expands to:

Positive(1) AND Positive(2) AND Positive(3)

Every one must be True.

### Example 1

Universe:

{2,4,6}

Predicate:

Even(x)

∀x Even(x)

True

### Example 2

Universe:

{2,3,4}

∀x Even(x)

False

because 3 is not even.

### Example 3

All birds have wings.

∀x(Bird(x) → HasWings(x))

------------------------------------------------------------------------

# 4. Existential Quantifier (∃)

## Meaning

Symbol:

∃x

Read as:

"There exists an x"

or

"There is at least one x"

Only one object needs to satisfy the predicate.

### Think of it as a Continuous OR

Universe:

{1,2,3}

Statement:

∃x Even(x)

Expands to:

Even(1) OR Even(2) OR Even(3)

Only one True is enough.

### Example 1

Universe:

{1,3,5,8}

∃x Even(x)

True

because 8 is even.

### Example 2

Universe:

{1,3,5}

∃x Even(x)

False

No even numbers exist.

### Example 3

Some students play football.

∃x(Student(x) ∧ FootballPlayer(x))

------------------------------------------------------------------------

# 5. Uniqueness Quantifier (∃!)

## Meaning

Symbol:

∃!x

Read as:

"There exists exactly one x"

Exactly one object satisfies the predicate.

Not zero.

Not two.

Only one.

### Example 1

Universe:

{1,2,3,4}

Predicate:

x = 3

Exactly one value satisfies it.

∃!x(x=3)

True

### Example 2

Universe:

{1,2,3,4}

Predicate:

Even(x)

Even numbers are:

2

4

Two values satisfy it.

∃!x Even(x)

False

because there are two solutions.

### Example 3

Classroom

There is exactly one class monitor.

∃!x Monitor(x)

True

If two students are class monitors,

the statement becomes False.

------------------------------------------------------------------------

# Comparison Table

  Quantifier           Symbol   Meaning
  -------------------- -------- ---------------------
  Universal            ∀        Every object
  Existential          ∃        At least one object
  Unique Existential   ∃!       Exactly one object

------------------------------------------------------------------------

# Expansion over Finite Domains

Suppose

Universe = {a,b,c}

Universal

∀x P(x)

becomes

P(a) ∧ P(b) ∧ P(c)

Existential

∃x P(x)

becomes

P(a) ∨ P(b) ∨ P(c)

Unique Existential

Exactly one of

P(a)

P(b)

P(c)

is True.

------------------------------------------------------------------------

# Real-Life Examples

Example 1

All employees have IDs.

∀x(Employee(x) → HasID(x))

Example 2

Some employee is a manager.

∃x(Employee(x) ∧ Manager(x))

Example 3

Exactly one CEO exists.

∃!x CEO(x)

Example 4

All fruits contain seeds.

∀x(Fruit(x) → HasSeed(x))

Example 5

Some fruits are sweet.

∃x(Fruit(x) ∧ Sweet(x))

------------------------------------------------------------------------

# Memory Tricks

-   Quantification tells **how many objects** satisfy a predicate.
-   Universe of Discourse = The set of allowed objects.
-   ∀ = Every object (AND over a finite domain).
-   ∃ = At least one object (OR over a finite domain).
-   ∃! = Exactly one object.

These concepts are fundamental to predicate logic, SQL, relational
databases, artificial intelligence, knowledge representation, theorem
proving, formal verification, and mathematical reasoning.
