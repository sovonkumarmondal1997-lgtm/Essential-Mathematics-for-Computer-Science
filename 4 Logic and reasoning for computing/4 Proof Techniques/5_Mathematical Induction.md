# Mathematical Induction

# 1. Mathematical Induction

## What is Mathematical Induction?

Mathematical induction is a proof technique used to show that a
statement is true for **every natural number** (0, 1, 2, 3, ... or 1, 2,
3, ... depending on the problem).

Instead of checking infinitely many numbers one by one, induction proves
the first case and then proves that each true case automatically makes
the next one true.

Think of it as building an infinite chain.

If the first link is secure and every link connects to the next, then
the whole chain holds together.

------------------------------------------------------------------------

## Example

Claim:

1 + 2 + 3 + ... + n = n(n + 1)/2

Instead of checking:

n = 1

n = 2

n = 3

...

forever,

we use mathematical induction to prove it for **all** natural numbers at
once.

------------------------------------------------------------------------

# 2. Domino Analogy

The most famous way to understand induction is with dominoes.

Imagine an infinitely long row of dominoes.

To make every domino fall, only two things are needed.

### Step 1

Push the first domino.

(Base Case)

### Step 2

Show that whenever one domino falls,

it always knocks down the next domino.

(Inductive Step)

Then:

Domino 1 falls.

Therefore Domino 2 falls.

Therefore Domino 3 falls.

Therefore Domino 4 falls.

...

Eventually every domino falls.

This is exactly how mathematical induction works.

------------------------------------------------------------------------

# 3. The Four Steps of Mathematical Induction

Every induction proof follows the same structure.

1.  Base Case
2.  Inductive Hypothesis
3.  Inductive Step
4.  Conclusion

------------------------------------------------------------------------

# 3.1 Base Case

## What is the Base Case?

The base case proves that the statement is true for the very first
value.

Usually:

P(0)

or

P(1)

depending on the problem.

If the first domino never falls,

nothing else can happen.

------------------------------------------------------------------------

## Example

Claim:

1 + 2 + ... + n = n(n+1)/2

Base case:

n = 1

Left side

= 1

Right side

= 1(2)/2 = 1

Both sides are equal.

Therefore,

P(1) is true.

------------------------------------------------------------------------

# 3.2 Inductive Hypothesis

## What is the Inductive Hypothesis?

Assume the statement is already true for an arbitrary number k.

This is **not cheating**.

It is only a temporary assumption used to prove the next step.

Write:

Assume

P(k)

is true.

Example

Assume

1 + 2 + ... + k

=

k(k+1)/2

------------------------------------------------------------------------

# 3.3 Inductive Step

Now prove

P(k+1)

using the inductive hypothesis.

Example

Start with

1 + 2 + ... + k + (k+1)

Replace the first part using the hypothesis.

=

k(k+1)/2 + (k+1)

Factor

(k+1)

=

(k+1)(k/2 + 1)

=

(k+1)(k+2)/2

This matches the required formula.

Therefore,

P(k+1)

is true.

------------------------------------------------------------------------

# 3.4 Conclusion

Since

-   the base case is true, and
-   P(k) implies P(k+1),

the statement is true for every natural number.

Usually we finish by writing:

Therefore,

the statement holds for all natural numbers.

□

The square symbol means:

Proof Complete.

------------------------------------------------------------------------

# Another Example

Claim:

2 + 4 + 6 + ... + 2n

=

n(n+1)

### Base Case

n=1

Left

2

Right

1×2

=2

Correct.

------------------------------------------------------------------------

### Hypothesis

Assume

2+4+...+2k

=

k(k+1)

------------------------------------------------------------------------

### Inductive Step

Add

2(k+1)

Left side

=

k(k+1)+2(k+1)

Factor

(k+1)

=

(k+1)(k+2)

This is exactly the required formula.

Therefore,

P(k+1)

is true.

------------------------------------------------------------------------

### Conclusion

The formula is true for every natural number.

□

------------------------------------------------------------------------

# Real-Life Analogy

Imagine teaching a line of people.

Person 1 learns the skill.

Every trained person teaches the next person.

Eventually,

everyone learns.

This is induction.

------------------------------------------------------------------------

# Summary Table

  Step                   Purpose
  ---------------------- ---------------------------------------------------------
  Base Case              Show the first value is true
  Inductive Hypothesis   Assume the statement is true for k
  Inductive Step         Use P(k) to prove P(k+1)
  Conclusion             Therefore the statement is true for all natural numbers

------------------------------------------------------------------------

# Memory Tricks

-   Base Case = Push the first domino.
-   Hypothesis = Assume domino k has fallen.
-   Inductive Step = Domino k knocks over domino k+1.
-   Conclusion = Every domino falls.
-   Induction proves infinitely many cases with only two main proofs.

Mathematical induction is widely used in algorithms, recursion, data
structures, discrete mathematics, graph theory, number theory, compiler
correctness, and theoretical computer science.
