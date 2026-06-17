# Floor Functions and Ceiling Functions

---

# 1. Floor Function

## Definition

The **Floor Function** maps a real number to the **largest integer that is less than or equal to that number**.

Notation:

⌊x⌋

Read as:

"Floor of x"

or

"Greatest integer less than or equal to x"

---

## Simple Idea

The floor function always moves downward to the nearest integer.

Think:

"Go down to the next whole number."

---

## Examples

### Example 1

⌊4.8⌋ = 4

Because:

4 ≤ 4.8 < 5

---

### Example 2

⌊7.1⌋ = 7

Because:

7 ≤ 7.1 < 8

---

### Example 3

⌊10⌋ = 10

Because 10 is already an integer.

---

## Real-Life Example

Suppose a hotel charges per full night.

Stayed:

4.9 nights

Counted as:

4 completed nights

Floor value:

⌊4.9⌋ = 4

---

# 2. Inequality Bounds for the Floor Function

## Definition

The floor function is formally defined by:

If

n ≤ x < n + 1

then

⌊x⌋ = n

---

## Meaning

Find the integer interval containing x.

The left endpoint becomes the floor value.

---

## Example 1

x = 3.6

Observe:

3 ≤ 3.6 < 4

Therefore:

⌊3.6⌋ = 3

---

## Example 2

x = 8.99

Observe:

8 ≤ 8.99 < 9

Therefore:

⌊8.99⌋ = 8

---

## Example 3

x = -1.2

Observe:

-2 ≤ -1.2 < -1

Therefore:

⌊-1.2⌋ = -2

---

# 3. Floor of Negative Numbers

## Definition

For negative numbers, floor still means:

Largest integer less than or equal to x.

The movement is downward on the number line.

---

## Important Rule

For negatives:

Floor moves away from zero.

---

## Example 1

⌊-2.5⌋

Integers around -2.5:

-3, -2

Largest integer ≤ -2.5 is:

-3

Answer:

⌊-2.5⌋ = -3

---

## Example 2

⌊-4.1⌋ = -5

Because:

-5 ≤ -4.1 < -4

---

## Example 3

⌊-7.99⌋ = -8

---

## Common Mistake

Wrong:

⌊-2.5⌋ = -2

Correct:

⌊-2.5⌋ = -3

Remember:

Floor goes downward.

---

# 4. Integer Invariance Property

## Definition

If x is already an integer:

⌊x⌋ = x

and

⌈x⌉ = x

---

## Meaning

Integers remain unchanged.

---

## Examples

⌊5⌋ = 5

⌈5⌉ = 5

---

⌊-7⌋ = -7

⌈-7⌉ = -7

---

⌊0⌋ = 0

⌈0⌉ = 0

---

## Why?

The number is already whole.

No rounding needed.

---

# 5. Step Function / Piecewise Constant Function

## Definition

A step function is a graph made of horizontal segments.

It looks like stairs.

Both floor and ceiling functions create step-shaped graphs.

---

## Example

Floor Function

⌊x⌋

Values:

| x Interval | Output |
|------------|----------|
| 0 ≤ x < 1 | 0 |
| 1 ≤ x < 2 | 1 |
| 2 ≤ x < 3 | 2 |

---

Graph Shape

```
     ___
    |
 ___|
|
|___
```

Looks like stairs.

---

## Real-Life Example

Parking fees:

0–1 hour → ₹50

1–2 hours → ₹100

2–3 hours → ₹150

Fee changes in steps rather than continuously.

---

# 6. Ceiling Function

## Definition

The **Ceiling Function** maps a real number to the smallest integer greater than or equal to that number.

Notation:

⌈x⌉

Read as:

"Ceiling of x"

---

## Simple Idea

Always move upward to the nearest integer.

Think:

"Go up to the next whole number."

---

## Examples

### Example 1

⌈4.2⌉ = 5

---

### Example 2

⌈7.01⌉ = 8

---

### Example 3

⌈10⌉ = 10

Already an integer.

---

## Real-Life Example

Suppose one taxi can carry 4 people.

Passengers:

17

Required taxis:

⌈17/4⌉

= ⌈4.25⌉

= 5

Need 5 taxis.

---

# 7. Inequality Bounds for the Ceiling Function

## Definition

If

n < x ≤ n+1

then

⌈x⌉ = n+1

---

## Meaning

Find the interval containing x.

Choose the upper endpoint.

---

## Example 1

x = 3.2

Observe:

3 < 3.2 ≤ 4

Therefore:

⌈3.2⌉ = 4

---

## Example 2

x = 8.7

Observe:

8 < 8.7 ≤ 9

Therefore:

⌈8.7⌉ = 9

---

## Example 3

x = -1.2

Observe:

-2 < -1.2 ≤ -1

Therefore:

⌈-1.2⌉ = -1

---

# 8. Ceiling of Negative Numbers

## Definition

For negative numbers:

Ceiling moves upward toward zero.

---

## Example 1

⌈-2.5⌉

Nearby integers:

-3 and -2

Smallest integer ≥ -2.5:

-2

Answer:

⌈-2.5⌉ = -2

---

## Example 2

⌈-4.7⌉ = -4

---

## Example 3

⌈-8.1⌉ = -8

---

## Memory Trick

Floor:

Downward

Ceiling:

Upward

Even for negative numbers.

---

# 9. Mathematical Proof by Substitution and Bounds

## Definition

Many floor and ceiling properties are proven using:

1. Bound inequalities
2. Algebraic manipulation
3. Substitution

---

## Example

Prove:

⌊x⌋ ≤ x

---

Let:

⌊x⌋ = n

By definition:

n ≤ x < n+1

Immediately:

n ≤ x

Since:

n = ⌊x⌋

Therefore:

⌊x⌋ ≤ x

Proved.

---

## Example 2

Show:

x < ⌊x⌋ + 1

From:

n ≤ x < n+1

Substitute:

n = ⌊x⌋

Result:

x < ⌊x⌋ + 1

Proved.

---

## General Strategy

Convert floor expression

↓

Use inequalities

↓

Manipulate algebraically

↓

Substitute back

↓

Finish proof

---

# 10. Integer Additivity Property

## Definition

For any integer n:

⌊x+n⌋

=

⌊x⌋+n

---

## Meaning

Whole numbers can move outside the floor function.

---

## Example 1

x = 3.7

n = 2

Left Side:

⌊3.7+2⌋

=⌊5.7⌋

=5

Right Side:

⌊3.7⌋+2

=3+2

=5

Equal.

---

## Example 2

x = 8.2

n = 5

Left:

⌊13.2⌋

=13

Right:

⌊8.2⌋+5

=8+5

=13

Equal.

---

## Example 3

Negative Case

x = -2.3

n = 4

Left:

⌊1.7⌋

=1

Right:

⌊-2.3⌋+4

=-3+4

=1

Equal.

---

## Why It Works

Suppose:

⌊x⌋ = k

Then:

k ≤ x < k+1

Add n:

k+n ≤ x+n < k+n+1

Therefore:

⌊x+n⌋ = k+n

Since:

k=⌊x⌋

Result:

⌊x+n⌋ = ⌊x⌋+n

Proved.

---

# Quick Comparison Table

| Concept | Floor | Ceiling |
|----------|----------|----------|
| Symbol | ⌊x⌋ | ⌈x⌉ |
| Direction | Down | Up |
| 4.8 | 4 | 5 |
| 2.1 | 2 | 3 |
| -2.5 | -3 | -2 |
| Integer Input | Same Number | Same Number |
| Graph Shape | Steps | Steps |

---

# Visual Number Line Example

Number:

3.6

```
3 -------- 3.6 -------- 4
```

Floor:

3

Ceiling:

4

---

Number:

-2.5

```
-3 ------- -2.5 ------- -2
```

Floor:

-3

Ceiling:

-2

---

# Learning Flow

Real Numbers
↓
Integers
↓
Floor Function
↓
Ceiling Function
↓
Inequality Bounds
↓
Negative Values
↓
Step Functions
↓
Mathematical Proofs
↓
Integer Properties
↓
Discrete Mathematics

---

# Key Facts to Remember

1. Floor means round downward.

2. Ceiling means round upward.

3. Floor of a negative number moves farther left on the number line.

4. Ceiling of a negative number moves toward zero.

5. Integers remain unchanged under floor and ceiling.

6. Floor and ceiling graphs look like stairs.

7. Floor uses:
   n ≤ x < n+1

8. Ceiling uses:
   n < x ≤ n+1

9. Integer additivity:
   ⌊x+n⌋ = ⌊x⌋ + n

10. Floor and ceiling functions are heavily used in:
    - Computer Science
    - Algorithms
    - Data Engineering
    - Database Systems
    - Scheduling Problems
    - Cryptography
    - Discrete Mathematics
    - Numerical Computing

Think of the floor function as always stepping down to the nearest safe integer below, and the ceiling function as always stepping up to the nearest safe integer above.