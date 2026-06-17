# Relation Representation, Matrices and Directed Graphs

---

# 1. Relation Representation

## Definition

A **Relation Representation** is a method used to organize, visualize, and understand relations.

Since a relation is simply a collection of ordered pairs, mathematicians use different tools to represent it clearly.

---

## Common Representation Methods

1. Ordered Pair Representation
2. Table Representation
3. Matrix Representation
4. Directed Graph (Digraph) Representation

---

## Example

Set:

A = {1,2,3}

Relation:

R = {(1,2),(2,3)}

Can be represented as:

### Ordered Pairs

{(1,2),(2,3)}

### Matrix

|   |1|2|3|
|---|---|---|---|
|1|0|1|0|
|2|0|0|1|
|3|0|0|0|

### Digraph

1 → 2 → 3

---

## Real-Life Example

A social network can be represented by:

- Friend lists
- Tables
- Adjacency matrices
- Graphs

All represent the same relation.

---

# 2. Zero-One Matrix / Logical Matrix (MR)

## Definition

A **Zero-One Matrix** represents a relation using only:

0 = Not Related

1 = Related

---

## Construction Rule

If:

(ai,bj) ∈ R

place:

1

Otherwise:

0

---

## Example

A = {1,2,3}

Relation:

R = {(1,2),(2,3)}

Matrix:

|   |1|2|3|
|---|---|---|---|
|1|0|1|0|
|2|0|0|1|
|3|0|0|0|

---

## Interpretation

Row 1 Column 2 = 1

Means:

(1,2) belongs to R

---

Row 3 Column 1 = 0

Means:

(3,1) does not belong to R

---

## Real-Life Example

Employee Access Matrix

1 = Has Access

0 = No Access

---

# 3. Cardinality (na, nb)

## Definition

**Cardinality** means the number of elements in a set.

Notation:

|A|

or

na

---

## Example 1

A = {1,2,3}

Cardinality:

|A| = 3

---

## Example 2

B = {a,b,c,d,e}

Cardinality:

|B| = 5

---

## Example 3

Students:

{Rahul, Priya, Amit, Neha}

Cardinality:

4

---

## Matrix Connection

If:

|A| = 3

|B| = 4

Then:

A × B matrix size:

3 × 4

---

# 4. Leading Diagonal / Main Diagonal

## Definition

The main diagonal runs from:

Top Left

↓

Bottom Right

of a square matrix.

---

## Example

Matrix:

|   |1|2|3|
|---|---|---|---|
|1|1|0|0|
|2|0|1|0|
|3|0|0|1|

Main Diagonal Entries:

1

1

1

---

## Another Example

|   |1|2|3|
|---|---|---|---|
|1|0|1|0|
|2|0|0|1|
|3|1|0|0|

Diagonal:

0

0

0

---

## Why Important?

The diagonal tells us whether elements are related to themselves.

---

# 5. Strict Inequality Matrix Profile

## Definition

The relation:

x < y

never allows:

x < x

Therefore:

No element relates to itself.

---

## Example

A = {1,2,3}

Relation:

<

Valid pairs:

(1,2)

(1,3)

(2,3)

---

## Matrix

|   |1|2|3|
|---|---|---|---|
|1|0|1|1|
|2|0|0|1|
|3|0|0|0|

---

## Diagonal

0

0

0

All zeros.

---

## Key Property

Strict inequality matrices always have:

Zero diagonal.

---

# 6. Reflexive Matrix Profile

## Definition

A relation is reflexive when every element relates to itself.

---

## Example

Relation:

≤

on

A = {1,2,3}

---

Valid pairs include:

(1,1)

(2,2)

(3,3)

---

## Matrix

|   |1|2|3|
|---|---|---|---|
|1|1|1|1|
|2|0|1|1|
|3|0|0|1|

---

## Diagonal

1

1

1

All ones.

---

## Key Property

Reflexive relations have:

Diagonal = All Ones

---

# 7. Relational Union (R ∪ S)

## Definition

The union combines all ordered pairs appearing in either relation.

---

## Formula

R ∪ S

=

All pairs in R or S or both

---

## Example

R = {(1,2),(2,3)}

S = {(2,3),(3,1)}

---

Union:

R ∪ S

=

{(1,2),(2,3),(3,1)}

---

## Real-Life Example

Students taking:

Math

OR

Science

Union gives students taking at least one subject.

---

# 8. Relational Intersection (R ∩ S)

## Definition

The intersection contains only pairs appearing in both relations.

---

## Example

R = {(1,2),(2,3)}

S = {(2,3),(3,1)}

---

Intersection:

R ∩ S

=

{(2,3)}

---

## Real-Life Example

Students taking:

Math

AND

Science

Only common students remain.

---

# 9. Boolean Matrix Arithmetic

## Definition

Operations performed on matrices containing only:

0 and 1

using logical rules.

---

## Logical Values

0 = False

1 = True

---

## Common Operations

OR

AND

NOT

---

## Example

Matrix A:

|1|0|
|---|---|
|0|1|

Matrix B:

|0|1|
|---|---|
|1|0|

Boolean operations combine them logically.

---

# 10. Join Operation (∨)

## Definition

Join means:

Logical OR

Used for relational union.

---

## OR Rule

| A | B | A ∨ B |
|---|---|---|
|0|0|0|
|0|1|1|
|1|0|1|
|1|1|1|

---

## Example

A

|1|0|
|---|---|
|0|1|

B

|0|1|
|---|---|
|1|0|

---

A ∨ B

|1|1|
|---|---|
|1|1|

---

## Meaning

If either relation exists:

Result = 1

---

# 11. Meet Operation (∧)

## Definition

Meet means:

Logical AND

Used for relational intersection.

---

## AND Rule

| A | B | A ∧ B |
|---|---|---|
|0|0|0|
|0|1|0|
|1|0|0|
|1|1|1|

---

## Example

A

|1|0|
|---|---|
|1|1|

B

|1|1|
|---|---|
|0|1|

---

A ∧ B

|1|0|
|---|---|
|0|1|

---

## Meaning

Both relations must exist.

---

# 12. Directed Graph / Digraph

## Definition

A digraph represents relations using:

Vertices (Nodes)

+

Directed Edges (Arrows)

---

## Example

Set:

{1,2,3}

Relation:

{(1,2),(2,3)}

---

Digraph:

1 → 2 → 3

---

## Real-Life Examples

- Road maps
- Social networks
- Website links
- Computer networks

---

# 13. Vertex / Node

## Definition

A vertex represents an element of the set.

---

## Example

Set:

{A,B,C}

Vertices:

A

B

C

---

## Example

Students:

{Rahul, Priya}

Each student becomes a node.

---

## Real-Life Example

Cities on a map are vertices.

---

# 14. Directed Edge / Arc

## Definition

An arrow from x to y indicates:

x is related to y

---

## Example

Relation:

(1,2)

Draw:

1 → 2

---

## Example

(3,5)

Draw:

3 → 5

---

## Real-Life Example

Instagram Follow

Rahul follows Priya

Rahul → Priya

---

# 15. Divisibility Relation

## Definition

x is related to y if:

x divides y exactly

with remainder zero.

---

## Notation

x | y

---

## Example 1

2 divides 8

8 ÷ 2 = 4

Remainder = 0

Relation exists.

---

## Example 2

3 divides 12

12 ÷ 3 = 4

Relation exists.

---

## Example 3

5 divides 12

12 ÷ 5 = 2 remainder 2

Relation does not exist.

---

## Digraph Example

Set:

{1,2,4}

Relations:

1 → 2

1 → 4

2 → 4

---

# 16. Self-Loop

## Definition

A self-loop is an arrow that starts and ends at the same vertex.

---

## Example

Relation:

(3,3)

Draw:

3 ↺

---

## Example

(5,5)

Draw:

5 ↺

---

## Why It Matters

Self-loops show:

An element is related to itself.

---

## Reflexive Relation Example

A={1,2,3}

Contains:

(1,1)

(2,2)

(3,3)

Each vertex has a self-loop.

---

# Quick Comparison Table

| Concept | Meaning |
|----------|----------|
| Relation Representation | Ways to display relations |
| Zero-One Matrix | Matrix using only 0 and 1 |
| Cardinality | Number of elements |
| Main Diagonal | Top-left to bottom-right |
| Strict Inequality Matrix | Diagonal all zeros |
| Reflexive Matrix | Diagonal all ones |
| Relational Union | Combine all pairs |
| Relational Intersection | Keep common pairs |
| Join (∨) | Logical OR |
| Meet (∧) | Logical AND |
| Digraph | Graph with arrows |
| Vertex | Node |
| Directed Edge | Arrow |
| Divisibility Relation | x divides y |
| Self-Loop | Arrow from a node to itself |

---

# Learning Flow

Sets
↓
Cartesian Products
↓
Relations
↓
Relation Representation
↓
Matrices
↓
Boolean Operations
↓
Union and Intersection
↓
Digraphs
↓
Vertices and Edges
↓
Divisibility Relations
↓
Self-Loops
↓
Graph Theory
↓
Computer Science

---

# Key Facts to Remember

1. Relations can be represented using ordered pairs, matrices, and graphs.

2. A Zero-One Matrix uses:
   - 1 = related
   - 0 = not related

3. Cardinality means set size.

4. The main diagonal reveals self-relations.

5. Strict inequality (<) produces a diagonal of all zeros.

6. Reflexive relations produce a diagonal of all ones.

7. Union uses logical OR.

8. Intersection uses logical AND.

9. Digraphs visualize relations using arrows.

10. Vertices represent elements.

11. Directed edges represent relationships.

12. Self-loops indicate an element is related to itself.

13. These concepts are fundamental to:
    - Graph Theory
    - Databases
    - Data Engineering
    - Computer Networks
    - Social Networks
    - Artificial Intelligence
    - Discrete Mathematics
    - Algorithms

Think of relation matrices as spreadsheet versions of relations and digraphs as visual map versions of the same information.