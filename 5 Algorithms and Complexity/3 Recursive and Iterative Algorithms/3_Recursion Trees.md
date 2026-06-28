# Recursion Trees

These notes explain recursion trees and important recursive concepts
using simple language, diagrams, analogies, and step-by-step examples.

------------------------------------------------------------------------

# 1. Recursion Tree

## Definition

A **Recursion Tree** is a diagram that shows every function call made
during a recursive algorithm.

Each function call is drawn as a **node**.

Children represent new recursive calls made by their parent.

The tree helps us visualize:

-   How recursion grows.
-   How many function calls occur.
-   How results return.

------------------------------------------------------------------------

## Real-Life Analogy

Imagine a family tree.

Parents create children.

Children create grandchildren.

Similarly,

one recursive call creates more recursive calls.

------------------------------------------------------------------------

## Example 1 (Factorial)

    Factorial(4)

    ↓

    Factorial(3)

    ↓

    Factorial(2)

    ↓

    Factorial(1)

Tree

    F(4)

    |

    F(3)

    |

    F(2)

    |

    F(1)

Only one branch.

------------------------------------------------------------------------

## Example 2 (Fibonacci)

    Fib(4)

    ↓

    Fib(3)

    ↓

    Fib(2)

and

    Fib(3)

    ↓

    Fib(1)

Tree

              F(4)
             /    \
          F(3)   F(2)
          /  \
       F(2) F(1)

Multiple branches.

------------------------------------------------------------------------

# 2. Base Cases (Termination States)

## Definition

A **Base Case** is a condition where recursion stops immediately.

Instead of making another recursive call,

the function directly returns an answer.

Without base cases,

recursion would continue forever.

------------------------------------------------------------------------

## Example 1

Factorial

    If n == 1

    Return 1

------------------------------------------------------------------------

## Example 2

Fibonacci

    Fib(0)=0

    Fib(1)=1

Both are base cases.

------------------------------------------------------------------------

## Real-Life Analogy

Imagine climbing down a ladder.

When you reach the ground,

you stop climbing.

------------------------------------------------------------------------

# 3. Single-Branching Recursion

## Definition

Every function call creates **exactly one** new recursive call.

The recursion tree looks like a straight chain.

------------------------------------------------------------------------

## Example

    F(5)

    ↓

    F(4)

    ↓

    F(3)

    ↓

    F(2)

    ↓

    F(1)

Only one child per node.

------------------------------------------------------------------------

## Example 2

Countdown

    5

    ↓

    4

    ↓

    3

    ↓

    2

    ↓

    1

------------------------------------------------------------------------

## Real-Life Analogy

A person calling one friend,

who calls one more friend,

and so on.

------------------------------------------------------------------------

# 4. Multi-Branching Recursion

## Definition

One recursive call creates **two or more** child calls.

The recursion tree spreads into many branches.

------------------------------------------------------------------------

## Example 1 (Fibonacci)

    F(5)

    ↓

    F(4)

    +

    F(3)

Each child creates more children.

------------------------------------------------------------------------

## Tree

                F(5)

             /        \

          F(4)       F(3)

         /    \      /   \

       F(3) F(2) F(2) F(1)

------------------------------------------------------------------------

## Example 2

Suppose

    G(2,5)

calls

    G(2,2)

    and

    G(2,3)

Then

    G(2,2)

may create even more recursive calls.

------------------------------------------------------------------------

## Real-Life Analogy

One manager assigns work to two employees.

Each employee assigns work to two more employees.

The organization tree keeps growing.

------------------------------------------------------------------------

# 5. Bottom-Up Value Propagation

## Definition

The recursion tree is solved **from the leaves upward**.

Base cases produce values first.

Those values combine to solve their parents.

Eventually the root gets its answer.

------------------------------------------------------------------------

## Example 1

Factorial

Tree

    F(4)

    |

    F(3)

    |

    F(2)

    |

    F(1)=1

Returning

    F(2)

    =

    2×1

    =

    2

    F(3)

    =

    3×2

    =

    6

    F(4)

    =

    4×6

    =

    24

The answer travels upward.

------------------------------------------------------------------------

## Example 2

Fibonacci

Leaves

    Fib(1)=1

    Fib(0)=0

Return upward

    Fib(2)

    =

    1+0

    =

    1

Then

    Fib(3)

    =

    1+1

    =

    2

Eventually

    Fib(5)=5

------------------------------------------------------------------------

## Real-Life Analogy

Imagine building a wall.

The bricks at the bottom support the bricks above.

Without the bottom layer,

the top cannot exist.

------------------------------------------------------------------------

# Complete Worked Example

Compute

    Factorial(5)

Tree

    F(5)

    |

    F(4)

    |

    F(3)

    |

    F(2)

    |

    F(1)=1

Returning

    F(2)

    =

    2

↓

    F(3)

    =

    6

↓

    F(4)

    =

    24

↓

    F(5)

    =

    120

Final Answer

    120

------------------------------------------------------------------------

# Time Complexity Examples

Factorial Recursion

    O(n)

Fibonacci (naive recursion)

    O(2^n)

because many recursive calls repeat.

------------------------------------------------------------------------

# Single vs Multi-Branching Recursion

  Single Branch        Multi Branch
  -------------------- -----------------------------
  One recursive call   Two or more recursive calls
  Looks like a chain   Looks like a tree
  Example: Factorial   Example: Fibonacci
  O(n) calls           Often exponential calls

------------------------------------------------------------------------

# Quick Summary

  -----------------------------------------------------------------------
  Concept                   Simple Meaning
  ------------------------- ---------------------------------------------
  Recursion Tree            Diagram showing every recursive function call

  Base Case                 The condition that stops recursion

  Single-Branching          One recursive call creates one child
  Recursion                 

  Multi-Branching Recursion One recursive call creates multiple children

  Bottom-Up Value           Base-case results travel upward to solve the
  Propagation               root
  -----------------------------------------------------------------------
