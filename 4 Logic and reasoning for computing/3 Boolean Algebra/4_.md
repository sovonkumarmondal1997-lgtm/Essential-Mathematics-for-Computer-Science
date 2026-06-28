# Logic Gates - Beginner Friendly Notes

# 1. Logic Gate

A **logic gate** is an electronic circuit that receives one or more
binary inputs (0 or 1) and produces one binary output according to a
Boolean rule.

Think of a logic gate as a tiny decision-maker inside a computer.

-   0 = LOW = OFF
-   1 = HIGH = ON

Examples: - Smartphone processors use billions of logic gates. -
Automatic doors decide whether to open based on sensor signals. -
Digital calculators perform arithmetic using logic gates.

------------------------------------------------------------------------

# 2. AND Gate

## Rule

f = x · y

The output is 1 **only when every input is 1**.

  x   y   Output
  --- --- --------
  0   0   0
  0   1   0
  1   0   0
  1   1   1

Examples: - Login requires **correct username AND correct password**. -
Car starts only if **battery works AND ignition is on**.

------------------------------------------------------------------------

# 3. OR Gate

## Rule

f = x + y

The output is 1 if **at least one input is 1**.

  x   y   Output
  --- --- --------
  0   0   0
  0   1   1
  1   0   1
  1   1   1

Examples: - Fire alarm activates if **smoke OR heat** is detected. -
Student passes by completing **assignment OR project**.

------------------------------------------------------------------------

# 4. NOT Gate (Inverter)

## Rule

f = x'

The NOT gate has only one input.

It reverses the input.

  x   Output
  --- --------
  0   1
  1   0

Examples: - Light ON becomes Light OFF. - Door Open becomes Door Closed.

------------------------------------------------------------------------

# 5. XOR (Exclusive OR) Gate

The output is 1 **only when the inputs are different**.

Rule:

f = x'y + xy'

  x   y   Output
  --- --- --------
  0   0   0
  0   1   1
  1   0   1
  1   1   0

Examples: - Hotel room: exactly one of two wall switches changes the
light state. - Choose **Tea or Coffee**, but not both.

------------------------------------------------------------------------

# 6. NAND Gate

A NAND gate is an **AND gate followed by a NOT gate**.

Rule:

f = (x·y)'

  x   y   Output
  --- --- --------
  0   0   1
  0   1   1
  1   0   1
  1   1   0

Examples: - Output stays HIGH unless **all required conditions** are
satisfied. - NAND gates are widely used because any digital circuit can
be built using only NAND gates.

------------------------------------------------------------------------

# 7. NOR Gate

A NOR gate is an **OR gate followed by a NOT gate**.

Rule:

f = (x+y)'

  x   y   Output
  --- --- --------
  0   0   1
  0   1   0
  1   0   0
  1   1   0

Examples: - Output is HIGH only when **every input is LOW**. - Used in
memory circuits and control logic.

------------------------------------------------------------------------

# 8. XNOR Gate

An XNOR gate is an **XOR gate followed by a NOT gate**.

Rule:

f = (x⊕y)'

  x   y   Output
  --- --- --------
  0   0   1
  0   1   0
  1   0   0
  1   1   1

Examples: - Password comparison. - Equality checking in processors. -
Output is HIGH when both inputs are the same.

------------------------------------------------------------------------

# 9. Associative and Commutative Gates

Some gates can easily be extended to three or more inputs.

## Commutative

Changing the order does not change the result.

Examples:

A·B = B·A

A+B = B+A

A⊕B = B⊕A

## Associative

Changing grouping does not change the result.

Examples:

(A·B)·C = A·(B·C)

(A+B)+C = A+(B+C)

(A⊕B)⊕C = A⊕(B⊕C)

Therefore AND, OR, XOR, and XNOR can naturally support multiple inputs.

Example:

A AND B AND C

is well-defined without worrying about grouping.

------------------------------------------------------------------------

# 10. Non-Associative Gates (NAND and NOR)

Although NAND and NOR are commutative,

(A NAND B) = (B NAND A),

they are **not associative**.

Examples:

(A NAND B) NAND C

is generally **not equal** to

A NAND (B NAND C)

The same is true for NOR.

Therefore parentheses matter when cascading NAND or NOR gates.

------------------------------------------------------------------------

# 11. Gate-Level De Morgan Representation

De Morgan's Theorems can be represented using logic gates.

Theorems:

(A·B)' = A' + B'

(A+B)' = A'·B'

Interpretation:

-   A NAND gate behaves like two NOT gates followed by an OR gate.
-   A NOR gate behaves like two NOT gates followed by an AND gate.

Examples:

NOT(A AND B)

is equivalent to

(NOT A) OR (NOT B)

NOT(A OR B)

is equivalent to

(NOT A) AND (NOT B)

These equivalent gate layouts help engineers simplify digital circuits.

------------------------------------------------------------------------

# Comparison Table

  Gate   Boolean Expression   Output Rule
  ------ -------------------- ----------------------
  AND    x·y                  All inputs 1
  OR     x+y                  At least one input 1
  NOT    x'                   Reverse input
  XOR    x'y+xy'              Inputs different
  NAND   (x·y)'               NOT of AND
  NOR    (x+y)'               NOT of OR
  XNOR   (x⊕y)'               Inputs equal

# Memory Tricks

-   AND = Everyone agrees.
-   OR = Anyone is enough.
-   NOT = Reverse.
-   XOR = Different.
-   XNOR = Same.
-   NAND = AND then NOT.
-   NOR = OR then NOT.
-   De Morgan swaps AND ↔ OR while negating every input.

Logic gates are the building blocks of CPUs, memory chips, digital
electronics, embedded systems, networking hardware, and modern
computers.
