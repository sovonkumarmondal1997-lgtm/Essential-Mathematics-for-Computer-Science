# Properties of Relations: Reflexive, Symmetric and Anti-Symmetric Relations

---

# 1. Properties of Relations

## Definition

**Properties of Relations** are characteristics that describe how elements of a set interact with each other.

These properties help us classify and understand relations.

---

## Main Properties

1. Reflexive
2. Symmetric
3. Anti-Symmetric
4. Transitive (studied later)

---

## Why Are They Important?

They help answer questions such as:

- Does every element relate to itself?
- If A relates to B, does B relate to A?
- Can two different elements relate in both directions?

---

## Example

Set:

S = {1,2,3}

Relation:

R = {(1,1),(2,2),(3,3)}

This relation is:

Reflexive ✔

Symmetric ✔

Anti-Symmetric ✔

---

# 2. Reflexivity / Reflexive Relation

## Definition

A relation is **Reflexive** if every element is related to itself.

Mathematically:

(x,x) ∈ R

for every

x ∈ S

---

## Simple Meaning

Every element must have a "self-connection."

---

## Example 1

Set:

S = {1,2,3}

Relation:

R = {
(1,1),
(2,2),
(3,3)
}

Reflexive ✔

---

## Example 2

Relation:

≤

on

{1,2,3}

Since:

1 ≤ 1

2 ≤ 2

3 ≤ 3

Reflexive ✔

---

## Example 3

Students and Friendship With Self

Every student is considered related to themselves.

(Rahul,Rahul)

(Priya,Priya)

(Amit,Amit)

Reflexive ✔

---

## Not Reflexive Example

S = {1,2,3}

R = {
(1,1),
(2,2)
}

Missing:

(3,3)

Not Reflexive ✘

---

# 3. Reflexive Digraph Profile

## Definition

In a digraph, a reflexive relation must contain a self-loop on every vertex.

---

## Example

Set:

{1,2,3}

Relation:

{
(1,1),
(2,2),
(3,3)
}

---

## Digraph

1 ↺

2 ↺

3 ↺

Every vertex has a loop.

Reflexive ✔

---

## Non-Reflexive Example

1 ↺

2 ↺

3

No loop on 3.

Not Reflexive ✘

---

## Rule

Reflexive Digraph

=

Self-loop at every vertex

---

# 4. Reflexive Matrix Profile

## Definition

A relation is reflexive when all entries on the main diagonal are 1.

---

## Example

|   |1|2|3|
|---|---|---|---|
|1|1|0|0|
|2|0|1|0|
|3|0|0|1|

---

## Diagonal

1

1

1

All ones.

Reflexive ✔

---

## Non-Reflexive Example

|   |1|2|3|
|---|---|---|---|
|1|1|0|0|
|2|0|1|0|
|3|0|0|0|

Diagonal:

1

1

0

Not Reflexive ✘

---

# 5. Symmetry / Symmetric Relation

## Definition

A relation is symmetric if:

Whenever

(a,b) ∈ R

then

(b,a) ∈ R

must also belong to R.

---

## Simple Meaning

If A relates to B,

then B relates to A.

---

## Example 1

Set:

{1,2}

Relation:

{
(1,2),
(2,1)
}

Symmetric ✔

---

## Example 2

Friendship Relation

Rahul is a friend of Priya.

Priya is a friend of Rahul.

Symmetric ✔

---

## Example 3

Same Age Relation

If Rahul is the same age as Amit,

then Amit is the same age as Rahul.

Symmetric ✔

---

## Non-Symmetric Example

Teacher Relation

Rahul teaches Priya.

Priya teaches Rahul.

Not necessarily true.

Not Symmetric ✘

---

# 6. Commutative Property of Equality

## Definition

Equality can be reversed.

If:

a = b

then:

b = a

---

## Why Important?

Many symmetric relation proofs depend on this property.

---

## Example 1

5 = 5

Reversing:

5 = 5

Still true.

---

## Example 2

x + 2 = y

Then:

y = x + 2

Still valid.

---

## Example 3

Modulo Arithmetic

If:

a mod 2 = b mod 2

Then:

b mod 2 = a mod 2

Equality can be reversed.

---

## Real-Life Example

If Rahul and Amit have the same birthday,

then Amit and Rahul have the same birthday.

---

# 7. Symmetric Digraph Profile

## Definition

A symmetric relation requires arrows in both directions.

---

## Example

Relation:

{
(1,2),
(2,1)
}

---

## Digraph

1 ⇄ 2

Two arrows.

---

## Example

{
(1,3),
(3,1)
}

---

Digraph

1 ⇄ 3

---

## Rule

Either:

No connection

or

Two-way connection

---

## Invalid Example

1 → 2

but not

2 → 1

Not symmetric.

---

# 8. Symmetric Matrix

## Definition

A matrix is symmetric when it mirrors itself across the main diagonal.

---

## Rule

Mij = Mji

---

## Example

|   |1|2|3|
|---|---|---|---|
|1|1|1|0|
|2|1|1|1|
|3|0|1|1|

---

Mirror image.

Symmetric matrix ✔

---

## Example

Position (1,2)=1

Position (2,1)=1

Match.

---

## Non-Symmetric Example

|   |1|2|
|---|---|---|
|1|0|1|
|2|0|0|

(1,2)=1

(2,1)=0

Not symmetric.

---

# 9. Anti-Symmetry / Anti-Symmetric Relation

## Definition

A relation is anti-symmetric if:

Whenever

(a,b) ∈ R

and

(b,a) ∈ R

then

a=b

must be true.

---

## Simple Meaning

Different elements cannot point to each other in both directions.

---

## Example 1

Relation:

≤

on numbers.

---

Suppose:

2 ≤ 3

True

---

3 ≤ 2

False

---

Anti-Symmetric ✔

---

## Example 2

Subset Relation

A ⊆ B

and

B ⊆ A

only when

A = B

Anti-Symmetric ✔

---

# 10. Divisibility Relation

## Definition

a is related to b when:

a divides b exactly.

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

## Why Anti-Symmetric?

Suppose:

a | b

and

b | a

Then:

a = b

for positive integers.

---

## Example

4 | 4

and

4 | 4

Same number.

Valid.

---

Different numbers cannot divide each other both ways.

---

# 11. Anti-Symmetric Digraph Profile

## Definition

Anti-symmetric relations prohibit two-way arrows between different vertices.

---

## Allowed

1 → 2

---

## Not Allowed

1 ⇄ 2

unless

1 = 2

---

## Example

Relation:

{
(1,2),
(2,3)
}

Digraph:

1 → 2 → 3

Anti-Symmetric ✔

---

## Invalid Example

{
(1,2),
(2,1)
}

Digraph:

1 ⇄ 2

Not Anti-Symmetric ✘

---

# 12. Anti-Symmetric Matrix Profile

## Definition

For distinct indices:

i ≠ j

If:

Mij = 1

then:

Mji = 0

---

## Example

|   |1|2|3|
|---|---|---|---|
|1|1|1|0|
|2|0|1|1|
|3|0|0|1|

---

Observe

(1,2)=1

(2,1)=0

Valid.

---

Observe

(2,3)=1

(3,2)=0

Valid.

---

Anti-Symmetric ✔

---

## Invalid Example

|   |1|2|
|---|---|---|
|1|1|1|
|2|1|1|

---

(1,2)=1

(2,1)=1

Different elements connected both ways.

Not Anti-Symmetric ✘

---

# 13. Adjacency Matrix

## Definition

An adjacency matrix is a square zero-one matrix representing a graph or relation.

Rows and columns correspond directly to vertices.

---

## Rule

1 = Edge Exists

0 = Edge Does Not Exist

---

## Example

Digraph:

1 → 2

2 → 3

---

Adjacency Matrix

|   |1|2|3|
|---|---|---|---|
|1|0|1|0|
|2|0|0|1|
|3|0|0|0|

---

## Example

Digraph

1 ⇄ 2

---

Matrix

|   |1|2|
|---|---|---|
|1|0|1|
|2|1|0|

---

## Real-Life Example

Social Networks

1 = User follows another user

0 = No connection

---

# Quick Comparison Table

| Property | Key Rule |
|-----------|-----------|
| Reflexive | Every element relates to itself |
| Symmetric | If aRb then bRa |
| Anti-Symmetric | If aRb and bRa then a=b |
| Adjacency Matrix | Matrix representation of a graph |
| Reflexive Matrix | Diagonal all ones |
| Symmetric Matrix | Mirror across diagonal |
| Anti-Symmetric Matrix | No mirrored ones off diagonal |

---

# Visual Learning Flow

Sets
↓
Relations
↓
Relation Properties
↓
Reflexive
↓
Symmetric
↓
Anti-Symmetric
↓
Digraph Representation
↓
Matrix Representation
↓
Adjacency Matrices
↓
Graph Theory
↓
Discrete Mathematics

---

# Key Facts to Remember

1. Reflexive means every element relates to itself.

2. Reflexive digraphs contain self-loops on every vertex.

3. Reflexive matrices have diagonal entries equal to 1.

4. Symmetric means relationships work both ways.

5. Symmetric digraphs contain paired arrows.

6. Symmetric matrices mirror across the main diagonal.

7. Anti-symmetric means different elements cannot relate both ways.

8. Divisibility is a classic anti-symmetric relation.

9. Anti-symmetric digraphs prohibit bidirectional arrows between different vertices.

10. Anti-symmetric matrices prohibit mirrored 1s across the diagonal.

11. Adjacency matrices are matrix representations of graphs.

12. These concepts are fundamental in:
    - Graph Theory
    - Database Design
    - Computer Networks
    - Data Engineering
    - Algorithms
    - Artificial Intelligence
    - Discrete Mathematics

Think of relation properties as rules that determine the behavior of connections between elements, while matrices and digraphs are simply different ways of visualizing those connections.