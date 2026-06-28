# Boolean Functions and Their Representations - Beginner Friendly Notes

# 1. Boolean Function

## What is a Boolean Function?

A Boolean function is a rule that takes one or more binary inputs (0
or 1) and produces exactly one binary output (0 or 1).

Think of it like a small machine:

Inputs (0 or 1) → Boolean Function → Output (0 or 1)

### Example 1

f(x) = x'

If x = 0 → Output = 1

If x = 1 → Output = 0

### Example 2

f(x,y) = x·y

  x   y   Output
  --- --- --------
  0   0   0
  0   1   0
  1   0   0
  1   1   1

The function outputs 1 only when both inputs are 1.

------------------------------------------------------------------------

# 2. Truth Table Representation

A truth table is the unique and complete way to describe a Boolean
function.

For n input variables, the truth table has:

2ⁿ rows

### Example

Function:

f(x,y)=x+y

  x   y   f
  --- --- ---
  0   0   0
  0   1   1
  1   0   1
  1   1   1

Every possible input combination is listed exactly once.

------------------------------------------------------------------------

# 3. Algebraic Representation

Instead of using a truth table, we can write Boolean functions as
algebraic expressions.

Different expressions can represent the same truth table.

### Example

f=x+x·y

Using the Absorption Law:

x+x·y=x

Both expressions have the same truth table.

Another Example

x'+y

is equivalent to

x→y

------------------------------------------------------------------------

# 4. Sum of Products (SOP)

SOP means:

First perform AND.

Then combine the terms using OR.

General form:

(A·B)+(C·D)+(E·F)

### Example

f=x'y+xy'

This is XOR.

Example

f=xy+xz+yz

Each term is an AND.

The final operation is OR.

------------------------------------------------------------------------

# 5. Product of Sums (POS)

POS means:

First perform OR.

Then multiply (AND) all groups together.

General form:

(A+B)(C+D)(E+F)

### Example

f=(x+y)(x+z)

Each bracket is an OR.

The brackets are combined using AND.

Another Example

(x+y)(y+z)(x+z)

------------------------------------------------------------------------

# 6. SOP Construction Rule

To build SOP from a truth table:

Step 1

Find every row where the output is 1.

Step 2

Create one AND term for each row.

Rule:

Input 1 → Variable

Input 0 → Complement

Step 3

Join all terms using OR.

### Example

Truth Table

  x   y   f
  --- --- ---
  0   0   0
  0   1   1
  1   0   1
  1   1   0

Rows with output 1:

(0,1)

(1,0)

Convert

(0,1)

↓

x'y

Convert

(1,0)

↓

xy'

Final SOP

x'y+xy'

------------------------------------------------------------------------

# 7. Exclusive OR (XOR)

Meaning:

Exactly one input is True.

Not both.

Truth Table

  x   y   x⊕y
  --- --- -----
  0   0   0
  0   1   1
  1   0   1
  1   1   0

SOP Expression

x'y+xy'

### Real-Life Examples

One switch ON

Light ON

Both switches ON

Light OFF

Another Example

Tea OR Coffee

Choose exactly one.

------------------------------------------------------------------------

# 8. Implies Function

"If x then y"

Boolean form

x→y

Equivalent Boolean expression

x'+y

Truth Table

  x   y   x→y
  --- --- -----
  0   0   1
  0   1   1
  1   0   0
  1   1   1

### Example

If you study

then you pass.

If you do not study,

the implication is automatically True.

Only when

Study=True

Pass=False

does the implication become False.

------------------------------------------------------------------------

# Comparison Table

  Representation   Example
  ---------------- ------------------------------------
  Truth Table      List all input-output combinations
  Algebraic        x+y
  SOP              x'y+xy'
  POS              (x+y)(x'+y)

------------------------------------------------------------------------

# Memory Tricks

-   Boolean Function = Binary inputs → Binary output.
-   Truth Table = Complete description.
-   Algebraic Representation = Mathematical formula.
-   SOP = AND first, then OR.
-   POS = OR first, then AND.
-   XOR = Exactly one input is True.
-   Implication = x'+y.

Boolean functions are used in logic gates, CPUs, digital circuit design,
databases, compiler optimization, artificial intelligence, networking,
and computer architecture.
