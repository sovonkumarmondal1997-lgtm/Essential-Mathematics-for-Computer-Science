# Predicate Logic Fundamentals - Beginner Friendly Notes

# 1. Predicate Logic

Predicate Logic (also called First-Order Logic) extends propositional
logic by allowing statements to contain variables. Instead of treating
an entire sentence as simply True or False, predicate logic lets us
describe properties of objects and determine truth after assigning
values.

Think of it like this:

-   Propositional Logic asks: "Is this sentence true?"
-   Predicate Logic asks: "For which objects is this sentence true?"

## Example

Statement:

x is an even number.

This is incomplete because x is unknown.

If x = 4 → True

If x = 7 → False

Predicate logic handles these changing truth values.

------------------------------------------------------------------------

# 2. Limitation of Propositional Logic

Propositional logic can only handle complete statements that are already
True or False.

It cannot directly represent statements whose truth depends on a
variable.

## Example 1

x² = 4

Is it True?

We cannot answer because x is unknown.

If x = 2 → True

If x = -2 → True

If x = 3 → False

Therefore it is not a proposition.

## Example 2

x \> 10

Without knowing x, no truth value exists.

## Example 3

Student x passed the exam.

Until we know who x is, we cannot determine truth.

------------------------------------------------------------------------

# 3. Predicate Logic Solution

Predicate logic solves this problem by introducing variables into
logical statements.

Instead of writing:

"x² = 4"

we write

P(x): x² = 4

Now P(x) is a predicate.

Once x receives a value, it becomes a proposition.

Examples

P(2) = True

P(-2) = True

P(5) = False

------------------------------------------------------------------------

# 4. Predicate

A predicate describes a property or relationship.

Think of it like a Python function that returns True or False.

General form

P(x)

Examples

Even(x)

Prime(x)

Tall(x)

Student(x)

Examples

Even(8) = True

Even(9) = False

Prime(13) = True

Prime(15) = False

Tall(Alice) may be True.

Tall(Bob) may be False.

------------------------------------------------------------------------

# 5. Subject (Variable)

The subject is the variable that receives the property.

Usually written as

x

y

z

Examples

Even(x)

Student(x)

Age(x)

If

x = 20

Age(x) \> 18

becomes

Age(20) \> 18

which is True.

------------------------------------------------------------------------

# 6. Propositional Function

A propositional function combines a predicate and one or more variables.

General form

P(x)

It is not yet True or False until values are supplied.

Examples

P(x): x \> 5

P(7) = True

P(3) = False

Example

Q(x): x is divisible by 3

Q(12) = True

Q(10) = False

------------------------------------------------------------------------

# 7. Single-Parameter Predicate

A predicate involving only one variable.

General form

P(x)

Examples

Even(x)

Odd(x)

Prime(x)

Positive(x)

Examples

Prime(11) = True

Prime(12) = False

Positive(-4) = False

Positive(10) = True

------------------------------------------------------------------------

# 8. Multiple-Parameter Predicate

A predicate involving two or more variables.

General forms

P(x,y)

Q(x,y,z)

Examples

Greater(x,y)

Equal(x,y)

LessThan(x,y)

AddLess(x,y,z)

Example

Greater(9,4)

True

Greater(2,8)

False

Example

Q(x,y,z)

x+y\<z

Q(2,3,8)

5\<8

True

Q(4,5,6)

9\<6

False

Example

Equal(x,y)

Equal(5,5)

True

Equal(7,3)

False

------------------------------------------------------------------------

# 9. Logical Operator Integration

Once predicates become propositions by assigning values, we can combine
them using logical operators.

AND

OR

NOT

Implication

Examples

P(x): x is even

Q(x): x \> 5

Suppose

x = 8

P(8)=True

Q(8)=True

P(8) AND Q(8)

True

Example

x=4

P(4)=True

Q(4)=False

P(4) OR Q(4)

True

Example

x=3

P(3)=False

NOT P(3)

True

Example

P(x): Student studies

Q(x): Student passes

P(Alice) → Q(Alice)

If Alice studies, then Alice passes.

------------------------------------------------------------------------

# Real-Life Examples

Example 1

Predicate

CanVote(x)

Person

Alice

CanVote(Alice)

True

Example 2

Predicate

HasDrivingLicense(x)

HasDrivingLicense(Bob)

False

Example 3

Predicate

Employee(x)

Manager(x)

Employee(Alice) AND Manager(Alice)

Example 4

Friend(x,y)

Friend(Alice,Bob)

Friend(Bob,Alice)

These are two different predicates.

------------------------------------------------------------------------

# Comparison

  Concept                  Example
  ------------------------ -------------------------
  Proposition              5\>3
  Predicate                Greater(x,3)
  Variable                 x
  Propositional Function   P(x)
  Single Parameter         Even(x)
  Multiple Parameter       Greater(x,y)
  Compound Predicate       Even(x) AND Positive(x)

------------------------------------------------------------------------

# Memory Tricks

-   Predicate = Property or relationship.
-   Variable = Input to the predicate.
-   Predicate + Value = Proposition.
-   One variable → Single-parameter predicate.
-   Two or more variables → Multiple-parameter predicate.
-   After evaluation, predicates can be combined using AND, OR, NOT, and
    implication.

Predicate logic forms the mathematical foundation of SQL queries,
relational databases, artificial intelligence, machine learning,
knowledge graphs, theorem proving, and logic programming.
