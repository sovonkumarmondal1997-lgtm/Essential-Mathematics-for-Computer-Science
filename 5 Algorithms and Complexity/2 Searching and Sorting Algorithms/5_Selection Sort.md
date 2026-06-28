# Selection Sort

These notes explain Selection Sort and its important concepts using
simple language, real-world analogies, and step-by-step examples.

------------------------------------------------------------------------

# 1. Selection Sort

## Definition

**Selection Sort** is a simple sorting algorithm that repeatedly finds
the **smallest element** from the unsorted part of the list and places
it at the beginning of that unsorted section.

Unlike Bubble Sort, Selection Sort does **not** repeatedly swap
neighboring elements. Instead, it performs **one swap per pass** after
finding the smallest value.

------------------------------------------------------------------------

## Real-Life Analogy

Imagine arranging books by height.

1.  Look at all the unsorted books.
2.  Find the shortest book.
3.  Place it in the first empty position.
4.  Repeat for the remaining books.

------------------------------------------------------------------------

## Example 1

Original list

    [5, 2, 8, 1]

Find smallest:

    1

Swap with first element.

    [1, 2, 8, 5]

Next pass searches only

    [2, 8, 5]

------------------------------------------------------------------------

## Example 2

Original

    [7, 4, 3, 9]

Smallest

    3

Swap with 7

    [3,4,7,9]

------------------------------------------------------------------------

# 2. Left-to-Right Growth

## Definition

The sorted portion grows **from left to right**.

After every pass, one more element is permanently placed into its
correct position.

------------------------------------------------------------------------

## Example

Original

    [6,4,2,8]

Pass 1

    [2,4,6,8]

Sorted part

    [2]

Pass 2

    [2,4,6,8]

Sorted part

    [2,4]

The sorted section keeps growing toward the right.

------------------------------------------------------------------------

## Real-Life Analogy

Students stand in a line from shortest to tallest.

Each time you correctly place one student at the front, the sorted line
grows from left to right.

------------------------------------------------------------------------

# 3. Dynamic Start Boundary

## Definition

After each pass, the first element of the unsorted section becomes
sorted.

Therefore, the algorithm starts searching from the **next index**.

The starting boundary moves one position to the right.

------------------------------------------------------------------------

## Example

Original

    [9,5,2,7]

Pass 1

Search

    Entire list

Pass 2

Search only

    [5,9,7]

Pass 3

Search only

    [9,7]

The unsorted area becomes smaller.

------------------------------------------------------------------------

# 4. Minimum Element Selection

## Definition

Selection Sort keeps track of the smallest value found while scanning
the unsorted section.

It remembers:

-   minimum value
-   minimum index

Whenever a smaller value is found, the stored minimum is updated.

------------------------------------------------------------------------

## Example

Current list

    [6,3,8,2]

Initially

    Minimum = 6

Compare

    3 < 6

    ↓

    Minimum = 3

Compare

    8

    ↓

    No change

Compare

    2 < 3

    ↓

    Minimum = 2

Finally

    Minimum = 2

------------------------------------------------------------------------

## Real-Life Analogy

Imagine choosing the shortest student in a classroom.

Every time you find someone shorter, you change your choice.

------------------------------------------------------------------------

# 5. In-Place Swapping

## Definition

After finding the smallest element, Selection Sort swaps it directly
with the first element of the unsorted section.

The swap happens inside the same list.

No extra list is created.

------------------------------------------------------------------------

## Example 1

Current

    [7,3,5,2]

Minimum

    2

Swap

    7

    ↓

    2

Result

    [2,3,5,7]

------------------------------------------------------------------------

## Example 2

Current

    [8,4,6]

Minimum

    4

Swap

    8

    ↓

    4

Result

    [4,8,6]

------------------------------------------------------------------------

## Real-Life Analogy

Two students exchange seats.

No new seats are added.

Only their positions change.

------------------------------------------------------------------------

# Complete Worked Example

Sort

    [9,4,6,2]

------------------------------------------------------------------------

Pass 1

Smallest

    2

Swap

    [2,4,6,9]

Sorted

    [2]

------------------------------------------------------------------------

Pass 2

Search

    [4,6,9]

Smallest

    4

Already correct.

No swap needed.

------------------------------------------------------------------------

Pass 3

Search

    [6,9]

Smallest

    6

Already correct.

------------------------------------------------------------------------

Finished

    [2,4,6,9]

------------------------------------------------------------------------

# Time Complexity

  Case      Time
  --------- -------
  Best      O(n²)
  Average   O(n²)
  Worst     O(n²)

Selection Sort always scans the remaining unsorted portion, even if the
list is already sorted.

------------------------------------------------------------------------

# Space Complexity

    O(1)

Only a few temporary variables are used.

------------------------------------------------------------------------

# Bubble Sort vs Selection Sort

  Bubble Sort                    Selection Sort
  ------------------------------ -------------------------------
  Swaps many times               Usually one swap per pass
  Largest moves to end           Smallest moves to front
  Compares neighbors             Searches entire unsorted part
  Sorted part grows from right   Sorted part grows from left

------------------------------------------------------------------------

# Quick Summary

  -----------------------------------------------------------------------
  Concept                   Simple Meaning
  ------------------------- ---------------------------------------------
  Selection Sort            Repeatedly find the smallest element and
                            place it first

  Left-to-Right Growth      Sorted section grows from the left

  Dynamic Start Boundary    Search begins one position later after each
                            pass

  Minimum Element Selection Continuously track the smallest value

  In-Place Swapping         Swap the smallest element into its correct
                            position without extra memory
  -----------------------------------------------------------------------
