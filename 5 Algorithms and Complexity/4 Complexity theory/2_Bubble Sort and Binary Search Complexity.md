# Bubble Sort and Binary Search Complexity

These notes explain the best, average, and worst-case performance of
Bubble Sort and Binary Search using simple language, analogies, and
step-by-step examples.

------------------------------------------------------------------------

# 1. Bubble Sort Best Case

## Definition

The **best case** happens when the list is **already sorted**.

Bubble Sort makes one pass through the list.

Since no swaps occur, the algorithm stops immediately.

### Example

    [1,2,3,4,5]

Comparisons:

    n - 1

Swaps:

    0

Time Complexity:

    O(n)

### Real-Life Analogy

Imagine checking a row of books that are already arranged
alphabetically.

You only verify the order once and finish.

------------------------------------------------------------------------

# 2. Bubble Sort Worst Case

## Definition

The **worst case** happens when the list is in **reverse order**.

Every comparison causes a swap.

The algorithm performs the maximum number of passes.

### Example

    [5,4,3,2,1]

Pass 1

Largest value moves to the end.

Pass 2

Second largest moves.

Continue until sorted.

Maximum comparisons:

    n(n-1)/2

Time Complexity:

    O(n²)

### Real-Life Analogy

Imagine arranging books that are completely reversed.

Nearly every book must be moved.

------------------------------------------------------------------------

# 3. Bubble Sort Average Case

## Definition

The **average case** measures performance on randomly ordered data.

Some comparisons require swaps.

Some do not.

Overall performance still grows quadratically.

Time Complexity:

    O(n²)

### Example

    [4,1,5,2,3]

Some elements are already close to their correct positions.

Others need several swaps.

------------------------------------------------------------------------

# 4. Binary Search Best Case (Lucky Search)

## Definition

The **best case** occurs when the target is exactly the first middle
element.

Only one comparison is needed.

### Example

    [2,4,6,8,10,12,14]

Target:

    8

Middle element:

    8

Found immediately.

Comparisons:

    1

Time Complexity:

    O(1)

### Analogy

Open a dictionary exactly at the page containing the desired word.

------------------------------------------------------------------------

# 5. Binary Search Worst Case

## Definition

The **worst case** occurs when the target is at an extreme end or is not
present.

The search repeatedly halves the remaining space until nothing remains.

### Example

    [2,4,6,8,10,12,14,16]

Search:

    16

Middle:

8

↓

Search right half

↓

12

↓

Search right half

↓

14

↓

Search right half

↓

16

Maximum comparisons grow as

    O(log n)

------------------------------------------------------------------------

# 6. Binary Search Average Case

## Definition

The **average case** measures the expected number of comparisons over
all possible search targets.

Because the search space keeps halving, the average performance is also
logarithmic.

Time Complexity:

    O(log n)

### Example

Searching random values in a sorted list of 1024 elements.

Average comparisons are about

    10

instead of hundreds.

------------------------------------------------------------------------

# Worked Comparison

Find

    45

List:

    [5,10,15,20,25,30,35,40,45]

### Linear Search

Checks:

5 → 10 → 15 → 20 → 25 → 30 → 35 → 40 → 45

Comparisons:

    9

### Binary Search

Middle:

25

↓

Right half

↓

40

↓

Right half

↓

45

Comparisons:

    3

------------------------------------------------------------------------

# Complexity Summary

  Algorithm       Best   Average    Worst
  --------------- ------ ---------- ----------
  Bubble Sort     O(n)   O(n²)      O(n²)
  Binary Search   O(1)   O(log n)   O(log n)

------------------------------------------------------------------------

# Quick Summary

-   Bubble Sort Best Case: Already sorted, one pass, O(n).
-   Bubble Sort Worst Case: Reverse order, maximum swaps, O(n²).
-   Bubble Sort Average Case: Random order, O(n²).
-   Binary Search Best Case: Middle element found immediately, O(1).
-   Binary Search Worst Case: Repeated halving until end, O(log n).
-   Binary Search Average Case: Average logarithmic comparisons, O(log
    n).
