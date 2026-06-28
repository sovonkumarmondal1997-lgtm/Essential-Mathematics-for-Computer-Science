# Heap Sort

These notes explain Heap Sort using simple language, diagrams,
analogies, and step-by-step examples.

------------------------------------------------------------------------

# 1. Heap Sort

## Definition

**Heap Sort** is a comparison-based sorting algorithm that uses a
**heap** (Max-Heap or Min-Heap) to sort data.

The basic idea is:

1.  Build a heap.
2.  Repeatedly remove the root element.
3.  Restore the heap.
4.  Continue until all elements are removed.

The extracted elements become the sorted list.

------------------------------------------------------------------------

## Real-Life Analogy

Imagine picking books from a shelf.

Every time you always take the **smallest** book first.

After removing it, you rearrange the remaining books and repeat.

Eventually the books are completely sorted.

------------------------------------------------------------------------

## Example

Numbers

    8 3 6 2 5

Min-Heap

            2
          /   \
         3     6
        / \
       8   5

Extract:

    2 → 3 → 5 → 6 → 8

Sorted result

    [2,3,5,6,8]

------------------------------------------------------------------------

# 2. Root Extraction (Minimum Retrieval)

## Definition

In a **Min-Heap**, the root always contains the **smallest** value.

Therefore every extraction removes the minimum remaining element.

------------------------------------------------------------------------

## Example 1

            4
          /   \
         8    10

Remove

    4

Remaining values

    8 10

------------------------------------------------------------------------

## Example 2

            1
          /   \
         5     7

First extracted value

    1

------------------------------------------------------------------------

## Analogy

The winner of a race always stands first.

The first person is removed before considering the others.

------------------------------------------------------------------------

# 3. Root Replacement Rule

## Definition

After removing the root, the tree would have an empty space.

To keep the tree **complete**, move the **last (bottom-right) leaf** to
the root.

Then repair the heap.

------------------------------------------------------------------------

## Example

Before

            2
          /   \
         4     6
        /
       9

Remove

    2

Move last node

    9

to root.

            9
          /   \
         4     6

Heap property may now be broken.

------------------------------------------------------------------------

## Analogy

If the captain leaves the front of a line, the last person temporarily
moves to the front before everyone reorganizes.

------------------------------------------------------------------------

# 4. Re-Heapification (Re-Heapify)

## Definition

After replacing the root, run **Heapify only from the root downward**.

The misplaced element moves down until the heap property is restored.

------------------------------------------------------------------------

## Example

            9
          /   \
         4     6

Swap

    9 ↔ 4

Result

            4
          /   \
         9     6

Now every parent is smaller than its children.

------------------------------------------------------------------------

## Another Example

            20
          /    \
        10      15

Swap

    20 ↔ 10

Continue downward if necessary.

------------------------------------------------------------------------

# 5. Secondary Storage List

## Definition

Each extracted root is placed into another list.

Eventually this secondary list contains all values in sorted order.

------------------------------------------------------------------------

## Example

Heap

    2 3 5 6 8

Extraction sequence

    2

    ↓

    3

    ↓

    5

    ↓

    6

    ↓

    8

Secondary list

    [2,3,5,6,8]

------------------------------------------------------------------------

## Analogy

Imagine taking books off a shelf one by one and placing them neatly onto
another shelf in order.

------------------------------------------------------------------------

# Complete Worked Example

Numbers

    7 2 9 4

Min-Heap

          2
        /   \
       4     9
      /
     7

### Step 1

Extract

    2

Sorted list

    [2]

Replace root with

    7

Tree

          7
        /   \
       4     9

Heapify

          4
        /   \
       7     9

### Step 2

Extract

    4

Sorted

    [2,4]

Replace with

    9

Heapify

          7
         /
        9

### Step 3

Extract

    7

Sorted

    [2,4,7]

### Step 4

Extract

    9

Final sorted list

    [2,4,7,9]

------------------------------------------------------------------------

# Time Complexity

  Operation            Complexity
  -------------------- ------------
  Build Heap           O(n)
  Each Extraction      O(log n)
  Complete Heap Sort   O(n log n)

------------------------------------------------------------------------

# Advantages

-   Guaranteed O(n log n)
-   In-place sorting (common implementation)
-   No worst-case slowdown like Quick Sort

------------------------------------------------------------------------

# Quick Summary

  -----------------------------------------------------------------------
  Concept                   Simple Meaning
  ------------------------- ---------------------------------------------
  Heap Sort                 Sort by repeatedly removing the heap root

  Root Extraction           Remove the smallest (Min-Heap) or largest
                            (Max-Heap) element

  Root Replacement Rule     Move the last leaf to the root

  Re-Heapification          Restore the heap by pushing the root downward

  Secondary Storage List    Collect extracted elements to form the sorted
                            sequence
  -----------------------------------------------------------------------
