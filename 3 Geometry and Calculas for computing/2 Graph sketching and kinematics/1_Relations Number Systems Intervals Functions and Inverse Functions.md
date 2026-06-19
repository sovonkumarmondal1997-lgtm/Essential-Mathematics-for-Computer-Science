# Relations, Number Systems, Intervals, Functions, and Inverse Functions

---

# 1. Relations and Mappings Between Sets

## What is a Set?

A set is simply a collection of distinct objects.

Example:

```text
Students = {Asif A, Asif B, Riya, John}
```

```text
Student IDs = {101, 102, 103, 104}
```

---

# What is a Relation?

A relation describes how elements of one set are connected to elements of another set.

Think of a relation as:

```text
A rule that connects items.
```

---

## Example: Student → Student ID

```text
Students          IDs

Asif A ----------> 101
Asif B ----------> 102
Riya ------------> 103
John ------------> 104
```

This relation connects students with their IDs.

---

## Real-Life Examples of Relations

### Employee → Employee ID

```text
Rahul → E101
Priya → E102
Aman  → E103
```

---

### Country → Capital

```text
India → New Delhi
Japan → Tokyo
France → Paris
```

---

### Product → Price

```text
Laptop → ₹50,000
Phone  → ₹20,000
Tablet → ₹15,000
```

---

# Uniqueness Constraints

To avoid confusion, elements should be uniquely identifiable.

---

## Problem Example

Suppose we have:

```text
Students = {Asif, Asif, John}
```

Which Asif is which?

We cannot tell.

---

## Better Representation

```text
Students = {Asif A, Asif B, John}
```

Now each student is unique.

---

# Why Uniqueness Matters

Without uniqueness:

```text
Incorrect mappings
```

can occur.

Databases, software systems, and mathematical models all require unique identifiers.

---

# Real-Life Example

Banks use:

```text
Account Numbers
```

instead of names because many customers may share the same name.

---

# 2. Number Systems

When defining variables or domains, we must specify what kinds of numbers are allowed.

---

# Natural Numbers (ℕ)

Natural numbers are counting numbers.

```text
1, 2, 3, 4, 5, ...
```

---

## Examples

Number of:

- Students
- Cars
- Books

cannot usually be negative.

---

### Example

```text
Students in class = 35
```

Valid Natural Number.

---

# Integers (ℤ)

Integers include:

- Negative numbers
- Zero
- Positive numbers

```text
..., -3, -2, -1, 0, 1, 2, 3, ...
```

---

## Examples

Temperature:

```text
-5°C
```

```text
0°C
```

```text
20°C
```

---

Bank balance change:

```text
-500
```

```text
+500
```

---

# Rational Numbers (ℚ)

A rational number can be written as:

\[
\frac{p}{q}
\]

where:

```text
p and q are integers
```

and

```text
q ≠ 0
```

---

## Examples

\[
\frac{1}{2}
\]

\[
\frac{3}{4}
\]

\[
-5
\]

Because:

\[
-5=\frac{-5}{1}
\]

---

## Decimal Examples

```text
0.5
```

```text
0.75
```

```text
1.25
```

All are rational.

---

# Real Numbers (ℝ)

Real numbers contain:

- All rational numbers
- All irrational numbers

---

## Irrational Numbers

Cannot be written as a fraction exactly.

Examples:

\[
\pi
\]

\[
\sqrt{2}
\]

\[
e
\]

---

# Real Number Examples

```text
3
```

```text
0.75
```

```text
-7
```

```text
π
```

```text
√2
```

All belong to ℝ.

---

# Number System Hierarchy

```text
Natural Numbers ⊂ Integers ⊂ Rational Numbers ⊂ Real Numbers
```

---

# Visual Representation

```text
Real Numbers (ℝ)

 └─ Rational Numbers (ℚ)

      └─ Integers (ℤ)

           └─ Natural Numbers (ℕ)
```

---

# 3. Interval Notation on a Number Line

## What is an Interval?

An interval represents a continuous range of numbers.

---

# Open Interval

Notation:

\[
(a,b)
\]

Meaning:

\[
a<x<b
\]

---

## Example

\[
(2,8)
\]

Contains:

```text
3
4
5
6
7
```

Does NOT contain:

```text
2
8
```

---

## Number Line

```text
o-----------o
2           8
```

Open circles mean:

```text
Endpoints excluded
```

---

# Closed Interval

Notation:

\[
[a,b]
\]

Meaning:

\[
a \le x \le b
\]

---

## Example

\[
[2,8]
\]

Contains:

```text
2
3
4
5
6
7
8
```

---

## Number Line

```text
●-----------●
2           8
```

Solid circles mean:

```text
Endpoints included
```

---

# Semi-Open Interval

Notation:

\[
(a,b]
\]

or

\[
[a,b)
\]

---

## Example

\[
(2,8]
\]

Contains:

```text
3
4
5
6
7
8
```

But not:

```text
2
```

---

## Number Line

```text
o-----------●
2           8
```

---

# Real-Life Example

Age requirement:

```text
18 ≤ Age < 60
```

Interval:

\[
[18,60)
\]

---

# 4. Definition of a Function

## What is a Function?

A function is a special type of relation.

Every input must have:

```text
Exactly one output.
```

---

# Domain

The set of all valid inputs.

---

## Example

```text
Domain = {1,2,3}
```

---

# Range

The outputs actually reached.

---

## Example

```text
Range = {2,4,6}
```

---

# Function Example

```text
x → 2x
```

Mapping:

```text
1 → 2
2 → 4
3 → 6
```

---

# Diverging Lines Test

A function cannot allow one input to point to multiple outputs.

---

## Valid Function

```text
1 → A
2 → B
3 → C
```

Each input has one output.

---

## Invalid Function

```text
1 → A
1 → B
```

Input:

```text
1
```

has two outputs.

Not a function.

---

# Why?

When we ask:

```text
What is f(1)?
```

We should get only one answer.

---

# Real-Life Example

Student ID system:

```text
Student 101 → Rahul
```

Valid.

---

But:

```text
Student 101 → Rahul
Student 101 → Priya
```

creates ambiguity.

---

# 5. Surjective Functions (Onto)

## Definition

A function is surjective if every element in the target set receives at least one connection.

---

# Example

Domain:

```text
{1,2,3}
```

Codomain:

```text
{A,B,C}
```

Mapping:

```text
1 → A
2 → B
3 → C
```

Every output is used.

Therefore:

```text
Surjective
```

---

# Another Example

```text
1 → A
2 → B
3 → B
```

Codomain:

```text
{A,B}
```

Both outputs are reached.

Still surjective.

---

# Not Surjective Example

```text
1 → A
2 → A
3 → B
```

Codomain:

```text
{A,B,C}
```

C is never reached.

Therefore:

```text
Not Surjective
```

---

# Real-Life Example

Suppose every classroom has at least one student assigned.

Then the assignment is surjective.

No classroom is empty.

---

# 6. Injective Functions (One-to-One)

## Definition

A function is injective if different inputs always produce different outputs.

---

# Rule

No converging lines.

---

# Injective Example

```text
1 → A
2 → B
3 → C
```

All outputs are different.

Injective.

---

# Not Injective Example

```text
1 → A
2 → A
3 → B
```

Inputs:

```text
1 and 2
```

both map to:

```text
A
```

Not injective.

---

# Visual

Injective:

```text
1 → A
2 → B
3 → C
```

---

Not Injective:

```text
1 ↘
     A
2 ↗
```

Two arrows converge.

---

# Real-Life Example

Employee ID system:

```text
E101 → Rahul
E102 → Priya
E103 → Aman
```

Each ID identifies one unique employee.

Injective.

---

# 7. Inverse Functions

## What is an Inverse Function?

An inverse reverses a function.

---

# Example

Original Function

```text
1 → A
2 → B
3 → C
```

Inverse Function

```text
A → 1
B → 2
C → 3
```

---

# Why Must a Function Be Injective?

Suppose:

```text
1 → A
2 → A
```

Now reverse it:

```text
A → 1
A → 2
```

One input:

```text
A
```

has two outputs.

This violates the function rule.

---

# Therefore

Only injective functions can have valid inverses.

---

# Example of Valid Inverse

Original:

```text
f(x)=2x
```

Mappings:

```text
1 → 2
2 → 4
3 → 6
```

---

Inverse:

```text
2 → 1
4 → 2
6 → 3
```

Formula:

\[
f^{-1}(x)=\frac{x}{2}
\]

---

# Real-Life Example

Suppose:

```text
Student ID → Student
```

If every ID belongs to exactly one student, we can reverse it:

```text
Student → Student ID
```

This works because the mapping is injective.

---

# Summary Table

| Concept | Meaning |
|----------|----------|
| Relation | Connection between elements of sets |
| Mapping | Assigning elements from one set to another |
| Natural Numbers (ℕ) | 1, 2, 3, 4, ... |
| Integers (ℤ) | ..., -2, -1, 0, 1, 2, ... |
| Rational Numbers (ℚ) | Fractions like 1/2, 3/4 |
| Real Numbers (ℝ) | Rational + Irrational numbers |
| Open Interval | (a,b) excludes endpoints |
| Closed Interval | [a,b] includes endpoints |
| Function | Each input has exactly one output |
| Domain | Set of inputs |
| Range | Outputs reached |
| Surjective | Every output is used |
| Injective | Different inputs → different outputs |
| Inverse Function | Reverses a function |
| Condition for Inverse | Function must be injective |

---

# Final Key Idea

Relations and functions are mathematical tools for describing connections between objects.

```text
Relation → General Connection
```

```text
Function → Special Relation
```

A function requires:

```text
One input → One output
```

Understanding:

- Number systems
- Intervals
- Domains
- Ranges
- Injective functions
- Surjective functions
- Inverse functions

forms the foundation of discrete mathematics, databases, programming, algorithms, data engineering, machine learning, and computer science.
