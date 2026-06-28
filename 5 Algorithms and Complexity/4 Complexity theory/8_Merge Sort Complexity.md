# Merge Sort Complexity

These notes explain why Merge Sort has the same time complexity in every
case and how its recurrence is analyzed using the Master Theorem.

------------------------------------------------------------------------

# 1. Merge Sort Case Uniformity

## Definition

**Merge Sort Case Uniformity** means that the **best case, average case,
and worst case all have the same time complexity:**

    O(n log n)

This happens because Merge Sort **always** performs the same two major
steps:

1.  Split the array into two halves.
2.  Merge the two sorted halves.

The initial order of the data does **not** change these steps.

### Example 1

Already sorted array

    [1,2,3,4,5,6,7,8]

Merge Sort still splits into halves until single elements and then
merges them.

### Example 2

Reverse sorted array

    [8,7,6,5,4,3,2,1]

Exactly the same splitting and merging process occurs.

### Real-Life Analogy

Imagine cutting a cake exactly in half every time.

Whether the cake is chocolate or vanilla, you still make the same cuts.

------------------------------------------------------------------------

# 2. Divide-and-Conquer Recurrence

## Definition

Merge Sort is described by

    T(n)=2T(n/2)+cn

Meaning:

-   Two recursive subproblems of size n/2.
-   Linear work (cn) to merge them.

### Example

Array

    [8,3,5,1]

Split into

    [8,3]

    [5,1]

Sort each half recursively.

Merge them back together.

------------------------------------------------------------------------

# 3. Linear-Time Merging Work (cn)

## Definition

After both halves are sorted, they must be merged.

Every element is copied exactly once during one merge.

Therefore merging takes

    cn

where c is a constant.

### Example

Merge

    [2,5,8]

    and

    [1,3,7]

Output

    [1,2,3,5,7,8]

All six elements are processed once.

### Another Example

    [4,9]

    and

    [2,6]

↓

    [2,4,6,9]

------------------------------------------------------------------------

# 4. Merge Sort Master Theorem Proof

Recurrence

    T(n)=2T(n/2)+cn

Parameters

    a=2

    b=2

    d=1

Compute

    log₂2=1

Since

    d = log_b(a)

Merge Sort satisfies the **Balanced-Work Case**.

Master Theorem immediately gives

    O(n log n)

### Why?

Every recursion level performs about

    n

units of work.

There are

    log n

levels.

Therefore

    n × log n

gives

    O(n log n)

------------------------------------------------------------------------

# Worked Example

Sort

    [8,3,5,1]

Split

    [8,3]

    [5,1]

↓

    [8][3][5][1]

Merge

    [3,8]

    [1,5]

Final merge

    [1,3,5,8]

The same sequence of splitting and merging happens whether the input
starts sorted, reverse sorted, or random.

------------------------------------------------------------------------

# Complexity Summary

  Case      Time Complexity   Reason
  --------- ----------------- ----------------------------
  Best      O(n log n)        Same splitting and merging
  Average   O(n log n)        Same recursion pattern
  Worst     O(n log n)        Same recursion pattern

------------------------------------------------------------------------

# Master Theorem Summary

  Parameter                 Value
  ------------------ ------------
  a                             2
  b                             2
  d                             1
  log_b(a)                      1
  Case                   Balanced
  Final Complexity     O(n log n)

------------------------------------------------------------------------

# Quick Summary

-   Merge Sort always performs the same recursive splitting.
-   The merge step always processes every element once.
-   Its recurrence is:

```{=html}
<!-- -->
```
    T(n)=2T(n/2)+cn

-   Using the Master Theorem:
    -   a = 2
    -   b = 2
    -   d = 1
-   Since d = log_b(a), Merge Sort belongs to the Balanced-Work Case.
-   Best, average, and worst cases are all:

```{=html}
<!-- -->
```
    O(n log n)
