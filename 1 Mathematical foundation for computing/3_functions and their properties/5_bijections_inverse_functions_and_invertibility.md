# Bijections, Inverse Functions and Invertibility

---

# 1. Bijection / Bijective Function

## Definition

A function is called **bijective** if it is:

1. Injective (One-to-One)
2. Surjective (Onto)

at the same time.

In simple words:

- Every input maps to a unique output.
- Every output is used exactly once.

A bijection creates a perfect pairing between the domain and codomain.

---

## Visual Idea

Domain:

{1,2,3}

Codomain:

{A,B,C}

Mapping:

1 → A

2 → B

3 → C

Every input has a unique output.

Every output is used.

Therefore:

Bijective

---

## Example 1

f(x)=x

Domain:

{1,2,3}

Codomain:

{1,2,3}

Mappings:

1 → 1

2 → 2

3 → 3

Injective ✔

Surjective ✔

Bijective ✔

---

## Example 2

Student ID → Student Record

101 → Rahul

102 → Priya

103 → Amit

Each ID identifies one student.

Every student has one ID.

Bijective.

---

## Example 3

Country → Capital

India → New Delhi

Japan → Tokyo

France → Paris

One country has one capital.

Each capital belongs to one country.

Bijective.

---

## Why Bijections Matter

Only bijective functions can be reversed perfectly.

This leads to inverse functions.

---

# 2. Invertibility / Invertible Function

## Definition

A function is invertible if we can reverse its operation and recover the original input.

Only bijective functions are invertible.

---

## Example 1

Function:

f(x)=x+5

Input:

3

Output:

8

Inverse operation:

8−5=3

Original input recovered.

Therefore:

Invertible.

---

## Example 2

Function:

f(x)=2x

Input:

4

Output:

8

Inverse:

8÷2=4

Invertible.

---

## Not Invertible Example

f(x)=x²

Input:

5 → 25

Input:

−5 → 25

Given output 25, we cannot determine which input produced it.

Therefore:

Not invertible.

---

## Real-Life Example

Password Encryption

Good encryption systems rely heavily on reversible and non-reversible transformations.

---

# 3. Mathematical Proof of Bijection

## Definition

To prove a function is bijective:

Step 1:
Prove Injection

Step 2:
Prove Surjection

Both must be true.

---

## Example

Function:

f(x)=2x+1

Domain:

ℝ

Codomain:

ℝ

---

### Step 1: Injection Proof

Assume:

f(a)=f(b)

2a+1=2b+1

Subtract 1:

2a=2b

Divide by 2:

a=b

Injective ✔

---

### Step 2: Surjection Proof

Let:

y=2x+1

Solve for x:

x=(y−1)/2

For every y there exists an x.

Surjective ✔

---

Result:

Bijective ✔

---

## Simple Memory Trick

Injection:

Different inputs

↓

Different outputs

Surjection:

Every output is used

↓

Together

↓

Bijective

---

# 4. Inverse Function (f⁻¹)

## Definition

An inverse function reverses the action of the original function.

It swaps:

Input ↔ Output

Domain ↔ Codomain

---

## Original Function

f(x)=x+2

Mappings:

1 → 3

2 → 4

3 → 5

---

## Inverse Function

f⁻¹(x)=x−2

Mappings:

3 → 1

4 → 2

5 → 3

---

## Example 2

f(x)=3x

Inverse:

f⁻¹(x)=x/3

---

## Real-Life Example

Currency Conversion

INR → USD

Inverse:

USD → INR

---

# 5. Identity Function

## Definition

An identity function leaves every input unchanged.

Notation:

I(x)=x

---

## Example

Input:

5

Output:

5

Input:

100

Output:

100

---

## Identity Through Inverse Functions

When a function and its inverse are applied one after another:

f(f⁻¹(x))=x

or

f⁻¹(f(x))=x

The result is the original value.

---

## Example

Function:

f(x)=x+5

Inverse:

f⁻¹(x)=x−5

Take:

x=10

Step 1:

f(10)=15

Step 2:

f⁻¹(15)=10

Original value returned.

Identity achieved.

---

## Real-Life Example

Unlocking a door immediately after locking it.

Lock

↓

Unlock

↓

Original state restored.

---

# 6. Algebraic Derivation of an Inverse Function

## Definition

Finding an inverse means solving:

f(x)=y

for x

and then rewriting the result.

---

## Standard Method

Step 1:

Replace f(x) by y

Step 2:

Solve for x

Step 3:

Replace y by x

Step 4:

Write f⁻¹(x)

---

## Example 1

Function:

f(x)=x+5

---

Step 1

y=x+5

---

Step 2

x=y−5

---

Step 3

Replace y with x

---

Answer

f⁻¹(x)=x−5

---

## Example 2

Function:

f(x)=3x

---

Step 1

y=3x

---

Step 2

x=y/3

---

Answer

f⁻¹(x)=x/3

---

## Example 3

Function:

f(x)=2x−7

---

Step 1

y=2x−7

---

Step 2

y+7=2x

---

Step 3

x=(y+7)/2

---

Answer

f⁻¹(x)=(x+7)/2

---

## Example 4

Function:

f(x)=5x+10

---

Step 1

y=5x+10

---

Step 2

y−10=5x

---

Step 3

x=(y−10)/5

---

Answer

f⁻¹(x)=(x−10)/5

---

# 7. Symmetry of Inverse Graphs

## Definition

The graph of a function and the graph of its inverse are mirror images of each other across:

y=x

---

## Important Line

y=x

This diagonal line acts like a mirror.

---

## Example 1

Function:

f(x)=x+2

Point:

(1,3)

---

Inverse:

f⁻¹(x)=x−2

Point:

(3,1)

---

Notice:

(1,3)

became

(3,1)

Coordinates swapped.

---

## Example 2

Function:

f(x)=2x

Point:

(2,4)

Inverse:

f⁻¹(x)=x/2

Point:

(4,2)

Again coordinates swap.

---

## Why This Happens

Original Function:

Input → Output

Inverse Function:

Output → Input

The coordinates exchange positions.

---

## Visual Example

Function:

(1,3)

(2,5)

(4,9)

Inverse:

(3,1)

(5,2)

(9,4)

Perfect reflection across:

y=x

---

## Real-Life Example

Think of looking at a graph in a mirror placed diagonally along y=x.

The original graph and inverse graph become reflections of one another.

---

# Complete Comparison Table

| Concept | Meaning |
|----------|----------|
| Injective | Different inputs give different outputs |
| Surjective | Every output is used |
| Bijective | Injective and Surjective |
| Invertible | Can be reversed |
| Inverse Function | Reverses original mapping |
| Identity Function | Leaves values unchanged |
| Algebraic Derivation | Solve y=f(x) for x |
| Graph Symmetry | Reflection across y=x |

---

# Relationship Between Concepts

Injective
+
Surjective
=
Bijective

Bijective
↓
Invertible

Invertible
↓
Inverse Function Exists

Function + Inverse
↓
Identity Function

---

# Visual Learning Flow

Set
↓
Relation
↓
Function
↓
Injective
↓
Surjective
↓
Bijective
↓
Invertibility
↓
Inverse Functions
↓
Identity Functions
↓
Graph Symmetry
↓
Advanced Mathematics

---

# Key Facts to Remember

1. A bijection is both injective and surjective.

2. Only bijective functions have inverses.

3. An inverse function reverses the original mapping.

4. To find an inverse:
   - Write y=f(x)
   - Solve for x
   - Replace y by x

5. A function and its inverse undo each other.

6. f(f⁻¹(x))=x

7. f⁻¹(f(x))=x

8. Function and inverse graphs are mirror images across y=x.

9. If a function is not injective, it cannot have an inverse.

10. Bijections and inverse functions are fundamental in:
    - Calculus
    - Linear Algebra
    - Cryptography
    - Computer Graphics
    - Machine Learning
    - Data Science
    - Database Key Mapping
    - Data Engineering Systems

Think of a bijection as a perfect two-way road: every destination has exactly one starting point, making it possible to travel forward using the function and backward using its inverse.