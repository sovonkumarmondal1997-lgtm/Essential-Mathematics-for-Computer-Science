# Set Theory - Part 4

---

# De Morgan's Laws

## Definition

**De Morgan's Laws** show how complements interact with union and intersection operations.

There are two laws:

### First Law

```text
(A ∪ B)' = A' ∩ B'
```

Meaning:

```text
The complement of a union equals the intersection of the complements.
```

---

### Second Law

```text
(A ∩ B)' = A' ∪ B'
```

Meaning:

```text
The complement of an intersection equals the union of the complements.
```

---

## Example 1 (First Law)

Given:

```text
U = {1,2,3,4,5,6}

A = {1,2,3}

B = {3,4}
```

Step 1:

```text
A ∪ B = {1,2,3,4}
```

Step 2:

```text
(A ∪ B)' = {5,6}
```

Now find complements:

```text
A' = {4,5,6}

B' = {1,2,5,6}
```

Step 3:

```text
A' ∩ B' = {5,6}
```

Therefore:

```text
(A ∪ B)' = A' ∩ B'
```

Verified.

---

## Example 2 (Second Law)

Given:

```text
U = {1,2,3,4,5,6}

A = {1,2,3}

B = {2,3,4}
```

Step 1:

```text
A ∩ B = {2,3}
```

Step 2:

```text
(A ∩ B)' = {1,4,5,6}
```

Now:

```text
A' = {4,5,6}

B' = {1,5,6}
```

Step 3:

```text
A' ∪ B' = {1,4,5,6}
```

Therefore:

```text
(A ∩ B)' = A' ∪ B'
```

Verified.

---

# Commutativity

## Definition

An operation is **commutative** if changing the order does not change the result.

General Form:

```text
A ★ B = B ★ A
```

---

# Union is Commutative

## Formula

```text
A ∪ B = B ∪ A
```

### Example

```text
A = {1,2}

B = {2,3}
```

Then:

```text
A ∪ B = {1,2,3}

B ∪ A = {1,2,3}
```

Hence:

```text
A ∪ B = B ∪ A
```

---

# Intersection is Commutative

## Formula

```text
A ∩ B = B ∩ A
```

### Example

```text
A = {1,2,3}

B = {2,3,4}
```

Then:

```text
A ∩ B = {2,3}

B ∩ A = {2,3}
```

Hence:

```text
A ∩ B = B ∩ A
```

---

# Symmetric Difference is Commutative

## Formula

```text
A △ B = B △ A
```

### Example

```text
A = {1,2,3}

B = {3,4,5}
```

Then:

```text
A △ B = {1,2,4,5}

B △ A = {1,2,4,5}
```

Hence:

```text
A △ B = B △ A
```

---

# Set Difference is NOT Commutative

## Formula

```text
A − B ≠ B − A
```

### Example

```text
A = {1,2,3}

B = {3,4,5}
```

Then:

```text
A − B = {1,2}
```

But:

```text
B − A = {4,5}
```

Since:

```text
{1,2} ≠ {4,5}
```

Therefore:

```text
A − B ≠ B − A
```

---

# Associativity

## Definition

An operation is **associative** if changing the grouping does not change the result.

General Form:

```text
(A ★ B) ★ C = A ★ (B ★ C)
```

---

## Simple Number Example

Addition:

```text
(2 + 3) + 4 = 2 + (3 + 4)

5 + 4 = 2 + 7

9 = 9
```

Therefore addition is associative.

---

# Union is Associative

## Formula

```text
(A ∪ B) ∪ C = A ∪ (B ∪ C)
```

### Example

```text
A = {1}
B = {2}
C = {3}
```

Left Side:

```text
(A ∪ B) ∪ C

= {1,2} ∪ {3}

= {1,2,3}
```

Right Side:

```text
A ∪ (B ∪ C)

= {1} ∪ {2,3}

= {1,2,3}
```

Therefore:

```text
(A ∪ B) ∪ C = A ∪ (B ∪ C)
```

---

# Intersection is Associative

## Formula

```text
(A ∩ B) ∩ C = A ∩ (B ∩ C)
```

### Example

```text
A = {1,2,3}

B = {2,3,4}

C = {3,4,5}
```

Left Side:

```text
(A ∩ B) ∩ C

= {2,3} ∩ {3,4,5}

= {3}
```

Right Side:

```text
A ∩ (B ∩ C)

= {1,2,3} ∩ {3,4}

= {3}
```

Therefore associative.

---

# Symmetric Difference is Associative

## Formula

```text
(A △ B) △ C = A △ (B △ C)
```

### Example

```text
A = {1}
B = {2}
C = {3}
```

Left Side:

```text
(A △ B) △ C

= {1,2} △ {3}

= {1,2,3}
```

Right Side:

```text
A △ (B △ C)

= {1} △ {2,3}

= {1,2,3}
```

Therefore associative.

---

# Set Difference is NOT Associative

## Formula

```text
(A − B) − C ≠ A − (B − C)
```

### Example

```text
A = {1,2,3}

B = {2}

C = {3}
```

Left Side:

```text
(A − B) − C

= {1,3} − {3}

= {1}
```

Right Side:

```text
A − (B − C)

= {1,2,3} − {2}

= {1,3}
```

Since:

```text
{1} ≠ {1,3}
```

Therefore:

```text
(A − B) − C ≠ A − (B − C)
```

---

# Distributivity

## Definition

An operation is **distributive** if one operation can be distributed over another operation.

General Form:

```text
A ★ (B ◇ C)
=
(A ★ B) ◇ (A ★ C)
```

---

## Simple Number Example

Multiplication over Addition:

```text
2 × (3 + 4)

= 2 × 7

= 14
```

and

```text
(2 × 3) + (2 × 4)

= 6 + 8

= 14
```

Therefore multiplication distributes over addition.

---

# Union is Distributive Over Intersection

## Formula

```text
A ∪ (B ∩ C)

=
(A ∪ B) ∩ (A ∪ C)
```

### Example

```text
A = {1}

B = {1,2}

C = {1,3}
```

Left Side:

```text
B ∩ C = {1}

A ∪ {1}

= {1}
```

Right Side:

```text
(A ∪ B) ∩ (A ∪ C)

= {1,2} ∩ {1,3}

= {1}
```

Verified.

---

# Intersection is Distributive Over Union

## Formula

```text
A ∩ (B ∪ C)

=
(A ∩ B) ∪ (A ∩ C)
```

### Example

```text
A = {1,2}

B = {2,3}

C = {1,4}
```

Left Side:

```text
B ∪ C

= {1,2,3,4}

A ∩ (B ∪ C)

= {1,2}
```

Right Side:

```text
(A ∩ B)

= {2}

(A ∩ C)

= {1}

{2} ∪ {1}

= {1,2}
```

Verified.

---

# Partition of a Set

## Definition

A **partition** of a set is a collection of non-empty subsets that:

1. Do not overlap.
2. Together contain all elements of the original set.

---

## Example

Given:

```text
A = {1,2,3,4,5,6}
```

Partition:

```text
P1 = {1,2}

P2 = {3,4}

P3 = {5,6}
```

Properties:

```text
P1 ∩ P2 = ∅

P2 ∩ P3 = ∅

P1 ∩ P3 = ∅
```

and

```text
P1 ∪ P2 ∪ P3 = A
```

Therefore these subsets form a partition.

---

# Disjoint Sets

## Definition

Two sets are **disjoint** if they have no common element.

### Formula

```text
A ∩ B = ∅
```

---

## Example 1

```text
A = {1,2,3}

B = {4,5,6}
```

Intersection:

```text
A ∩ B = ∅
```

Therefore A and B are disjoint.

---

## Example 2

```text
A = {a,b}

B = {x,y,z}
```

Intersection:

```text
A ∩ B = ∅
```

Therefore A and B are disjoint.

---

# Quick Revision Table

| Property | Formula |
|-----------|----------|
| De Morgan's Law 1 | (A ∪ B)' = A' ∩ B' |
| De Morgan's Law 2 | (A ∩ B)' = A' ∪ B' |
| Commutative Union | A ∪ B = B ∪ A |
| Commutative Intersection | A ∩ B = B ∩ A |
| Commutative Symmetric Difference | A △ B = B △ A |
| Non-Commutative Difference | A − B ≠ B − A |
| Associative Union | (A ∪ B) ∪ C = A ∪ (B ∪ C) |
| Associative Intersection | (A ∩ B) ∩ C = A ∩ (B ∩ C) |
| Associative Symmetric Difference | (A △ B) △ C = A △ (B △ C) |
| Non-Associative Difference | (A − B) − C ≠ A − (B − C) |
| Union Distributes Over Intersection | A ∪ (B ∩ C) = (A ∪ B) ∩ (A ∪ C) |
| Intersection Distributes Over Union | A ∩ (B ∪ C) = (A ∩ B) ∪ (A ∩ C) |
| Disjoint Sets | A ∩ B = ∅ |
| Partition of Set | Non-overlapping subsets whose union equals the original set |