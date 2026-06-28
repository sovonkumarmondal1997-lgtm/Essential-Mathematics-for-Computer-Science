# Two-Valued Boolean Algebra - Beginner Friendly Notes

# 1. Two-Valued Boolean Algebra

## What is Boolean Algebra?

Boolean Algebra is a branch of mathematics that works with only **two
possible values**:

-   **0 = False = OFF**
-   **1 = True = ON**

Unlike ordinary algebra, Boolean Algebra does not use numbers like 2, 5,
or 100. Every variable can only be either **0** or **1**.

Think of it as the mathematics of decision making.

### Examples

  Variable   Value
  ---------- -------
  x          0
  y          1
  z          0

Example 1

x = 1

Meaning:

True

Example 2

Door Sensor

1 = Door Open

0 = Door Closed

Example 3

Light Switch

1 = ON

0 = OFF

------------------------------------------------------------------------

# 2. Modern Computer Circuit Application

Boolean Algebra is the foundation of modern digital electronics.

Every computer, smartphone, calculator, and processor uses Boolean
Algebra.

Computers understand only:

0

and

1

Transistors behave like tiny electronic switches.

Switch OFF → 0

Switch ON → 1

Millions or billions of transistors work together by applying Boolean
operations.

## Examples

### Example 1

Automatic Door

IF

Motion Detected

AND

Door Unlocked

THEN

Door Opens

### Example 2

Login System

Correct Username

AND

Correct Password

Access Granted

### Example 3

Fire Alarm

Smoke Detected

OR

High Temperature

Alarm Sounds

### Example 4

CPU

Processors perform billions of Boolean operations every second to
execute programs.

------------------------------------------------------------------------

# 3. Boolean Operator Precedence

When no parentheses exist, Boolean expressions are evaluated in this
order:

1.  NOT
2.  AND
3.  OR

Memory Trick

NOT → AND → OR

### Example 1

A + B·C'

Step 1

C'

Step 2

B·C'

Step 3

A + (B·C')

### Example 2

A'·B + C

Step 1

A'

Step 2

A'·B

Step 3

(A'·B) + C

### Example 3

A + B'·C'

Step 1

B'

C'

Step 2

B'·C'

Step 3

A + (B'·C')

------------------------------------------------------------------------

# 4. Logical Product (AND)

## Symbol

·

Example

x · y

It behaves exactly like logical AND.

Both inputs must be 1.

Truth Table

  x   y   x·y
  --- --- -----
  0   0   0
  0   1   0
  1   0   0
  1   1   1

### Examples

Door opens only if

Key Card

AND

Fingerprint

are correct.

Both must be True.

Example

Computer starts if

Power

AND

Motherboard

work.

------------------------------------------------------------------------

# 5. Logical Sum (OR)

## Symbol

-   

Example

x + y

It behaves exactly like logical OR.

Only one input needs to be 1.

Truth Table

  x   y   x+y
  --- --- -----
  0   0   0
  0   1   1
  1   0   1
  1   1   1

### Examples

Alarm sounds if

Smoke

OR

Heat

is detected.

Example

Student passes if

Assignment

OR

Project

is completed.

------------------------------------------------------------------------

# 6. Logical Complement (NOT)

## Symbol

'

Example

x'

It reverses the value.

Truth Table

  x   x'
  --- ----
  0   1
  1   0

### Examples

Door Closed

DoorOpen'

If

DoorOpen = 1

Then

DoorOpen' = 0

Example

Light ON

Light'

means

Light OFF

------------------------------------------------------------------------

# Comparison with Propositional Logic

  Boolean Algebra   Propositional Logic
  ----------------- ---------------------
  0                 False
  1                 True
  x·y               x AND y
  x+y               x OR y
  x'                NOT x

------------------------------------------------------------------------

# Real-Life Examples

### Traffic Signal

Green = 1

Red = 0

### Mobile Unlock

Correct PIN

AND

Fingerprint

Unlock

### Emergency System

Fire

OR

Gas Leak

Alarm

### Air Conditioner

Temperature High

AND

Power Available

AC Turns ON

------------------------------------------------------------------------

# Memory Tricks

-   Boolean Algebra has only two values: **0** and **1**.
-   **0 = False = OFF**
-   **1 = True = ON**
-   Product (·) = AND
-   Sum (+) = OR
-   Complement (') = NOT
-   Evaluate expressions in the order: **NOT → AND → OR**

Boolean Algebra is the mathematical foundation of digital circuits,
logic gates, CPUs, memory chips, operating systems, compilers,
databases, networking devices, and modern computer hardware.
