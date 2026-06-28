# Binary Trees and Heaps

These notes explain Binary Trees, Complete Binary Trees, Array
Representation, Max-Heaps, and Min-Heaps using simple language,
diagrams, and examples.

------------------------------------------------------------------------

# 1. Binary Tree

## Definition

A **Binary Tree** is a tree data structure in which every node has **at
most two children**:

-   Left child
-   Right child

A binary tree always starts from one special node called the **root**.

------------------------------------------------------------------------

## Simple Diagram

            A
           / \
          B   C
         / \
        D   E

Here:

-   A is the root.
-   B and C are children of A.
-   D and E are children of B.

------------------------------------------------------------------------

## Real-Life Analogy

Think of a family tree.

Each person may have:

-   Left child
-   Right child

but never more than two children in a binary tree.

------------------------------------------------------------------------

## Example 1

            10
           /  \
          5    20

Root = 10

Children = 5 and 20

------------------------------------------------------------------------

## Example 2

            50
           /
         30
           \
            40

Still a valid binary tree because each node has at most two children.

------------------------------------------------------------------------

# 2. Complete Binary Tree

## Definition

A **Complete Binary Tree** is a binary tree where:

-   Every level is completely filled,
-   except possibly the last level.
-   The last level is filled **from left to right**.

------------------------------------------------------------------------

## Valid Example

            1
          /   \
         2     3
        / \   /
       4  5  6

Last level:

    4 5 6

Nodes are packed to the left.

------------------------------------------------------------------------

## Invalid Example

            1
          /   \
         2     3
          \   /
           5 6

Node 2 is missing its left child.

Not complete.

------------------------------------------------------------------------

## Real-Life Analogy

Imagine people taking seats in a theater.

Everyone fills seats from left to right.

Nobody skips an empty seat.

------------------------------------------------------------------------

# 3. Tree Array Representation

## Definition

A complete binary tree can be stored inside an array.

If the root starts at index **1**:

-   Parent = i
-   Left Child = 2i
-   Right Child = 2i + 1

------------------------------------------------------------------------

## Example

Tree

            10
          /    \
         20     30
        / \     /
       40 50   60

Array

  Index   1    2    3    4    5    6
  ------- ---- ---- ---- ---- ---- ----
  Value   10   20   30   40   50   60

------------------------------------------------------------------------

### Parent of index 2

    20

Children

Left

    2×2 = 4

    ↓

    40

Right

    2×2+1=5

    ↓

    50

------------------------------------------------------------------------

### Parent of index 3

    30

Left child

    6

    ↓

    60

Right child

    7

    ↓

    None

------------------------------------------------------------------------

# 4. Max-Heap

## Definition

A **Max-Heap** is a Complete Binary Tree where:

Every parent node is **greater than or equal to** its children.

The largest value is always at the root.

------------------------------------------------------------------------

## Example

            90
          /    \
         70     60
        / \    /
       40 50 20

Check

    90 > 70

    90 > 60

    70 > 40

    70 > 50

    60 > 20

All conditions are satisfied.

------------------------------------------------------------------------

## Invalid Example

           40
          /  \
         60  30

Parent

    40

is smaller than child

    60

Not a Max-Heap.

------------------------------------------------------------------------

## Real-Life Analogy

A company hierarchy.

The CEO has the highest authority.

Managers have less.

Employees have even less.

------------------------------------------------------------------------

# 5. Min-Heap

## Definition

A **Min-Heap** is a Complete Binary Tree where:

Every parent node is **smaller than or equal to** its children.

The smallest value is always at the root.

------------------------------------------------------------------------

## Example

            10
          /    \
         20     30
        / \    /
       40 50 60

Check

    10 < 20

    10 < 30

    20 < 40

    20 < 50

    30 < 60

Correct Min-Heap.

------------------------------------------------------------------------

## Invalid Example

            30
          /    \
         20     40

Parent

    30

is larger than

    20

Not a Min-Heap.

------------------------------------------------------------------------

## Real-Life Analogy

A race.

The winner stands first.

Everyone else finishes later.

------------------------------------------------------------------------

# Complete Worked Example

Numbers

    90 70 60 40 50 20

Stored as Max-Heap

            90
          /    \
         70     60
        / \    /
       40 50 20

Array Representation

  Index   1    2    3    4    5    6
  ------- ---- ---- ---- ---- ---- ----
  Value   90   70   60   40   50   20

Example

Parent

    Index 2

    ↓

    70

Children

    Index 4

    ↓

    40

    Index 5

    ↓

    50

Heap property

    70 > 40

    70 > 50

Correct.

------------------------------------------------------------------------

# Time Complexity

Access root

    O(1)

Insert into heap

    O(log n)

Delete root

    O(log n)

------------------------------------------------------------------------

# Max-Heap vs Min-Heap

  Max-Heap                    Min-Heap
  --------------------------- --------------------------
  Largest at root             Smallest at root
  Parent ≥ Children           Parent ≤ Children
  Used for highest priority   Used for lowest priority

------------------------------------------------------------------------

# Quick Summary

  -----------------------------------------------------------------------
  Concept                   Simple Meaning
  ------------------------- ---------------------------------------------
  Binary Tree               Every node has at most two children

  Complete Binary Tree      Levels filled from left to right

  Tree Array Representation Store tree in an array using index formulas

  Max-Heap                  Parent is always greater than or equal to its
                            children

  Min-Heap                  Parent is always smaller than or equal to its
                            children
  -----------------------------------------------------------------------
