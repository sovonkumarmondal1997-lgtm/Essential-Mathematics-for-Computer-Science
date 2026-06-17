# Mathematical Relations, Cartesian Products and Binary Relations

---

# 1. Mathematical Relation

## Definition

A **Mathematical Relation** is a link, connection, or association between elements of one set and elements of another set (or the same set).

A relation tells us:

"Which elements are connected to which?"

---

## Simple Idea

Think of a relation as drawing arrows between objects.

Example:

Rahul → Mathematics

Priya → Science

Amit → Mathematics

These arrows create a relation.

---

## Example 1: Students and Courses

Students:

A = {Rahul, Priya, Amit}

Courses:

B = {Math, Science}

Relation:

R = {
(Rahul, Math),
(Priya, Science),
(Amit, Math)
}

This relation shows which course each student studies.

---

## Example 2: Parents and Children

Parents:

{John, Sarah}

Children:

{Tom, Emma}

Relation:

{
(John, Tom),
(Sarah, Emma)
}

---

## Example 3: Countries and Capitals

{
(India, New Delhi),
(Japan, Tokyo),
(France, Paris)
}

Each pair represents a relation.

---

## Real-Life Example

Social media friendships, employee-department assignments, and customer-order mappings are all examples of relations.

---

# 2. Relation Notation (x R y vs x not R y)

## Definition

Mathematicians use special notation to indicate whether two elements are related.

---

## Related

x R y

means:

"x is related to y under relation R"

---

## Not Related

x not R y

means:

"x is not related to y under relation R"

---

## Example 1

Relation:

"Is enrolled in"

Rahul R Mathematics

means:

Rahul is enrolled in Mathematics.

---

Priya not R Mathematics

means:

Priya is not enrolled in Mathematics.

---

## Example 2

Relation:

"<"

2 R 5

means:

2 < 5

True.

---

5 not R 2

means:

5 < 2

False.

---

## Example 3

Relation:

"Divides"

2 R 8

because:

2 divides 8

---

3 not R 8

because:

3 does not divide 8

---

# 3. Set

## Definition

A **Set** is a collection of distinct objects.

The objects inside a set are called elements.

---

## Example 1

Numbers:

A = {1,2,3,4,5}

---

## Example 2

Students:

S = {Rahul, Priya, Amit}

---

## Example 3

Courses:

C = {Math, Science, History}

---

## Example 4

Programming Languages:

P = {Python, Java, SQL}

---

## Important Rule

Sets do not contain duplicate elements.

---

### Valid Set

{1,2,3}

---

### Invalid Representation

{1,2,2,3}

Duplicates are ignored.

Equivalent set:

{1,2,3}

---

# 4. Cartesian Product (A × B)

## Definition

The Cartesian Product of two sets A and B is the set of all possible ordered pairs.

Notation:

A × B

---

## Formula

A × B

=

{(x,y) | x ∈ A and y ∈ B}

---

## Example 1

A = {1,2}

B = {a,b}

Then:

A × B

=

{
(1,a),
(1,b),
(2,a),
(2,b)
}

---

## Example 2

A = {Red, Blue}

B = {Circle, Square}

Cartesian Product:

{
(Red,Circle),
(Red,Square),
(Blue,Circle),
(Blue,Square)
}

---

## Real-Life Example

Shirt Colors:

{Red, Blue}

Sizes:

{M,L}

Possible combinations:

{
(Red,M),
(Red,L),
(Blue,M),
(Blue,L)
}

---

# 5. Ordered Pair (x,y)

## Definition

An ordered pair is a pair of elements where order matters.

Notation:

(x,y)

---

## Important Rule

(x,y)

is generally different from

(y,x)

---

## Example 1

(1,2)

≠

(2,1)

---

## Example 2

Student and Course

(Rahul, Math)

means:

Rahul studies Math.

---

(Math, Rahul)

has a completely different meaning.

---

## Example 3

Coordinates

(3,5)

means:

x = 3

y = 5

---

## Real-Life Example

Address:

(House Number, Street)

(25, Park Street)

Different from:

(Park Street, 25)

---

# 6. Binary Relation

## Definition

A Binary Relation is a selected collection of ordered pairs from a Cartesian Product.

It is a subset of:

A × B

---

## Formula

R ⊆ A × B

---

## Example 1

A = {1,2,3}

B = {a,b}

Cartesian Product:

{
(1,a),
(1,b),
(2,a),
(2,b),
(3,a),
(3,b)
}

---

Relation:

R = {
(1,a),
(2,b)
}

R is a binary relation.

---

## Example 2

Students:

{Rahul, Priya}

Courses:

{Math, Science}

Relation:

{
(Rahul, Math),
(Priya, Science)
}

---

## Real-Life Example

Employee-to-Department assignments.

Only specific pairs are chosen from all possible combinations.

---

# 7. Relation on a Single Set

## Definition

A relation on a single set occurs when:

Domain = Codomain

The relation is a subset of:

A × A

---

## Example

A = {1,2,3}

---

Cartesian Product

A × A

=

{
(1,1),
(1,2),
(1,3),
(2,1),
(2,2),
(2,3),
(3,1),
(3,2),
(3,3)
}

---

Relation:

R = {
(1,2),
(2,3)
}

This is a relation on A.

---

## Example 2

Students:

A = {Rahul, Priya, Amit}

Relation:

"Is friends with"

{
(Rahul, Priya),
(Priya, Amit)
}

Same set on both sides.

---

## Example 3

Numbers:

Relation:

"Less than"

A = {1,2,3}

{
(1,2),
(1,3),
(2,3)
}

---

# 8. Strict Inequality Relation (<)

## Definition

The strict inequality relation "<" connects two numbers when the first number is strictly smaller than the second.

---

## Rule

x < y

means:

x is less than y

---

## Example 1

2 < 5

True

Relation exists.

Pair:

(2,5)

belongs to the relation.

---

## Example 2

7 < 10

True

---

## Example 3

5 < 5

False

Because strict inequality requires:

smaller

not equal.

---

## Example 4

8 < 3

False

No relation.

---

## Relation on Set

A = {1,2,3}

Using "<"

Valid pairs:

{
(1,2),
(1,3),
(2,3)
}

---

Pairs not included:

(1,1)

(2,2)

(3,3)

(3,1)

(3,2)

---

## Real-Life Example

Age Comparison

Person A is younger than Person B.

If:

Age(A)=20

Age(B)=25

Then:

20 < 25

Relation holds.

---

# Quick Comparison Table

| Concept | Meaning |
|----------|----------|
| Set | Collection of distinct elements |
| Ordered Pair | Pair where order matters |
| Cartesian Product | All possible ordered pairs |
| Relation | Selected connections between elements |
| Binary Relation | Subset of a Cartesian Product |
| Relation on a Set | Relation from A to A |
| x R y | x is related to y |
| x not R y | x is not related to y |
| Strict Inequality | x < y |

---

# Visual Learning Flow

Set
↓
Elements
↓
Ordered Pairs
↓
Cartesian Product
↓
Binary Relation
↓
Relation Notation
↓
Relations on a Single Set
↓
Ordering Relations
↓
Strict Inequality Relations

---

# Key Facts to Remember

1. A relation is a connection between elements.

2. A set is a collection of distinct objects.

3. Ordered pairs care about order.

4. (x,y) is usually different from (y,x).

5. A Cartesian Product contains all possible ordered pairs.

6. A binary relation is a subset of a Cartesian Product.

7. Relations can exist between two different sets or within the same set.

8. x R y means x is related to y.

9. x not R y means x is not related to y.

10. The strict inequality relation (<) only holds when the first number is smaller than the second.

11. Relations are the foundation of:
    - Functions
    - Databases
    - Graph Theory
    - Discrete Mathematics
    - Data Modeling
    - Data Engineering
    - Computer Science

Think of a relation as a set of approved connections chosen from all possible connections that could exist between objects.