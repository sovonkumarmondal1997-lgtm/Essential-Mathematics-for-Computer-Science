# Searching and Sorting Fundamentals: Linear Search and Insertion Sort

These beginner-friendly notes explain two of the most important
introductory algorithms used in computer science.

------------------------------------------------------------------------

# 1. Sequential Search (Linear Search)

## Definition

**Sequential Search** (also called **Linear Search**) is the simplest
searching algorithm.

It starts from the **first element** and checks each element **one by
one** until:

-   the target is found, or
-   the end of the list is reached.

Think of it as reading names in a class attendance register from top to
bottom.

------------------------------------------------------------------------

## Real-Life Analogy

Suppose you're looking for your friend's name in a handwritten
attendance sheet.

You don't jump randomly.

You read:

Student 1

↓

Student 2

↓

Student 3

↓

...

until you find the name.

------------------------------------------------------------------------

## Example 1

List

    [12, 8, 25, 17, 30]

Target

    17

Search

    12 ❌

    8 ❌

    25 ❌

    17 ✅

Found after checking four numbers.

------------------------------------------------------------------------

## Example 2

Target

    50

Search

    12 ❌

    8 ❌

    25 ❌

    17 ❌

    30 ❌

Reached the end.

Result

    Not Found

------------------------------------------------------------------------

## Characteristics

Advantages

-   Very easy
-   Works on sorted and unsorted lists

Disadvantages

-   Slow for large lists

------------------------------------------------------------------------

# 2. Insertion Sort

## Definition

**Insertion Sort** builds a sorted list **one element at a time**.

Each new element is removed from the unsorted part and inserted into its
correct position in the sorted part.

Think of arranging playing cards in your hand.

------------------------------------------------------------------------

## Real-Life Analogy

Suppose you receive playing cards one by one.

Every new card is placed into its correct position among the cards you
already hold.

Eventually all cards become sorted.

------------------------------------------------------------------------

## Example

Original List

    [7, 4, 5, 2]

Initially

Sorted

    [7]

Unsorted

    [4,5,2]

Take

    4

Insert before 7

    [4,7]

Take

    5

Insert between 4 and 7

    [4,5,7]

Take

    2

Insert at beginning

    [2,4,5,7]

Finished.

------------------------------------------------------------------------

# 3. Pivot (Insertion Sort)

## Definition

The **pivot** is the element currently selected from the unsorted
section.

The algorithm tries to place this pivot into its correct position.

------------------------------------------------------------------------

## Example 1

Current list

    [3,6,8,5]

Sorted

    [3,6,8]

Pivot

    5

Compare

    5 < 8

    Shift 8

    5 < 6

    Shift 6

    5 > 3

    Insert here

Result

    [3,5,6,8]

------------------------------------------------------------------------

## Example 2

Current list

    [2,4,6,9,7]

Pivot

    7

Move

    9

Insert

    7

Result

    [2,4,6,7,9]

------------------------------------------------------------------------

# 4. Hole Mechanism

## Definition

When the pivot is temporarily removed,

an empty position (called a **hole**) is created.

Larger elements shift into the hole,

and finally the pivot fills the last remaining hole.

------------------------------------------------------------------------

## Example 1

Original

    [3,6,8,5]

Remove pivot

    5

Temporary hole

    [3,6,8,_]

Shift

    8

    [3,6,_,8]

Shift

    6

    [3,_,6,8]

Insert pivot

    [3,5,6,8]

The hole moved left until the correct location was found.

------------------------------------------------------------------------

## Example 2

Original

    [2,5,9,4]

Pivot

    4

Hole

    [2,5,9,_]

Shift

    9

↓

    [2,5,_,9]

Shift

    5

↓

    [2,_,5,9]

Insert

    4

↓

    [2,4,5,9]

------------------------------------------------------------------------

# Complete Worked Example

Sort

    [9,5,1,4]

Step 1

Sorted

    [9]

Pivot

    5

Insert

    [5,9]

------------------------------------------------------------------------

Step 2

Pivot

    1

Insert

    [1,5,9]

------------------------------------------------------------------------

Step 3

Pivot

    4

Hole

    [1,5,9,_]

Shift

    9

    ↓

    5

Insert

    4

Final

    [1,4,5,9]

------------------------------------------------------------------------

# Time Complexity

## Linear Search

  Case      Time
  --------- ------
  Best      O(1)
  Average   O(n)
  Worst     O(n)

------------------------------------------------------------------------

## Insertion Sort

  Case                     Time
  ------------------------ -------
  Best (Already Sorted)    O(n)
  Average                  O(n²)
  Worst (Reverse Sorted)   O(n²)

------------------------------------------------------------------------

# Quick Summary

  -----------------------------------------------------------------------
  Concept                   Simple Meaning
  ------------------------- ---------------------------------------------
  Sequential Search         Check every element one by one

  Insertion Sort            Build a sorted list by inserting one element
                            at a time

  Pivot                     Current element chosen from the unsorted
                            section

  Hole Mechanism            Temporary empty position created while moving
                            the pivot
  -----------------------------------------------------------------------