# Set Theory - Part 2

---

# Set Listing Method (Roster Method)

## Definition
The **set listing method** is a way of representing a set by explicitly listing all its elements inside curly braces `{}`.

### Example
```text
A = {1, 2, 3, 4, 5}
```

Here, all elements of set A are listed one by one.

### Another Example
```text
V = {a, e, i, o, u}
```

### Another Example
```text
D = {Monday, Tuesday, Wednesday, Thursday, Friday}
```

---

# Set Builder Notation

## Definition
**Set builder notation** is a method of representing a set by describing a property that all elements of the set satisfy.

### General Form

```text
A = {x | condition on x}
```

Read as:

```text
A is the set of all x such that x satisfies the given condition.
```

---

## Example 1: Even Numbers

```text
E = {x | x is an even positive integer}
```

Roster Form:

```text
E = {2, 4, 6, 8, 10, ...}
```

---

## Example 2: Multiples of 5

```text
M = {x | x is a multiple of 5}
```

Roster Form:

```text
M = {5, 10, 15, 20, 25, ...}
```

---

## Example 3: Natural Numbers Less Than 6

```text
N = {x | x ∈ N and x < 6}
```

Roster Form:

```text
N = {1, 2, 3, 4, 5}
```

---

# Power Set

## Definition
The **power set** of a set A is the set containing all possible subsets of A.

### Symbol

```text
P(A)
```

or

```text
2ᴬ
```

---

## Example 1

Given

```text
A = {1}
```

Subsets:

```text
∅
{1}
```

Power Set:

```text
P(A) = {∅, {1}}
```

---

## Example 2

Given

```text
B = {1, 2}
```

Subsets:

```text
∅
{1}
{2}
{1,2}
```

Power Set:

```text
P(B) = {∅, {1}, {2}, {1,2}}
```

---

## Example 3

Given

```text
C = {a,b,c}
```

Subsets:

```text
∅
{a}
{b}
{c}
{a,b}
{a,c}
{b,c}
{a,b,c}
```

Power Set:

```text
P(C) =
{
∅,
{a},
{b},
{c},
{a,b},
{a,c},
{b,c},
{a,b,c}
}
```

---

# Cardinality of a Power Set

## Definition
The number of elements in a power set is called the **cardinality of the power set**.

### Formula

If

```text
|A| = n
```

then

```text
|P(A)| = 2ⁿ
```

---

## Example 1

```text
A = {1}
```

Cardinality:

```text
|A| = 1
```

Power Set Cardinality:

```text
|P(A)| = 2¹ = 2
```

Subsets:

```text
∅
{1}
```

---

## Example 2

```text
B = {1,2}
```

Cardinality:

```text
|B| = 2
```

Power Set Cardinality:

```text
|P(B)| = 2² = 4
```

Subsets:

```text
∅
{1}
{2}
{1,2}
```

---

## Example 3

```text
C = {a,b,c}
```

Cardinality:

```text
|C| = 3
```

Power Set Cardinality:

```text
|P(C)| = 2³ = 8
```

Subsets:

```text
∅
{a}
{b}
{c}
{a,b}
{a,c}
{b,c}
{a,b,c}
```

---

# Set Union

## Definition
The **union** of two sets contains all elements that belong to either set or both sets.

### Symbol

```text
∪
```

---

## Example 1

```text
A = {1,2,3}
B = {3,4,5}
```

Union:

```text
A ∪ B = {1,2,3,4,5}
```

---

## Example 2

```text
X = {a,b,c}
Y = {c,d,e}
```

Union:

```text
X ∪ Y = {a,b,c,d,e}
```

---

## Union Membership Table

| A | B | A ∪ B |
|---|---|--------|
| 0 | 0 | 0 |
| 0 | 1 | 1 |
| 1 | 0 | 1 |
| 1 | 1 | 1 |

Where:

```text
1 = Element belongs to the set
0 = Element does not belong to the set
```

---

# Set Intersection

## Definition
The **intersection** of two sets contains only the elements common to both sets.

### Symbol

```text
∩
```

---

## Example 1

```text
A = {1,2,3}
B = {2,3,4}
```

Intersection:

```text
A ∩ B = {2,3}
```

---

## Example 2

```text
X = {a,b,c}
Y = {b,c,d}
```

Intersection:

```text
X ∩ Y = {b,c}
```

---

## Intersection Membership Table

| A | B | A ∩ B |
|---|---|--------|
| 0 | 0 | 0 |
| 0 | 1 | 0 |
| 1 | 0 | 0 |
| 1 | 1 | 1 |

---

# Set Difference

## Definition
The **difference** of two sets A and B is the set of elements that belong to A but not to B.

### Symbol

```text
A − B
```

---

## Example 1

```text
A = {1,2,3,4}
B = {3,4,5}
```

Difference:

```text
A − B = {1,2}
```

---

## Example 2

```text
X = {a,b,c,d}
Y = {b,d,e}
```

Difference:

```text
X − Y = {a,c}
```

---

## Set Difference Membership Table

| A | B | A − B |
|---|---|--------|
| 0 | 0 | 0 |
| 0 | 1 | 0 |
| 1 | 0 | 1 |
| 1 | 1 | 0 |

---

# Set Symmetric Difference

## Definition
The **symmetric difference** of two sets contains elements that belong to exactly one of the sets but not both.

### Symbol

```text
A △ B
```

or

```text
A ⊕ B
```

---

## Formula

```text
A △ B = (A − B) ∪ (B − A)
```

---

## Example 1

```text
A = {1,2,3}
B = {3,4,5}
```

Difference Parts:

```text
A − B = {1,2}
B − A = {4,5}
```

Symmetric Difference:

```text
A △ B = {1,2,4,5}
```

---

## Example 2

```text
X = {a,b,c}
Y = {b,c,d}
```

Difference Parts:

```text
X − Y = {a}
Y − X = {d}
```

Symmetric Difference:

```text
X △ Y = {a,d}
```

---

## Symmetric Difference Membership Table

| A | B | A △ B |
|---|---|--------|
| 0 | 0 | 0 |
| 0 | 1 | 1 |
| 1 | 0 | 1 |
| 1 | 1 | 0 |

---

# Quick Summary Table

| Operation | Symbol | Meaning |
|------------|---------|---------|
| Union | ∪ | Elements in A or B or both |
| Intersection | ∩ | Elements common to A and B |
| Difference | − | Elements in A but not in B |
| Symmetric Difference | △ | Elements in exactly one set |
| Power Set | P(A) | Set of all subsets of A |
| Cardinality | \|A\| | Number of elements in A |
| Power Set Cardinality | \|P(A)\| | Number of subsets of A = 2ⁿ |

---

# Important Formulae

```text
|P(A)| = 2ⁿ
```

```text
A △ B = (A − B) ∪ (B − A)
```

```text
A ∩ B ⊆ A
```

```text
A ∩ B ⊆ B
```

```text
A ⊆ A ∪ B
```

```text
B ⊆ A ∪ B
```