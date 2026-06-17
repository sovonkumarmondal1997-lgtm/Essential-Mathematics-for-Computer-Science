# Function Composition and Composite Functions

---

# 1. Function Composition

## Definition

Function Composition is the process of combining two functions to create a new function.

The output of one function becomes the input of another function.

Think of it as:

Function A → Function B

or

Machine 1 → Machine 2

---

## Simple Analogy

Imagine a factory:

Step 1: Paint a car

Step 2: Add wheels

The output of Step 1 becomes the input of Step 2.

This is exactly how function composition works.

---

## Example 1

Let:

f(x) = x + 2

g(x) = 3x

Input:

x = 2

First apply g:

g(2) = 6

Now apply f:

f(6) = 8

Result:

(f ∘ g)(2) = 8

---

## Example 2

f(x)=x²

g(x)=x+1

Input:

x=3

g(3)=4

f(4)=16

Result:

(f∘g)(3)=16

---

## Real-Life Example

Temperature Conversion

Step 1:

Convert Celsius to Fahrenheit

Step 2:

Round to nearest integer

Output from first step becomes input for second step.

---

# 2. Composition Notation

## Definition

The notation:

(f ∘ g)(x)

means:

Apply g first

Then apply f

---

## Important Rule

(f ∘ g)(x)

means

f(g(x))

NOT

g(f(x))

---

## Reading

(f ∘ g)(x)

is read as:

"f composed with g"

or

"f after g"

---

## Example 1

f(x)=x+5

g(x)=2x

Then:

(f∘g)(x)

=f(2x)

=2x+5

---

## Example 2

f(x)=x²

g(x)=x+1

(f∘g)(x)

=f(x+1)

=(x+1)²

---

## Quick Memory Trick

Inside function works first.

Outside function works second.

---

# 3. Two-Stage Functional Processing

## Definition

Function composition works like a two-stage pipeline.

Stage 1:

Inner Function

↓

Stage 2:

Outer Function

---

## General Form

Input x

↓

g(x)

↓

f(g(x))

↓

Final Output

---

## Example 1

g(x)=x+2

f(x)=3x

Input:

x=4

Stage 1:

g(4)=6

Stage 2:

f(6)=18

Final output:

18

---

## Example 2

g(x)=x²

f(x)=x−1

Input:

3

Stage 1:

3²=9

Stage 2:

9−1=8

Output:

8

---

## Real-Life Example

Online Shopping

Input:

Product Price

↓

Apply Discount

↓

Apply Tax

↓

Final Price

Two-stage processing.

---

# 4. Domain-to-Codomain Chaining (Sets A, B, and C)

## Definition

For composition to work:

Output of first function must be acceptable as input to second function.

---

## Structure

f : A → B

g : B → C

Then:

g ∘ f : A → C

---

## Visual Diagram

A

↓

f

↓

B

↓

g

↓

C

---

## Example

A = {1,2,3}

B = {2,4,6}

C = {4,8,12}

Function:

f(x)=2x

Function:

g(x)=2x

Then:

g(f(x))

works perfectly.

---

## Real-Life Example

Student Marks

↓

Letter Grades

↓

Scholarship Category

Marks become grades.

Grades become categories.

---

## Invalid Example

Suppose:

f outputs words

g expects numbers

Output and input types do not match.

Composition impossible.

---

# 5. Non-Commutative Property of Composition

## Definition

Function composition is usually order-dependent.

Changing the order changes the answer.

---

## Mathematical Statement

Generally:

f(g(x))

≠

g(f(x))

---

## Example 1

f(x)=x+1

g(x)=2x

Find:

f(g(x))

First:

g(x)=2x

Then:

f(2x)=2x+1

Result:

2x+1

---

Now:

g(f(x))

First:

f(x)=x+1

Then:

g(x+1)=2(x+1)

=2x+2

Result:

2x+2

---

Comparison:

2x+1

≠

2x+2

Therefore:

f(g(x))

≠

g(f(x))

---

## Example 2

f(x)=x²

g(x)=x+3

Compute:

f(g(x))

=(x+3)²

=x²+6x+9

---

Compute:

g(f(x))

=x²+3

---

Not equal.

Order matters.

---

## Real-Life Example

Cooking

Operation 1:

Bake Cake

Operation 2:

Add Frosting

Correct:

Bake → Frost

Incorrect:

Frost → Bake

Results are different.

---

# 6. Algebraic Expansion of Composite Functions

## Definition

Algebraic expansion means replacing the variable in one function with the complete expression from another function.

---

## General Process

Step 1:

Find inner function.

Step 2:

Substitute entire expression.

Step 3:

Simplify.

---

## Example 1

f(x)=x²

g(x)=x+2

Find:

(f∘g)(x)

=f(g(x))

=f(x+2)

=(x+2)²

Expand:

=x²+4x+4

Final Answer:

x²+4x+4

---

## Example 2

f(x)=3x+1

g(x)=x²

Find:

(f∘g)(x)

=f(x²)

=3(x²)+1

=3x²+1

---

## Example 3

f(x)=√x

g(x)=x+4

Find:

(f∘g)(x)

=f(x+4)

=√(x+4)

---

## Example 4

f(x)=2x−5

g(x)=3x+1

Find:

(f∘g)(x)

=f(3x+1)

=2(3x+1)-5

=6x+2-5

=6x-3

---

## Example 5

f(x)=x³

g(x)=2x

Find:

(f∘g)(x)

=(2x)³

=8x³

---

## Common Student Mistake

Wrong:

f(x)=x²

g(x)=x+1

(f∘g)(x)

=x²+1

❌ Incorrect

Correct:

(x+1)²

=x²+2x+1

✔ Correct

Always substitute the entire expression.

---

# Complete Comparison Table

| Concept | Meaning |
|----------|----------|
| Function Composition | Combining two functions |
| Composition Notation | (f∘g)(x)=f(g(x)) |
| Two-Stage Processing | Inner function then outer function |
| Domain-Codomain Chaining | Output of first must fit input of second |
| Non-Commutative Property | Order matters |
| Algebraic Expansion | Substitute and simplify |

---

# Visual Flow of Composition

Input x

↓

Inner Function g(x)

↓

Intermediate Output

↓

Outer Function f(x)

↓

Final Output

---

# Complete Learning Flow

Set
↓
Relation
↓
Function
↓
Domain and Co-domain
↓
Range and Image
↓
Injective Functions
↓
Surjective Functions
↓
Bijective Functions
↓
Inverse Functions
↓
Function Composition
↓
Composite Functions
↓
Function Chaining
↓
Algebraic Expansion
↓
Advanced Mathematics

---

# Key Facts to Remember

1. Composition combines two functions into one.

2. (f∘g)(x) means f(g(x)).

3. The inside function is always evaluated first.

4. Composition usually is NOT commutative.

5. f(g(x)) is generally different from g(f(x)).

6. The output of the first function must be valid input for the second function.

7. To expand a composite function, substitute the entire expression, not just the variable.

8. Composite functions are heavily used in:
   - Calculus
   - Machine Learning
   - Data Science
   - Artificial Intelligence
   - Computer Graphics
   - Signal Processing
   - Data Engineering Pipelines

Think of function composition as mathematical pipelines where the output of one stage automatically becomes the input of the next stage.