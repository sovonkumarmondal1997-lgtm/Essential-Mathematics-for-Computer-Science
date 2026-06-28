# Combinational Circuits and Adders - Beginner Friendly Notes

# 1. Combinational Circuits (Logic Networks)

## What is a Combinational Circuit?

A combinational circuit is a collection of interconnected logic gates
that work together to implement a Boolean function.

The output depends **only on the current input values**.

There is **no memory** of previous inputs.

Think of it as a calculator:

Current Inputs → Logic Gates → Current Output

If the inputs change, the output changes immediately.

### Examples

Example 1

Automatic Door

Inputs: - Motion Sensor - Door Unlocked

Output: - Door Opens

Example 2

Fire Alarm

Inputs: - Smoke - High Temperature

Output: - Alarm ON

Example 3

Digital Calculator

Inputs: - Two binary numbers

Output: - Sum

------------------------------------------------------------------------

# 2. Circuit Minimization

## What is Circuit Minimization?

Circuit minimization means designing the same Boolean function using
**fewer logic gates**.

Goals:

-   Reduce hardware cost
-   Reduce power consumption
-   Increase speed
-   Reduce chip size
-   Simplify wiring

### Example

Original Function

F = A·B + A·B'

Using Boolean Algebra

F = A(B + B')

F = A·1

F = A

Instead of three gates, only one wire is needed.

Another Example

F = A + A·B

↓

A

(Absorption Law)

------------------------------------------------------------------------

# 3. Functional Mapping

Functional mapping means moving between a Boolean expression and a logic
circuit.

There are two directions.

### Direction 1

Boolean Function → Circuit

Example

F = A·B + C

Build:

1.  AND gate for A·B
2.  OR gate combines A·B with C

### Direction 2

Circuit → Boolean Function

Read the circuit gate by gate.

Example

Inputs A and B go to an AND gate.

The AND output and C go to an OR gate.

Boolean function:

F = A·B + C

------------------------------------------------------------------------

# 4. Half Adder

A Half Adder adds **two binary bits**.

Inputs:

A

B

Outputs:

Sum (S)

Carry (C)

Logic:

Sum = A ⊕ B

Carry = A·B

Truth Table

  A   B   Sum   Carry
  --- --- ----- -------
  0   0   0     0
  0   1   1     0
  1   0   1     0
  1   1   0     1

### Example

1 + 0

Binary result:

01

Sum = 1

Carry = 0

Example

1 + 1

Binary result:

10

Sum = 0

Carry = 1

Limitation:

A Half Adder cannot accept a Carry from a previous addition.

------------------------------------------------------------------------

# 5. Full Adder

A Full Adder solves the limitation of a Half Adder.

Inputs:

A

B

Carry In (Cin)

Outputs:

Sum

Carry Out (Cout)

Logic

Sum = A ⊕ B ⊕ Cin

Carry = AB + ACin + BCin

Truth Table

  A   B   Cin   Sum   Carry
  --- --- ----- ----- -------
  0   0   0     0     0
  0   0   1     1     0
  0   1   0     1     0
  0   1   1     0     1
  1   0   0     1     0
  1   0   1     0     1
  1   1   0     0     1
  1   1   1     1     1

### Example

1 + 1 + Carry(1)

Binary:

1 + 1 + 1

= 11₂

Sum = 1

Carry = 1

Full Adders are connected together to add multi-bit binary numbers
inside CPUs.

------------------------------------------------------------------------

# Half Adder vs Full Adder

  Feature        Half Adder   Full Adder
  -------------- ------------ -----------------------------
  Inputs         2            3
  Carry In       No           Yes
  Sum Output     Yes          Yes
  Carry Output   Yes          Yes
  Used Alone     Yes          Usually connected in chains

------------------------------------------------------------------------

# 6. Block Diagram Abstraction (Box Diagram)

Instead of drawing every logic gate, engineers often hide the internal
circuit.

They show only:

-   Inputs
-   Outputs
-   A box representing the circuit

Example

+----------------+
| Half Adder     |
|                |
| A Sum B Carry  |
+----------------+

Internally:

-   XOR gate
-   AND gate

But users do not need to see them.

Another Example

CPU

Instead of drawing billions of transistors, diagrams simply show:

  -----------
  CPU

  -----------

This makes large systems easier to understand.

------------------------------------------------------------------------

# Real-Life Applications

### Calculator

Uses Full Adders to add numbers.

### CPU

Contains millions of combinational circuits.

### ALU (Arithmetic Logic Unit)

Uses Half Adders, Full Adders, multiplexers, and logic gates.

### Digital Clock

Uses combinational circuits to process input signals.

### Traffic Controller

Processes sensor inputs and controls traffic lights.

------------------------------------------------------------------------

# Memory Tricks

-   Combinational Circuit = Output depends only on current inputs.
-   Circuit Minimization = Same function, fewer gates.
-   Functional Mapping = Expression ↔ Circuit.
-   Half Adder = Adds two bits.
-   Full Adder = Adds two bits plus Carry In.
-   Box Diagram = Hide internal details.

These circuits are the foundation of CPUs, arithmetic logic units
(ALUs), calculators, digital electronics, computer architecture,
embedded systems, and processor design.