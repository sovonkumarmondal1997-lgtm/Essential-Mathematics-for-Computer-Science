# Series and Summation Fundamentals

---

# 1. Series

## Definition

A **Series** is created when we **add together the terms of a sequence**.

### Sequence vs Series

A sequence is a list of numbers.

Example:

1, 2, 3, 4, 5

A series is the addition of those numbers.

Example:

1 + 2 + 3 + 4 + 5

---

## Example 1

Sequence:

2, 4, 6, 8

Series:

2 + 4 + 6 + 8 = 20

---

## Example 2

Sequence:

5, 10, 15, 20

Series:

5 + 10 + 15 + 20 = 50

---

## Example 3

Sequence:

1, 4, 9, 16

Series:

1 + 4 + 9 + 16 = 30

---

## Real-Life Example

Suppose you save money:

Day 1 = ₹10

Day 2 = ₹20

Day 3 = ₹30

Day 4 = ₹40

Sequence:

10, 20, 30, 40

Series:

10 + 20 + 30 + 40 = ₹100

Total savings = ₹100

---

# 2. Recursive Summation Formula

## Definition

A recursive formula defines a sum using the previous sum.

Instead of calculating everything from the beginning, we build the sum step by step.

General form:

Sₙ = Sₙ₋₁ + aₙ

where:

- Sₙ = sum of first n terms
- Sₙ₋₁ = previous sum
- aₙ = nth term

We also need a base case.

Example:

S₁ = 1

---

## Example 1

Sequence:

1, 2, 3, 4, 5

Base case:

S₁ = 1

Now:

S₂ = S₁ + 2
   = 1 + 2
   = 3

S₃ = S₂ + 3
   = 3 + 3
   = 6

S₄ = S₃ + 4
   = 6 + 4
   = 10

S₅ = S₄ + 5
   = 10 + 5
   = 15

Answer:

S₅ = 15

---

## Example 2

Sequence:

2, 4, 6, 8

Base case:

S₁ = 2

S₂ = 2 + 4 = 6

S₃ = 6 + 6 = 12

S₄ = 12 + 8 = 20

Answer:

S₄ = 20

---

## Why Recursive Formulas Matter

Many algorithms work recursively.

Examples:

- Factorial
- Fibonacci Numbers
- Dynamic Programming
- Tree Traversals

---

# 3. Sigma Notation (Σ)

## Definition

Sigma notation is a shorthand way of writing long sums.

The symbol:

Σ

means:

"Add all these terms."

General form:

Σ(k=1 to n) aₖ

Meaning:

Start at k=1

Keep increasing k

Stop at k=n

Add all generated terms

---

## Example 1

Σ(k=1 to 5) k

Expands to:

1 + 2 + 3 + 4 + 5

Answer:

15

---

## Example 2

Σ(k=1 to 4) 2k

Expands to:

2(1) + 2(2) + 2(3) + 2(4)

= 2 + 4 + 6 + 8

= 20

---

## Example 3

Σ(k=1 to 4) k²

Expands to:

1² + 2² + 3² + 4²

= 1 + 4 + 9 + 16

= 30

---

## Why Sigma Notation Is Useful

Instead of writing:

1 + 2 + 3 + ... + 100

we simply write:

Σ(k=1 to 100) k

Much shorter and cleaner.

---

# 4. Dummy Variable (k)

## Definition

The variable inside sigma notation is called a **dummy variable**.

It acts as a temporary counter.

Common choices:

- k
- i
- j
- n
- t

The name does not matter.

---

## Example 1

Σ(k=1 to 5) k

means

1 + 2 + 3 + 4 + 5

---

## Example 2

Σ(i=1 to 5) i

means

1 + 2 + 3 + 4 + 5

Same answer.

---

## Example 3

Σ(j=1 to 5) j

means

1 + 2 + 3 + 4 + 5

Same answer.

---

## Why Called Dummy?

Because after the summation is completed, the variable disappears.

For example:

Σ(k=1 to 5) k = 15

The k no longer matters.

Only 15 remains.

---

# 5. Sum of the First n Natural Numbers Formula

## Definition

Instead of adding numbers one by one:

1 + 2 + 3 + ... + n

we use:

Sₙ = n(n+1)/2

---

## Example 1

Find:

1 + 2 + 3 + 4 + 5

Using formula:

S₅ = 5(6)/2

= 30/2

= 15

---

## Example 2

Find:

1 + 2 + ... + 10

S₁₀ = 10(11)/2

= 55

---

## Example 3

Find:

1 + 2 + ... + 100

S₁₀₀ = 100(101)/2

= 5050

---

## Example 4

Find:

1 + 2 + ... + 1000

S₁₀₀₀ = 1000(1001)/2

= 500500

---

## Why Important?

Without formula:

Need 1000 additions.

With formula:

Only one calculation.

Huge time saving.

---

# 6. Proof by Reversal and Addition

## Definition

This elegant proof shows why:

Sₙ = n(n+1)/2

works.

---

## Example

Find:

1 + 2 + 3 + 4 + 5

Forward:

S = 1 + 2 + 3 + 4 + 5

Reverse:

S = 5 + 4 + 3 + 2 + 1

Add vertically:

2S = (1+5)
    +(2+4)
    +(3+3)
    +(4+2)
    +(5+1)

2S = 6 + 6 + 6 + 6 + 6

2S = 30

S = 15

---

## General Case

Forward:

S = 1 + 2 + 3 + ... + n

Reverse:

S = n + (n-1) + (n-2) + ... + 1

Add them:

2S = (n+1) + (n+1) + (n+1) + ... + (n+1)

There are n terms.

Therefore:

2S = n(n+1)

Divide by 2:

S = n(n+1)/2

Proved.

---

## Historical Story

A famous story says that young
:contentReference[oaicite:0]{index=0}
used this trick to quickly find:

1 + 2 + 3 + ... + 100

Answer:

5050

while his classmates were still adding.

---

# 7. Closed-Form Evaluation

## Definition

A closed-form formula gives the answer directly.

No repeated additions.

No loops.

No recursion.

Just plug values into a formula.

---

## Example 1

Without formula:

1 + 2 + 3 + ... + 100

Needs many additions.

Using closed form:

S₁₀₀ = 100(101)/2

= 5050

Done instantly.

---

## Example 2

Find:

1 + 2 + ... + 500

S₅₀₀ = 500(501)/2

= 125250

---

## Example 3

Find:

1 + 2 + ... + 10000

S₁₀₀₀₀ = 10000(10001)/2

= 50005000

---

## Why Computer Scientists Love Closed Forms

Suppose a loop runs:

for i in range(1,1000001):
    total += i

The computer performs 1,000,000 additions.

Using the formula:

1000000 × 1000001 / 2

The answer is obtained immediately.

This reduces work dramatically.

---

# Quick Summary Table

| Concept | Simple Meaning |
|----------|---------------|
| Sequence | Ordered list of numbers |
| Series | Sum of a sequence |
| Recursive Summation | Current sum = previous sum + next term |
| Sigma Notation (Σ) | Short way to write large sums |
| Dummy Variable | Temporary counter inside Σ |
| Sum Formula | Sₙ = n(n+1)/2 |
| Reversal & Addition Proof | Add forward and backward versions of a series |
| Closed-Form Evaluation | Direct formula without repeated calculations |

---

# Final Mental Model

Sequence:

1, 2, 3, 4, 5

↓

Series:

1 + 2 + 3 + 4 + 5

↓

Sigma Notation:

Σ(k=1 to 5) k

↓

Recursive Form:

Sₙ = Sₙ₋₁ + n

↓

Closed Form:

Sₙ = n(n+1)/2

↓

For n = 5:

S₅ = 5(6)/2 = 15

All five representations describe the same sum from different viewpoints.