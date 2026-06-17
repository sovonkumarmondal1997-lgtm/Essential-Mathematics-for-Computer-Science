# Partial Orders, Total Orders and Comparability

---

# 1. Properties of Relations

## Definition

**Properties of Relations** are rules that describe how elements interact inside a set.

These properties help us classify relations and understand their behavior.

---

## Common Properties

1. Reflexive
2. Symmetric
3. Anti-Symmetric
4. Transitive

Different combinations of these properties create different kinds of relations.

---

## Example

Relation:

≤

on integers

This relation is:

- Reflexive ✔
- Anti-Symmetric ✔
- Transitive ✔

Therefore:

It forms a Partial Order.

---

## Real-Life Example

Think of relation properties as traffic rules that determine how roads (relationships) are allowed to connect places (elements).

---

# 2. Partial Order

## Definition

A **Partial Order** is a relation that satisfies:

1. Reflexive
2. Anti-Symmetric
3. Transitive

simultaneously.

---

## Mathematical Definition

A relation R is a partial order if:

- Reflexive ✔
- Anti-Symmetric ✔
- Transitive ✔

---

## Simple Idea

A partial order creates a structured ordering system.

However, not every pair of elements must be comparable.

---

## Example 1

Relation:

≤

on integers

This relation is:

Reflexive ✔

Anti-Symmetric ✔

Transitive ✔

Partial Order ✔

---

## Example 2

Subset Relation

⊆

between sets

Example:

{1} ⊆ {1,2}

This relation is a partial order.

---

## Example 3

Divisibility Relation

1 divides 2

2 divides 4

1 divides 4

Partial Order ✔

---

# 3. Reflexivity Requirement

## Definition

Every element must relate to itself.

---

## Mathematical Form

For every element a:

aRa

must be true.

---

## Example 1

≤ Relation

5 ≤ 5

True.

Reflexive ✔

---

## Example 2

Divisibility

6 divides 6

True.

Reflexive ✔

---

## Example 3

Subset Relation

A ⊆ A

Always true.

Reflexive ✔

---

## Not Reflexive Example

Relation:

<

5 < 5

False.

Not reflexive.

---

# 4. Transitivity Requirement

## Definition

If:

aRb

and

bRc

then:

aRc

must also hold.

---

## Simple Meaning

You can skip the middle step.

---

## Example 1

≤ Relation

2 ≤ 5

5 ≤ 9

Therefore:

2 ≤ 9

Transitive ✔

---

## Example 2

Divisibility

2 divides 4

4 divides 8

Therefore:

2 divides 8

Transitive ✔

---

## Example 3

Subset Relation

A ⊆ B

B ⊆ C

Therefore:

A ⊆ C

Transitive ✔

---

# 5. Anti-Symmetry Requirement

## Definition

If:

aRb

and

bRa

then:

a = b

must be true.

---

## Simple Meaning

Two different elements cannot point to each other in both directions.

---

## Example 1

≤ Relation

Suppose:

3 ≤ 5

True.

---

5 ≤ 3

False.

No problem.

---

Suppose:

5 ≤ 5

and

5 ≤ 5

Then:

5 = 5

Anti-Symmetric ✔

---

## Example 2

Subset Relation

A ⊆ B

and

B ⊆ A

implies

A = B

Anti-Symmetric ✔

---

## Example 3

Divisibility

4 divides 4

and

4 divides 4

Same element.

Anti-Symmetric ✔

---

# 6. Less Than or Equal To Relation (≤)

## Definition

The relation:

a ≤ b

means:

a is less than or equal to b

---

## Examples

1 ≤ 3

True.

---

4 ≤ 4

True.

---

7 ≤ 2

False.

---

## Why Is It a Partial Order?

### Reflexive

5 ≤ 5

✔

---

### Anti-Symmetric

If:

a ≤ b

and

b ≤ a

Then:

a = b

✔

---

### Transitive

2 ≤ 4

4 ≤ 8

Therefore:

2 ≤ 8

✔

---

## Why Is It Also a Total Order?

Every pair can be compared.

Either:

a ≤ b

or

b ≤ a

Always true.

---

# 7. Divisibility Relation (|)

## Definition

a relates to b when:

a divides b

with no remainder.

Notation:

a | b

---

## Example 1

2 | 8

because:

8 ÷ 2 = 4

---

## Example 2

3 | 12

because:

12 ÷ 3 = 4

---

## Example 3

5 does not divide 12

because remainder exists.

---

## Why Is It a Partial Order?

### Reflexive

5 divides 5

✔

---

### Anti-Symmetric

If:

a divides b

and

b divides a

Then:

a = b

✔

---

### Transitive

2 divides 4

4 divides 8

Therefore:

2 divides 8

✔

---

## Why Is It NOT a Total Order?

Consider:

5 and 7

5 does not divide 7

7 does not divide 5

No comparison possible.

---

Not a total order.

---

# 8. Total Order

## Definition

A **Total Order** is a partial order where every pair of elements can be compared.

---

## Mathematical Condition

For any two elements:

a and b

Either:

aRb

or

bRa

must be true.

---

## Simple Meaning

Every pair has a relationship.

Nothing is left incomparable.

---

## Example 1

≤ on integers

Compare:

3 and 7

3 ≤ 7

---

Compare:

9 and 2

2 ≤ 9

---

Every pair can be compared.

Total Order ✔

---

## Example 2

Age Ranking

People sorted by age.

Every pair can be compared.

Total Order ✔

---

## Example 3

Book Ranking

Rank 1

Rank 2

Rank 3

Every pair has an order.

Total Order ✔

---

# 9. Comparability

## Definition

Two elements are comparable if one is related to the other.

---

## Mathematical Form

For elements:

a and b

Either:

aRb

or

bRa

---

## Example 1

Using ≤

Compare:

4 and 9

4 ≤ 9

Comparable ✔

---

## Example 2

Compare:

10 and 3

3 ≤ 10

Comparable ✔

---

## Example 3

Age Comparison

20 years

25 years

Comparable ✔

---

## Total Orders

Every pair is comparable.

---

# 10. Incomparability

## Definition

Two elements are incomparable when neither direction holds.

---

## Mathematical Form

Neither:

aRb

nor

bRa

is true.

---

## Example 1

Divisibility Relation

5 and 7

5 does not divide 7

7 does not divide 5

Incomparable ✔

---

## Example 2

Sets

A = {1}

B = {2}

---

A ⊆ B

False

---

B ⊆ A

False

---

Incomparable ✔

---

## Example 3

Company Departments

Finance and Marketing

Neither department contains the other.

Incomparable.

---

## Why Important?

Incomparability is what separates partial orders from total orders.

---

# Visual Comparison

## Total Order

Every pair connected.

```
1 ≤ 2 ≤ 3 ≤ 4
```

All comparable.

---

## Partial Order

```
      12
     /  \
    4    6
     \  /
      2
      |
      1
```

Some elements may not be directly comparable.

---

# Quick Comparison Table

| Concept | Meaning |
|----------|----------|
| Partial Order | Reflexive + Anti-Symmetric + Transitive |
| Reflexivity | Every element relates to itself |
| Transitivity | Skip the middle step |
| Anti-Symmetry | Two-way relation implies equality |
| ≤ Relation | Partial Order and Total Order |
| Divisibility Relation | Partial Order but not Total Order |
| Total Order | Every pair is comparable |
| Comparability | One element relates to the other |
| Incomparability | No relation in either direction |

---

# Partial Order vs Total Order

| Feature | Partial Order | Total Order |
|----------|----------|----------|
| Reflexive | ✔ | ✔ |
| Anti-Symmetric | ✔ | ✔ |
| Transitive | ✔ | ✔ |
| Every Pair Comparable | ✘ Not Required | ✔ Required |
| Example | Divisibility | ≤ |

---

# Complete Learning Flow

Sets
↓
Relations
↓
Reflexive Relations
↓
Symmetric Relations
↓
Anti-Symmetric Relations
↓
Transitive Relations
↓
Equivalence Relations
↓
Partial Orders
↓
Comparability
↓
Total Orders
↓
Posets (Partially Ordered Sets)
↓
Lattices
↓
Discrete Mathematics

---

# Key Facts to Remember

1. A partial order requires:
   - Reflexive
   - Anti-Symmetric
   - Transitive

2. Every total order is also a partial order.

3. Not every partial order is a total order.

4. Total orders require comparability between every pair of elements.

5. Divisibility is a classic partial order.

6. ≤ is both a partial order and a total order.

7. Incomparability can exist only in partial orders.

8. Comparability is required for total orders.

9. Partial orders are heavily used in:
   - Database Dependencies
   - Task Scheduling
   - Version Control Systems
   - Graph Theory
   - Data Engineering
   - Distributed Systems

10. Think of a partial order as a hierarchy where some items cannot be directly compared, while a total order is a ranking where every item can be compared with every other item.