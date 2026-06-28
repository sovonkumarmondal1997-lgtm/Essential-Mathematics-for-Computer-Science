# Contradiction and Contrapositive Proof Strategies

# 1. Contradiction Proof Strategy

## What is the Strategy?

Suppose we want to prove:

"If 5n + 2 is even, then n is even."

Instead of proving it directly, we assume:

-   The premise is true.
-   The conclusion is false.

For an implication A → B, assume:

A is True

and

B is False

Then try to reach an impossible result.

------------------------------------------------------------------------

## Step-by-Step Example

Claim:

If 5n + 2 is even,

then n is even.

### Step 1

Assume

5n + 2 is even.

### Step 2

Assume the opposite of the conclusion.

Suppose n is odd.

Write

n = 2k + 1

### Step 3

Substitute.

5n + 2

= 5(2k + 1) + 2

= 10k + 5 + 2

= 10k + 7

Factor:

= 2(5k + 3) + 1

This is odd.

But we assumed

5n + 2

was even.

Contradiction.

Therefore,

n cannot be odd.

Hence,

n must be even.

------------------------------------------------------------------------

# 2. Contrapositive Proof Strategy

Instead of looking for a contradiction, rewrite the statement.

Original:

If 5n + 2 is even,

then n is even.

Contrapositive:

If n is odd,

then 5n + 2 is odd.

Now prove this directly.

------------------------------------------------------------------------

## Step-by-Step

Assume

n = 2k + 1

Substitute.

5n + 2

= 5(2k + 1) + 2

= 10k + 7

Rewrite.

= 2(5k + 3) + 1

This has the form

2m + 1

Therefore,

5n + 2

is odd.

Since the contrapositive is true,

the original implication is also true.

------------------------------------------------------------------------

# 3. Implication Falsity Condition

An implication

A → B

is false only in one situation.

The premise is true,

but the conclusion is false.

Truth Table

  A   B   A→B
  --- --- -----
  T   T   T
  T   F   F
  F   T   T
  F   F   T

This is why contradiction proofs assume:

Premise = True

Conclusion = False

because that is the only way an implication could fail.

------------------------------------------------------------------------

## Example

"If I study,

then I pass."

The implication fails only if:

I studied

but

I did not pass.

Every other situation satisfies the implication.

------------------------------------------------------------------------

# 4. Odd Parity Evaluation

Odd numbers always have the form:

2k + 1

Substitute this form into an expression.

If the result can still be written as

2m + 1,

then the result is odd.

------------------------------------------------------------------------

## Example 1

Suppose

n = 2k + 1

Find

3n + 2

Substitute.

3(2k + 1) + 2

= 6k + 5

Rewrite.

= 2(3k + 2) + 1

Therefore,

3n + 2

is odd.

------------------------------------------------------------------------

## Example 2

Suppose

n = 2k + 1

Find

7n + 4

Substitute.

7(2k + 1) + 4

= 14k + 11

Rewrite.

= 2(7k + 5) + 1

Therefore,

7n + 4

is odd.

------------------------------------------------------------------------

## Example 3

Suppose

n = 2k + 1

Find

9n + 8

Substitute.

9(2k + 1) + 8

= 18k + 17

Rewrite.

= 2(9k + 8) + 1

Therefore,

9n + 8

is odd.

------------------------------------------------------------------------

# Comparison

  ----------------------------------------------------------------------------
  Method           Starting Assumption                         Goal
  ---------------- ------------------------------------------- ---------------
  Direct Proof     Premise is true                             Show conclusion

  Contrapositive   Negated conclusion                          Show negated
                                                               premise

  Contradiction    Premise true and conclusion false           Reach
                                                               impossibility
  ----------------------------------------------------------------------------

------------------------------------------------------------------------

# Memory Tricks

-   Contradiction = Assume the only failing case.
-   Contrapositive = Reverse and negate.
-   Implication fails only for True → False.
-   Odd numbers always look like 2k + 1.
-   If an expression becomes 2m + 1, it is odd.

These proof strategies are widely used in number theory, discrete
mathematics, algorithms, cryptography, compiler correctness, and
theoretical computer science.
