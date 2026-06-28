# Binary Search

These notes explain Binary Search and its core concepts using simple
language, practical analogies, and step-by-step examples.

------------------------------------------------------------------------

# 1. Sorted List Advantage

## Definition

A **sorted list** has all elements arranged in order (ascending or
descending).

Because of this order, every element tells you something about its
neighbors:

-   All elements before it are smaller (ascending order).
-   All elements after it are larger (ascending order).

This extra information allows faster searching.

------------------------------------------------------------------------

## Example 1

Sorted list

    [5, 10, 15, 20, 25, 30]

Look at

    20

You immediately know:

Left side

    5,10,15

are smaller.

Right side

    25,30

are larger.

------------------------------------------------------------------------

## Example 2

Searching for

    28

When you see

    20

you already know

    5

    10

    15

cannot possibly be 28.

No need to check them.

------------------------------------------------------------------------

## Real-Life Analogy

Dictionary.

Words are alphabetically sorted.

If searching for

    Tiger

you never start from page 1.

------------------------------------------------------------------------

# 2. Binary Search

## Definition

Binary Search is a fast searching algorithm that repeatedly divides a
**sorted list** into two halves until the target is found.

It only works on **sorted data**.

------------------------------------------------------------------------

## Example

Sorted list

    [2,4,6,8,10,12,14]

Target

    10

Middle

    8

Since

    10 > 8

search only the right half.

New list

    [10,12,14]

Middle

    12

Since

    10 < 12

search left.

Answer

    10

Found.

------------------------------------------------------------------------

## Real-Life Analogy

Finding a word in a dictionary by repeatedly opening near the middle.

------------------------------------------------------------------------

# 3. Search Space Halving

## Definition

Every comparison removes **half of the remaining elements**.

This is why Binary Search is much faster than Linear Search.

------------------------------------------------------------------------

## Example

List has

    16

elements.

Step 1

    16

    ↓

    8

Step 2

    8

    ↓

    4

Step 3

    4

    ↓

    2

Step 4

    2

    ↓

    1

Only four comparisons were needed.

------------------------------------------------------------------------

## Example 2

One million elements.

Binary Search checks only about

    20

middle values instead of one million sequential comparisons.

------------------------------------------------------------------------

# 4. Pivot (Binary Search)

## Definition

The **pivot** is the middle element of the current search space.

Every decision is based on comparing the target with the pivot.

------------------------------------------------------------------------

## Example

List

    [10,20,30,40,50]

Pivot

    30

Searching

    50

Since

    50 > 30

search only

    40,50

------------------------------------------------------------------------

## Example 2

Searching

    20

Since

    20 < 30

search only

    10,20

------------------------------------------------------------------------

# 5. Splitting Procedure

## Definition

After comparing the target with the pivot,

one half is discarded.

Only the remaining half is searched.

------------------------------------------------------------------------

## Example

List

    [5,10,15,20,25,30,35]

Target

    30

Pivot

    20

Discard

    5

    10

    15

Continue with

    25

    30

    35

------------------------------------------------------------------------

## Real-Life Analogy

Imagine looking for a page in a book.

You instantly throw away half the pages because you know the answer
cannot be there.

------------------------------------------------------------------------

# 6. Recursive Search Function

## Definition

A recursive Binary Search solves the problem by calling itself on the
smaller search space.

Each recursive call searches only half of the previous list.

------------------------------------------------------------------------

## Example

Search

    50

List

    [10,20,30,40,50,60]

Call 1

Search entire list.

↓

Call 2

Search

    [40,50,60]

↓

Call 3

Search

    [50]

Found.

------------------------------------------------------------------------

## Real-Life Analogy

Imagine asking someone to search one room.

If not found,

they search only half of the remaining rooms,

repeating the process.

------------------------------------------------------------------------

# 7. Algorithmic Efficiency Comparison

## Definition

Different algorithms solve the same problem with different numbers of
comparisons.

Fewer comparisons usually means faster execution.

------------------------------------------------------------------------

## Example

Find

    99

inside

    100 numbers

Linear Search

Worst case

    100 comparisons

Binary Search

Worst case

    About 7 comparisons

Huge improvement.

------------------------------------------------------------------------

## Another Example

One million numbers.

Linear Search

    1,000,000 comparisons

Binary Search

    About 20 comparisons

------------------------------------------------------------------------

# Complete Worked Example

Sorted List

    [3,6,9,12,15,18,21,24]

Target

    18

Step 1

Pivot

    12

18 \> 12

↓

Search

    15,18,21,24

------------------------------------------------------------------------

Step 2

Pivot

    18

Found.

------------------------------------------------------------------------

Comparisons

Only

    2

------------------------------------------------------------------------

# Time Complexity

## Linear Search

  Case      Time
  --------- ------
  Best      O(1)
  Average   O(n)
  Worst     O(n)

------------------------------------------------------------------------

## Binary Search

  Case      Time
  --------- ----------
  Best      O(1)
  Average   O(log n)
  Worst     O(log n)

------------------------------------------------------------------------

# Binary Search vs Linear Search

  Linear Search       Binary Search
  ------------------- ----------------------------
  Works on any list   Requires sorted list
  Checks one by one   Removes half every step
  O(n)                O(log n)
  Simple              Much faster for large data

------------------------------------------------------------------------

# Quick Summary

  -----------------------------------------------------------------------
  Concept                   Simple Meaning
  ------------------------- ---------------------------------------------
  Sorted List Advantage     Order tells which half can be ignored

  Binary Search             Search by repeatedly dividing the list into
                            halves

  Search Space Halving      Remove half the elements after every
                            comparison

  Pivot                     Middle element used for comparison

  Splitting Procedure       Keep only the half that may contain the
                            target

  Recursive Search Function Search function repeatedly calls itself on a
                            smaller list

  Algorithmic Efficiency    Compare algorithms by the number of
                            comparisons they perform
  -----------------------------------------------------------------------
