# Set Theory - Part 3

---

# Universal Set

## Definition
The **universal set** is the set that contains all elements under consideration in a particular discussion.

### Symbol

```text
U
```

---

## Example

Suppose we are discussing numbers from 1 to 10.

```text
U = {1,2,3,4,5,6,7,8,9,10}
```

Let

```text
A = {2,4,6,8,10}
```

Then:

```text
A ⊆ U
```

because every element of A belongs to the universal set.

---

## Another Example

Universal set of English vowels and consonants:

```text
U = {a,b,c,d,e,f,g,...,z}
```

Vowels:

```text
V = {a,e,i,o,u}
```

Then:

```text
V ⊆ U
```

---

# Venn Diagram

## Definition

A **Venn Diagram** is a visual representation of sets using circles inside a rectangle representing the universal set.

### Components

```text
Rectangle → Universal Set (U)

Circle → A Set

Overlapping Region → Common Elements
```

---

# Venn Diagram Example 1

Let

```text
U = {1,2,3,4,5,6,7,8}

A = {1,2,3,4}

B = {3,4,5,6}
```

Venn Diagram Representation

```text
+-----------------------+
|                       |
|      ( A )            |
|    1  2 |3 4|         |
|         |   |         |
|         |   |         |
|         |5 6| ( B )   |
|                       |
+-----------------------+
```

Common elements:

```text
A ∩ B = {3,4}
```

---

# Venn Diagram Example 2

Students who like:

```text
A = Cricket

B = Football
```

Suppose:

```text
A = {Rahul, Amit, Raj}

B = {Raj, Amit, John}
```

Then:

```text
A ∩ B = {Raj, Amit}
```

Meaning:

```text
Raj and Amit like both sports.
```

---

# Complement of a Set

## Definition

The **complement** of a set A is the set of all elements in the universal set that are not in A.

### Symbol

```text
A'
```

or

```text
Aᶜ
```

---

## Formula

```text
A' = U − A
```

---

## Example 1

Given:

```text
U = {1,2,3,4,5,6,7,8,9,10}

A = {2,4,6,8,10}
```

Complement:

```text
A' = {1,3,5,7,9}
```

---

## Example 2

Given:

```text
U = {a,b,c,d,e,f}

A = {a,c,e}
```

Complement:

```text
A' = {b,d,f}
```

---

# Venn Diagram of Set Union

## Meaning in Simple Terms

Take everything that belongs to A or B or both.

### Symbol

```text
A ∪ B
```

---

## Example

```text
A = {1,2,3}

B = {3,4,5}
```

Union:

```text
A ∪ B = {1,2,3,4,5}
```

---

## Venn Diagram Interpretation

```text
      A           B

    (#####|#####)
    (#####|#####)

Shade:
- Entire A
- Entire B
- Overlapping part
```

Think:

```text
"Take everything inside both circles."
```

---

# Venn Diagram of Set Intersection

## Meaning in Simple Terms

Take only the elements common to both sets.

### Symbol

```text
A ∩ B
```

---

## Example

```text
A = {1,2,3}

B = {2,3,4}
```

Intersection:

```text
A ∩ B = {2,3}
```

---

## Venn Diagram Interpretation

```text
      A       B

      (   |   )
      (###|###)

Shade:
Only the overlapping region
```

Think:

```text
"Take only what both sets share."
```

---

# Venn Diagram of Set Difference

## Meaning in Simple Terms

Take elements that belong to A but not to B.

### Symbol

```text
A − B
```

---

## Example

```text
A = {1,2,3,4}

B = {3,4,5}
```

Difference:

```text
A − B = {1,2}
```

---

## Venn Diagram Interpretation

```text
      A         B

    (####|     )
    (####|     )

Shade:
Only A's non-overlapping region
```

Think:

```text
"Keep A only and remove common elements."
```

---

# Venn Diagram of B − A

## Example

```text
A = {1,2,3,4}

B = {3,4,5}
```

Difference:

```text
B − A = {5}
```

---

## Venn Diagram Interpretation

```text
      A         B

         ( |####)
         ( |####)

Shade:
Only B's non-overlapping region
```

Think:

```text
"Keep B only and remove common elements."
```

---

# Venn Diagram of Symmetric Difference

## Meaning in Simple Terms

Take elements that belong to exactly one set, but not both.

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

## Example

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

## Venn Diagram Interpretation

```text
      A         B

    (####|####)
    (####|####)

      Common
      region
      NOT shaded
```

Shade:

```text
A only region
+
B only region
```

Do NOT Shade:

```text
A ∩ B
```

Think:

```text
"Take what is unique to each set."
```

---

# Quick Visual Summary

## Union

```text
Take EVERYTHING

A ∪ B
```

```text
[ A ] + [ B ]
```

---

## Intersection

```text
Take ONLY COMMON PART

A ∩ B
```

```text
Common Elements Only
```

---

## Difference

```text
Take A and remove common elements

A − B
```

```text
Only A Side
```

---

## Symmetric Difference

```text
Take unique elements from both sets

A △ B
```

```text
A Only + B Only
```

---

# Important Formulas

```text
A' = U − A
```

```text
A ∪ B
```

```text
A ∩ B
```

```text
A − B
```

```text
B − A
```

```text
A △ B = (A − B) ∪ (B − A)
```

---

# One-Line Revision Sheet

| Concept | Symbol | Meaning |
|----------|---------|----------|
| Universal Set | U | Contains all elements under discussion |
| Complement | A' or Aᶜ | Elements in U but not in A |
| Union | ∪ | Everything in A or B or both |
| Intersection | ∩ | Elements common to both sets |
| Difference | − | Elements in first set but not second |
| Symmetric Difference | △ or ⊕ | Elements in exactly one set |
| Venn Diagram | — | Visual representation of sets using circles |