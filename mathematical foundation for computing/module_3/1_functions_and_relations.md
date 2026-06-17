# Functions, Relations, Sets, Domain, Co-domain, Range and Related Concepts

---

# 1. Set

## Definition
A **Set** is a collection of distinct objects, numbers, letters, words, or any items grouped together.

Think of a set as a **container** that stores unique items.

---

## Examples

### Example 1: Number Set

A = {1, 2, 3, 4, 5}

This set contains five numbers.

---

### Example 2: Letter Set

B = {a, b, c, d}

This set contains four letters.

---

### Example 3: Fruit Set

Fruits = {Apple, Mango, Banana}

This set contains three fruits.

---

## Real-Life Example

A classroom contains students:

Students = {Rahul, Priya, Amit, Neha}

This collection of students forms a set.

---

# 2. Mathematical Relation

## Definition

A **Relation** is a connection between elements of two sets.

A relation tells us which elements are linked to which.

---

## Example

Let:

A = {1, 2, 3}

B = {a, b, c}

Relation:

R = {(1,a), (2,b), (3,c)}

Meaning:

- 1 is related to a
- 2 is related to b
- 3 is related to c

---

## Another Example

Students and Subjects:

Students = {Rahul, Priya}

Subjects = {Math, Science}

Relation:

R = {
(Rahul, Math),
(Rahul, Science),
(Priya, Science)
}

This relation shows which subjects each student studies.

---

## Important

Every function is a relation.

But every relation is NOT a function.

---

# 3. Function

## Definition

A **Function** is a special type of relation where:

Each input has exactly ONE output.

---

## Function Machine Analogy

Imagine a machine:

Input → Machine → Output

Input: 2

Rule: Multiply by 3

Output: 6

---

## Example

f(x) = 2x

Inputs:

1 → 2

2 → 4

3 → 6

Table:

| Input | Output |
|---------|---------|
| 1 | 2 |
| 2 | 4 |
| 3 | 6 |

Every input gives exactly one output.

Therefore it is a function.

---

## Non-Function Example

1 → A

1 → B

Input 1 produces two outputs.

Not a function.

---

# 4. Domain (Df)

## Definition

The **Domain** is the set of all possible inputs of a function.

---

## Example

Function:

f(x)=x+2

Inputs:

1,2,3,4

Domain:

Df = {1,2,3,4}

---

## Real-Life Example

Age → Ticket Price

Possible ages:

{5,10,15,20}

These ages form the domain.

---

# 5. Co-Domain (co-Df)

## Definition

The **Co-domain** is the set of all allowed or possible outputs.

Think of it as the "output container".

---

## Example

f(x)=x²

Domain:

{1,2,3}

Co-domain:

{1,4,9,16,25}

Even if some outputs never appear, they may still belong to the co-domain.

---

## Real-Life Example

Exam Grades

Possible grades:

{A,B,C,D,F}

This is the co-domain.

Not every grade must occur.

---

# 6. Range (Rf)

## Definition

The **Range** is the set of actual outputs produced.

Range is always a subset of the co-domain.

---

## Example

f(x)=x²

Domain:

{1,2,3}

Outputs:

1² = 1

2² = 4

3² = 9

Range:

Rf = {1,4,9}

---

## Comparison

Co-domain:

{1,4,9,16,25}

Range:

{1,4,9}

Range is smaller.

---

# 7. Image

## Definition

The **Image** is the output corresponding to a specific input.

---

## Example

f(x)=x²

Input:

x=3

Output:

f(3)=9

Image of 3 is 9.

---

## More Examples

f(2)=4

Image of 2 = 4

f(5)=25

Image of 5 = 25

---

# 8. Pre-image / Antecedent

## Definition

The **Pre-image** is the input that produces a given output.

---

## Example

f(x)=x²

Output:

9

Which input produced 9?

Answer:

3 and -3

Pre-image of 9:

{3,-3}

---

## Example

f(x)=2x

Output:

10

Input:

5

Pre-image of 10:

5

---

# 9. Function Mapping Notation

## Definition

The notation

f : A → B

means:

Function f maps elements from set A to set B.

---

## Example

f : {1,2,3} → {2,4,6}

Rule:

f(x)=2x

Mappings:

1 → 2

2 → 4

3 → 6

---

## Reading

f : A → B

Read as:

"Function f maps A into B."

---

# 10. Uniqueness of Output Constraint

## Definition

A valid function cannot assign multiple outputs to one input.

One input → One output only.

---

## Valid Example

1 → A

2 → B

3 → C

Valid function.

---

## Invalid Example

1 → A

1 → B

Input 1 has two outputs.

Not a function.

---

## Real-Life Example

Student ID → Student Name

One ID should identify exactly one student.

Otherwise confusion occurs.

---

# 11. Completeness of Input Constraint

## Definition

Every element of the domain must have an output.

No input can be left unmapped.

---

## Valid Example

Domain:

{1,2,3}

Mappings:

1 → A

2 → B

3 → C

All inputs mapped.

Function is valid.

---

## Invalid Example

Domain:

{1,2,3}

Mappings:

1 → A

2 → B

3 has no output.

Not a valid function.

---

## Real-Life Example

Employee ID → Salary

Every employee ID must have a salary.

Otherwise the function is incomplete.

---

# 12. Absolute Value Function

## Definition

Absolute value removes the sign.

It measures distance from zero.

Notation:

|x|

---

## Rule

|5| = 5

|-5| = 5

---

## Examples

| Input | Output |
|---------|---------|
| 5 | 5 |
| -5 | 5 |
| 8 | 8 |
| -8 | 8 |
| 0 | 0 |

---

## Real-Life Example

Temperature difference:

+10°C and -10°C

Both are 10 units away from zero.

Absolute value:

10

---

# 13. Real-Valued Function

## Definition

A function whose inputs and outputs are real numbers.

---

## Example

f(x)=x+1

Inputs:

1.5

2.7

-3.8

Outputs:

2.5

3.7

-2.8

All are real numbers.

---

## Example

f(x)=x²

Input:

2.5

Output:

6.25

Still real-valued.

---

## Real-Life Example

Height → Weight

Both can be represented using real numbers.

---

# 14. Quadratic Mapping

## Definition

A quadratic mapping is a function involving x².

General form:

f(x)=ax²+bx+c

where a ≠ 0

---

## Example 1

f(x)=x²+1

Inputs:

| x | Output |
|----|----|
| 0 | 1 |
| 1 | 2 |
| 2 | 5 |
| 3 | 10 |

---

## Example 2

f(x)=x²

| x | Output |
|----|----|
| -2 | 4 |
| -1 | 1 |
| 0 | 0 |
| 1 | 1 |
| 2 | 4 |

---

## Real-Life Example

The path of a thrown ball often follows a quadratic curve.

Engineers and scientists use quadratic functions to model motion.

---

# Complete Relationship Diagram

Set
↓
Relation
↓
Function
↓
Domain (Inputs)
↓
Mapping Rule
↓
Image (Output for One Input)
↓
Range (All Actual Outputs)
↓
Co-domain (All Allowed Outputs)

Important:

Range ⊆ Co-domain

Every Function is a Relation

Not Every Relation is a Function

Function Rules:

1. Every input must have an output.
2. One input cannot have multiple outputs.
3. Multiple inputs can share the same output.

Example:

f(x)=x²

-2 → 4

2 → 4

This is still a valid function because each input has only one output.
