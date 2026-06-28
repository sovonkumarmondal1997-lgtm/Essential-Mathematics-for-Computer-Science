# Quick Sort and Partition Algorithm

These notes explain the Partition Algorithm and Quick Sort using simple
language, diagrams, real-world analogies, and step-by-step examples.

------------------------------------------------------------------------

# 1. Partition Algorithm

## Definition

The **Partition Algorithm** is the heart of **Quick Sort**.

Its job is to rearrange the list so that:

-   All elements **smaller** than the pivot are placed on the left.
-   All elements **larger** than the pivot are placed on the right.

The pivot eventually ends up in its correct sorted position.

------------------------------------------------------------------------

## Real-Life Analogy

Imagine a teacher dividing students by height.

-   Shorter students stand on the left.
-   Taller students stand on the right.
-   The teacher stands in the middle.

------------------------------------------------------------------------

## Example

Original list

    [8, 3, 7, 1, 10, 5]

Pivot = 8

After partition

    [5, 3, 7, 1, 8, 10]

Everything left of 8 is smaller.

Everything right of 8 is larger.

------------------------------------------------------------------------

# 2. Pivot (in Partition)

## Definition

The **pivot** is the reference element used to compare all other
elements.

Many implementations choose the **first element**, though other choices
are also possible.

------------------------------------------------------------------------

## Example 1

    [6, 2, 9, 4]

Pivot

    6

Compare every other element with 6.

------------------------------------------------------------------------

## Example 2

    [15, 8, 20, 5]

Pivot

    15

Elements smaller than 15 move left.

Larger ones move right.

------------------------------------------------------------------------

## Analogy

Think of the pivot as the referee who decides which side everyone
belongs on.

------------------------------------------------------------------------

# 3. Two-Pointer Approach (i and j)

## Definition

Partition often uses two pointers.

-   **i** starts from the left and moves right looking for values larger
    than the pivot.
-   **j** starts from the right and moves left looking for values
    smaller than the pivot.

------------------------------------------------------------------------

## Example

    [8, 3, 7, 1, 10, 5]

Pivot = 8

    i →

    8 3 7 1 10 5

                ← j

-   i stops at 10.
-   j stops at 5.

Swap them.

------------------------------------------------------------------------

## Analogy

Imagine two inspectors walking toward each other from opposite ends of a
hallway.

------------------------------------------------------------------------

# 4. Pointer Swapping Condition

## Definition

If **i \< j**, swap the elements at i and j.

This moves misplaced elements to the correct side of the pivot.

------------------------------------------------------------------------

## Example

Before

    [8,3,7,1,10,5]

Swap

    10 ↔ 5

After

    [8,3,7,1,5,10]

------------------------------------------------------------------------

## Another Example

    [20,6,30,9]

Swap

    30 ↔ 9

Result

    [20,6,9,30]

------------------------------------------------------------------------

# 5. Final Pivot Placement

## Definition

Eventually, the pointers cross.

When **i ≥ j**, scanning stops.

Now swap the pivot with the element at **j**.

The pivot reaches its final sorted position.

------------------------------------------------------------------------

## Example

Before

    [8,3,7,1,5,10]

Pointers cross.

Swap

    8 ↔ 5

Result

    [5,3,7,1,8,10]

Now 8 is permanently in its correct position.

------------------------------------------------------------------------

# 6. Quicksort

## Definition

**Quick Sort** is a recursive **divide-and-conquer** sorting algorithm.

Steps:

1.  Choose a pivot.
2.  Partition the list.
3.  Recursively sort the left sub-list.
4.  Recursively sort the right sub-list.

------------------------------------------------------------------------

## Example

    [8,3,7,1,10,5]

Partition

↓

    [5,3,7,1] 8 [10]

Sort the left part.

Sort the right part.

Eventually

    [1,3,5,7,8,10]

------------------------------------------------------------------------

# 7. Base Case Condition (n ≤ 1)

## Definition

A list with **0 or 1 element** is already sorted.

Recursion stops.

------------------------------------------------------------------------

## Examples

    []

Already sorted.

    [9]

Already sorted.

No further recursive calls are needed.

------------------------------------------------------------------------

# 8. Sub-list Division

## Definition

After partitioning, the list splits into two independent parts:

-   Left: smaller than pivot.
-   Right: larger than pivot.

Each part is sorted separately.

------------------------------------------------------------------------

## Example

    [5,3,7,1] 8 [10]

Left sub-list

    [5,3,7,1]

Right sub-list

    [10]

------------------------------------------------------------------------

## Analogy

Imagine dividing a large class into two smaller groups for easier
management.

------------------------------------------------------------------------

# 9. Pivot Stabilization

## Definition

Once the pivot is placed correctly, it never moves again.

Future recursive calls ignore it.

------------------------------------------------------------------------

## Example

    [5,3,7,1,8,10]

Pivot

    8

Position fixed forever.

Only

    [5,3,7,1]

needs further sorting.

------------------------------------------------------------------------

# 10. Recursive Sort Strategy

## Definition

Quick Sort repeatedly applies the same process to smaller and smaller
sub-lists until every sub-list reaches the base case.

------------------------------------------------------------------------

## Example

    [8,3,7,1,10,5]

↓

    [5,3,7,1] 8 [10]

↓

    [3,1] 5 [7]

↓

    [1] 3 []

Eventually every part has one element.

------------------------------------------------------------------------

## Analogy

Breaking a large puzzle into smaller puzzles until each puzzle contains
only one piece.

------------------------------------------------------------------------

# Complete Worked Example

Original

    [9,4,7,2,8]

Pivot = 9

Partition

    [8,4,7,2] 9

Sort left

Pivot = 8

    [2,4,7] 8

Sort left

Pivot = 2

    2 [4,7]

Sort remaining

Final

    [2,4,7,8,9]

------------------------------------------------------------------------

# Time Complexity

  Case      Complexity
  --------- ------------
  Best      O(n log n)
  Average   O(n log n)
  Worst     O(n²)

Worst case happens when poor pivots repeatedly create highly unbalanced
partitions.

------------------------------------------------------------------------

# Quick Sort vs Merge Sort

  Quick Sort                          Merge Sort
  ----------------------------------- --------------------------
  Partition around a pivot            Split exactly in half
  Usually faster in practice          Stable sorting algorithm
  In-place (common implementations)   Requires extra memory
  Worst case O(n²)                    Worst case O(n log n)

------------------------------------------------------------------------

# Quick Summary

  -----------------------------------------------------------------------
  Concept                   Simple Meaning
  ------------------------- ---------------------------------------------
  Partition Algorithm       Rearrange elements around a pivot

  Pivot                     Reference element used for comparisons

  Two-Pointer Approach      Two indices move toward each other while
                            scanning

  Pointer Swapping          Swap misplaced elements when i \< j

  Final Pivot Placement     Put the pivot into its final sorted position

  Quick Sort                Recursively partition and sort smaller
                            sub-lists

  Base Case                 Stop when a sub-list has 0 or 1 element

  Sub-list Division         Split into left and right partitions

  Pivot Stabilization       Pivot never moves again after partition

  Recursive Sort Strategy   Keep sorting smaller sub-lists recursively
  -----------------------------------------------------------------------
