# Sets - Quick Notes

## Definition of a Set
A **set** is a well-defined collection of distinct objects called elements.

**Example:**
```text
E = {2, 3, 4, 5}
```

---

# Examples of Different Sets

## Set of Positive Integers
```text
P = {1, 2, 3, 4, 5, ...}
```

## Set of Even Numbers
```text
E = {2, 4, 6, 8, 10, ...}
```

## Set of Vowels
```text
V = {a, e, i, o, u}
```

## Empty Set
A set containing no elements is called an **empty set**.

**Symbol:**
```text
∅
```

**Example:**
```text
A = ∅
```

or

```text
A = {}
```

---

# Set Notation

## Definition
**Set notation** is a way of representing the elements of a set using curly braces `{ }`.

**Example:**
```text
A = {1, 2, 3, 4, 5}
```

---

# Element of a Set

## Definition
An object belonging to a set is called an **element** of that set.

**Symbol:**
```text
∈
```
(read as "belongs to" or "is an element of")

### Example
```text
A = {1, 2, 3, 4, 5}

3 ∈ A
```

Meaning:
```text
3 is an element of set A.
```

### Another Example
```text
7 ∉ A
```

Meaning:
```text
7 is not an element of set A.
```

---

# Cardinality of a Set

## Definition
The **cardinality** of a set is the number of elements present in the set.

**Symbol:**
```text
|A|
```

### Example
```text
A = {1, 2, 3, 4, 5}
```

Then,

```text
|A| = 5
```

because there are 5 elements in the set.

### Another Example
```text
B = {a, b, c}
```

Then,

```text
|B| = 3
```

---

# Subset of a Set

## Definition
A set A is called a **subset** of set B if every element of A is also an element of B.

**Symbol:**
```text
⊆
```

### Example
```text
A = {1, 2, 3}
B = {1, 2, 3, 4, 5}
```

Then,

```text
A ⊆ B
```

because every element of A is present in B.

---

# Empty Set is a Subset of Any Set

The empty set contains no elements, so it never violates the subset condition.

### Example
```text
A = {1, 2, 3, 4}
```

Then,

```text
∅ ⊆ A
```

because there are no elements in ∅ that are missing from A.

### Another Example
```text
∅ ⊆ {a, b, c}
```

This is always true.

---

# Any Set is a Subset of Itself

Every element of a set obviously belongs to the same set.

### Example
```text
A = {1, 2, 3}
```

Then,

```text
A ⊆ A
```

because all elements of A are contained in A itself.

### Another Example
```text
B = {a, b, c}
```

Then,

```text
B ⊆ B
```

---

# Special Sets

## 1. Natural Numbers (N)

### Definition
Natural numbers are counting numbers starting from 1.

**Symbol:**
```text
N
```

**Example:**
```text
N = {1, 2, 3, 4, 5, ...}
```

### Examples
```text
1 ∈ N
25 ∈ N
100 ∈ N
```

---

## 2. Integers (Z)

### Definition
Integers include positive numbers, negative numbers, and zero.

**Symbol:**
```text
Z
```

**Example:**
```text
Z = {..., -3, -2, -1, 0, 1, 2, 3, ...}
```

### Examples
```text
-5 ∈ Z
0 ∈ Z
10 ∈ Z
```

---

## 3. Rational Numbers (Q)

### Definition
Numbers that can be written in the form p/q where q ≠ 0.

**Symbol:**
```text
Q
```

**Examples**
```text
1/2
3/4
5
-7/3
```

### Example Set
```text
Q = {1/2, 3/4, -2/5, 5, ...}
```

---

## 4. Real Numbers (R)

### Definition
Real numbers include all rational and irrational numbers.

**Symbol:**
```text
R
```

### Examples
```text
5
-3
1/2
√2
π
```

### Example Set
```text
R = {..., -2, -1, 0, 1, 2, 3, π, √2, ...}
```

---

# Relationship Between Special Sets

```text
N ⊆ Z ⊆ Q ⊆ R
```

Meaning:

Natural Numbers ⊆ Integers ⊆ Rational Numbers ⊆ Real Numbers

Example:

```text
5 ∈ N
5 ∈ Z
5 ∈ Q
5 ∈ R
```

Therefore,

```text
Every natural number is an integer.
Every integer is a rational number.
Every rational number is a real number.
```

---

# Summary

| Concept | Symbol | Example |
|----------|---------|----------|
| Element of a Set | ∈ | 3 ∈ {1,2,3} |
| Not an Element | ∉ | 5 ∉ {1,2,3} |
| Empty Set | ∅ | A = ∅ |
| Cardinality | \|A\| | \|{1,2,3}\| = 3 |
| Subset | ⊆ | {1,2} ⊆ {1,2,3} |
| Natural Numbers | N | {1,2,3,...} |
| Integers | Z | {...,-2,-1,0,1,2,...} |
| Rational Numbers | Q | 1/2, 3/4, 5 |
| Real Numbers | R | π, √2, 5, 1/2 |