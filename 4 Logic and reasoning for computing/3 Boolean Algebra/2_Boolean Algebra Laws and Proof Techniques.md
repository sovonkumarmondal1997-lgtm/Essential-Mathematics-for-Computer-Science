# Boolean Algebra Laws and Proof Techniques - Beginner Friendly Notes

# 1. Huntington's Postulates

Huntington's Postulates are the basic rules that a system must satisfy
to be called a Boolean Algebra.

The six main ideas are:

1.  Closure -- combining Boolean values always gives another Boolean
    value.
2.  Identity -- 0 and 1 act as identity elements.
3.  Commutativity -- order does not matter.
4.  Distributivity -- AND distributes over OR and OR distributes over
    AND.
5.  Complements -- every variable has an opposite.
6.  Distinct Elements -- 0 and 1 are different.

### Examples

-   1 + 0 = 1 (closure)
-   x + 0 = x (identity)
-   x·y = y·x (commutative)
-   x + x' = 1 (complement)

------------------------------------------------------------------------

# 2. Idempotent Laws

Using the same variable twice changes nothing.

x + x = x

x·x = x

### Examples

A OR A = A

A AND A = A

If a light switch is ON OR ON, it is still ON.

------------------------------------------------------------------------

# 3. Tautology and Contradiction Laws

x + 1 = 1

x·0 = 0

### Examples

True OR anything = True

False AND anything = False

If an alarm is forced ON, OR with anything stays ON.

------------------------------------------------------------------------

# 4. Involution Law

Applying NOT twice returns the original value.

x'' = x

### Examples

NOT(NOT(True)) = True

NOT(NOT(False)) = False

------------------------------------------------------------------------

# 5. Associative Laws

Grouping does not matter when using only the same operator.

(x+y)+z = x+(y+z)

(x·y)·z = x·(y·z)

### Example

(A OR B) OR C = A OR (B OR C)

------------------------------------------------------------------------

# 6. Absorption Laws

Extra terms can sometimes be absorbed.

x + (x·y) = x

x·(x+y) = x

### Example

Student OR (Student AND Athlete)

= Student

------------------------------------------------------------------------

# 7. Uniqueness of Complements

Every Boolean variable has exactly one complement.

If y satisfies

x+y=1

and

x·y=0

then y is uniquely x'.

### Example

The complement of 1 is only 0.

There cannot be another complement.

------------------------------------------------------------------------

# 8. Inversion Law

0' = 1

1' = 0

### Examples

NOT(OFF)=ON

NOT(ON)=OFF

------------------------------------------------------------------------

# 9. De Morgan's Theorems

(x·y)' = x' + y'

(x+y)' = x'·y'

### Examples

NOT(A AND B)

=

NOT A OR NOT B

NOT(A OR B)

=

NOT A AND NOT B

Real-life example:

Door opens if Card AND Fingerprint.

NOT(Open condition)

means

Card missing OR Fingerprint missing.

------------------------------------------------------------------------

# 10. Principle of Duality

Any valid Boolean identity remains valid after:

-   Swap + with ·
-   Swap · with +
-   Swap 0 with 1
-   Swap 1 with 0

### Example

x+0=x

Dual:

x·1=x

Both are valid.

------------------------------------------------------------------------

# 11. Perfect Induction

To prove two Boolean expressions are equivalent, compare every possible
input using a truth table.

### Example

Show

x+y = y+x

Truth table:

  x   y   x+y   y+x
  --- --- ----- -----
  0   0   0     0
  0   1   1     1
  1   0   1     1
  1   1   1     1

Columns match, so the expressions are equivalent.

------------------------------------------------------------------------

# 12. Axiomatic Proof

Instead of using a truth table, simplify expressions using Boolean laws.

### Example

x+(x·y)

= x (Absorption Law)

Another:

x+0

= x (Identity Law)

------------------------------------------------------------------------

# 13. Proof by Contradiction

Assume the statement is false.

If that assumption leads to an impossible result, the original statement
must be true.

### Example

Claim:

"There is no largest positive integer."

Assume there is a largest positive integer n.

Then n+1 is also a positive integer and is larger than n.

Contradiction.

Therefore the assumption is false.

Boolean Example:

Assume x and x' are both 1.

Then

x·x' = 1

But complement law says

x·x' = 0

Contradiction.

Therefore both cannot be 1.

------------------------------------------------------------------------

# Summary Table

  Law             Formula
  --------------- ----------------------------
  Idempotent      x+x=x, x·x=x
  Tautology       x+1=1
  Contradiction   x·0=0
  Involution      x''=x
  Associative     (x+y)+z=x+(y+z)
  Absorption      x+(x·y)=x
  Inversion       0'=1, 1'=0
  De Morgan       (x·y)'=x'+y', (x+y)'=x'·y'
  Duality         Swap +/· and 0/1

# Memory Tricks

-   Idempotent: "Doing it twice changes nothing."
-   Tautology: OR with 1 always gives 1.
-   Contradiction: AND with 0 always gives 0.
-   Double NOT cancels itself.
-   Absorption removes unnecessary terms.
-   De Morgan swaps AND/OR while negating everything.
-   Duality means every Boolean law has a twin.
-   Perfect induction = truth table proof.
-   Axiomatic proof = simplify using laws.
-   Contradiction proof = assume false and reach the impossible.

These laws are the foundation of logic gates, digital circuit design,
CPUs, computer architecture, compiler optimization, and formal
verification.
