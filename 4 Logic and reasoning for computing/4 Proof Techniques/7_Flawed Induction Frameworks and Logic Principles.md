# Flawed Induction Frameworks and Logic Principles

# 1. Flawed Induction Frameworks

Mathematical induction is powerful, but it only works when **every
required step is correct**.

If even one step is wrong, the entire proof fails.

Two of the most common mistakes are explained below.

------------------------------------------------------------------------

# 1.1 Missing Base Case Fallacy

## What is it?

This mistake happens when someone correctly proves the **inductive
step** but **never proves the first case (base case)**.

Without the first case, induction cannot start.

Think of dominoes:

-   You proved every falling domino knocks over the next one.
-   But you never pushed the first domino.

Nothing falls.

------------------------------------------------------------------------

## Example 1

Claim:

Every natural number is greater than 100.

Suppose someone proves:

"If k \> 100, then k+1 \> 100."

That step is correct.

But what about the base case?

P(1):

1 \> 100

False.

Since the base case fails, the proof is invalid.

------------------------------------------------------------------------

## Example 2

Imagine climbing stairs.

You prove:

"If I can reach step k, I can reach step k+1."

Great.

But if you never show you can reach the **first step**, you never begin
climbing.

------------------------------------------------------------------------

# 1.2 Overlapping Subset Fallacy (Horse/Pencil Paradox)

## What is it?

This is one of the most famous incorrect induction proofs.

The false claim is:

"All horses have the same color."

The mistake comes from assuming two groups always overlap.

------------------------------------------------------------------------

## Incorrect Proof Idea

Suppose every group of k horses has the same color.

Now consider k+1 horses.

Split them into two groups:

Group 1:

Horse 1 ... Horse k

Group 2:

Horse 2 ... Horse k+1

The proof claims these groups overlap, so they must all have the same
color.

This works only when the overlap actually exists.

------------------------------------------------------------------------

## Where It Fails

Look at the first inductive step.

k = 1

Trying to prove it for 2 horses.

Groups become:

Group 1:

Horse A

Group 2:

Horse B

There is **no overlapping horse**.

Without a shared horse, you cannot conclude the colors are the same.

The proof breaks immediately.

------------------------------------------------------------------------

## Pencil Example

Claim:

Every pencil has the same color.

Take two pencils.

One is blue.

One is red.

The "overlap" disappears.

The argument fails exactly like the horse paradox.

------------------------------------------------------------------------

# 2. Logic Principles

# 2.1 Monochromatic Group Rule

## Meaning

If you want to prove an entire collection has the same color by
combining smaller groups,

you must first be able to prove the property for groups of size two.

Without the smallest valid overlap,

the induction cannot continue.

------------------------------------------------------------------------

## Example

Suppose we want to prove:

Every marble in a box is blue.

If we cannot even prove that **any two marbles** in the box are both
blue,

we certainly cannot prove that every marble is blue.

------------------------------------------------------------------------

## Another Example

Suppose we claim:

Every student in a class has the same favorite subject.

If two students already have different favorite subjects,

the larger claim immediately fails.

------------------------------------------------------------------------

# 2.2 Inductive Checklist Verification

## What is it?

When checking an induction proof, always verify two things.

### Step 1

Is the base case true?

### Step 2

Does the inductive step work for the **smallest possible value**?

Many incorrect proofs fail at the very first transition.

------------------------------------------------------------------------

## Example

Suppose the induction starts at n = 1.

Check:

P(1)

Then check

1 → 2

Many famous induction errors fail exactly here.

------------------------------------------------------------------------

## Example

Horse paradox.

Base case:

One horse has one color.

True.

Transition:

1 horse → 2 horses.

Fails because there is no overlap.

------------------------------------------------------------------------

# Real-Life Analogy

Imagine a relay race.

Runner 1 starts.

Runner 1 passes the baton to Runner 2.

Runner 2 passes it to Runner 3.

For the race to succeed:

-   Someone must actually start.
-   Every baton pass must work.

Missing either one causes the whole race to fail.

Induction works the same way.

------------------------------------------------------------------------

# Summary Table

  -----------------------------------------------------------------------
  Concept                         Main Idea
  ------------------------------- ---------------------------------------
  Missing Base Case Fallacy       No first domino, so induction never
                                  starts

  Overlapping Subset Fallacy      Overlap assumption fails at the
                                  smallest case

  Monochromatic Group Rule        Need valid overlap (at least size two)
                                  before generalizing

  Inductive Checklist             Always check the base case and the
  Verification                    first inductive transition
  -----------------------------------------------------------------------

------------------------------------------------------------------------

# Memory Tricks

-   No base case = No induction.
-   Always test the smallest value.
-   Never assume overlap exists---verify it.
-   Horse paradox fails at 1 → 2.
-   Before trusting an induction proof, ask:
    1.  Is the base case true?
    2.  Does the inductive step really work for the smallest boundary
        case?
