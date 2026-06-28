# Heapify Algorithm

These notes explain Heapify and its important concepts using simple
language, diagrams, real-world analogies, and step-by-step examples.

------------------------------------------------------------------------

# 1. Heapify Algorithm

## Definition

**Heapify** is the process of converting an **unordered Complete Binary
Tree** into a valid **Max-Heap** or **Min-Heap**.

Instead of inserting elements one by one, Heapify rearranges existing
elements so the heap property becomes true.

------------------------------------------------------------------------

## Real-Life Analogy

Imagine arranging children by height.

Initially they stand randomly.

You repeatedly rearrange them until every parent is taller (Max-Heap) or
shorter (Min-Heap) than their children.

------------------------------------------------------------------------

## Example 1 (Min-Heap)

Original tree

            20
          /    \
         5      8
        / \
       12 15

Parent 20 is larger than child 5.

After Heapify

            5
          /   \
        12     8
       / \
     20 15

Now every parent is smaller than its children.

------------------------------------------------------------------------

## Example 2 (Max-Heap)

Original

          10
         /  \
        40   30

After Heapify

          40
         /  \
       10    30

------------------------------------------------------------------------

# 2. Bottom-Up Evaluation

## Definition

Heapify starts from the **lowest non-leaf node** and moves upward toward
the root.

Leaves are already valid heaps because they have no children.

------------------------------------------------------------------------

## Example

            9
          /   \
         6     4
        / \
       8   2

Process order

    Node 6

    ↓

    Node 9

The root is processed last.

------------------------------------------------------------------------

## Real-Life Analogy

When building a wall, you complete the lower bricks before the top ones.

------------------------------------------------------------------------

# 3. Min-Heap Violation Correction (Swapping)

## Definition

If a parent is **larger** than one of its children in a Min-Heap, swap
it with the **smallest child**.

This restores the heap property.

------------------------------------------------------------------------

## Example 1

          18
         /  \
        5   12

Since

    18 > 5

Swap them.

          5
         / \
       18  12

------------------------------------------------------------------------

## Example 2

          30
         /  \
        10   20

Smallest child is 10.

Swap.

          10
         /  \
        30  20

------------------------------------------------------------------------

# 4. Cascade Effect (Trickle Down)

## Definition

After a swap, the moved element may still violate the heap property
lower in the tree.

Therefore it keeps moving downward until no violation remains.

This repeated movement is called **Trickle Down** or **Cascade Effect**.

------------------------------------------------------------------------

## Example

Original

            50
          /    \
        20      30
       / \
     10  40

Step 1

Swap 50 and 20

            20
          /    \
        50      30
       / \
     10  40

Step 2

50 is still larger than 10.

Swap again.

            20
          /    \
        10      30
       / \
     50  40

Now the heap property is satisfied.

------------------------------------------------------------------------

## Real-Life Analogy

A heavy stone dropped into water keeps sinking until it reaches the
bottom.

------------------------------------------------------------------------

# Complete Worked Example

Convert into a Min-Heap.

Original

            25
          /    \
        40      30
       / \
     10  50

### Step 1

Lowest non-leaf node:

    40

Compare with

    10

    50

Swap with 10.

            25
          /    \
        10      30
       / \
     40  50

### Step 2

Move to root.

Compare

    25

    10

    30

Swap with 10.

            10
          /    \
        25      30
       / \
     40  50

### Final Heap

Every parent is smaller than its children.

------------------------------------------------------------------------

# Time Complexity

Building a heap using Heapify

    O(n)

Heapify on one node

    O(log n)

------------------------------------------------------------------------

# Quick Summary

  -----------------------------------------------------------------------
  Concept                   Simple Meaning
  ------------------------- ---------------------------------------------
  Heapify Algorithm         Convert an unordered complete binary tree
                            into a valid heap

  Bottom-Up Evaluation      Start from the lowest non-leaf node and move
                            upward

  Min-Heap Violation        Swap a parent with its smallest child when
  Correction                needed

  Cascade Effect (Trickle   Continue pushing a swapped node downward
  Down)                     until the heap property is restored
  -----------------------------------------------------------------------
