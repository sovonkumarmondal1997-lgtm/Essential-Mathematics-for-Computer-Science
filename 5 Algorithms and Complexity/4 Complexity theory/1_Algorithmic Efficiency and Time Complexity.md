# Algorithmic Efficiency and Time Complexity

These notes explain algorithm efficiency and complexity using simple
language, analogies, and examples.

------------------------------------------------------------------------

# 1. Algorithmic Efficiency

**Algorithmic Efficiency** studies how an algorithm's **time** and
**memory** change as the input size grows.

### Example

Two algorithms sort 1,000 numbers.

-   Algorithm A: 1 second
-   Algorithm B: 10 seconds

Algorithm A is more efficient.

**Analogy:** Two cars travel the same distance. The one using less fuel
and time is more efficient.

------------------------------------------------------------------------

# 2. Time Complexity Analysis

Time complexity describes how the running time changes when the input
size `n` increases.

### Example

Linear Search

    10 items → about 10 checks
    100 items → about 100 checks

The work grows with `n`.

------------------------------------------------------------------------

# 3. Comparative Algorithm Analysis

Compare algorithms using standard complexity measures.

### Example

Find a number in 1,000 sorted values.

-   Linear Search: up to 1000 comparisons
-   Binary Search: about 10 comparisons

Binary Search is much faster.

------------------------------------------------------------------------

# 4. Two-Phone Durability Riddle (Egg Dropping Variant)

Imagine a 100-floor building and **2 phones** that may break if dropped.

Goal: Find the highest safe floor using the fewest worst-case drops.

A naive strategy checks every floor.

A smarter strategy jumps by decreasing intervals (for example 14, then
13, then 12...) to balance the worst case.

This puzzle teaches optimization under limited resources.

------------------------------------------------------------------------

# 5. Time Complexity Performance Measuring

We measure **how execution time grows**, not the exact seconds.

Example:

    n = 100

    ↓

    Algorithm A: 100 steps

    Algorithm B: 10,000 steps

Algorithm A scales better.

------------------------------------------------------------------------

# 6. Sequential vs Binary Search Efficiency

Sequential Search:

Checks one item after another.

Time:

    O(n)

Binary Search:

Cuts the remaining search space in half each step.

Time:

    O(log n)

Example:

1,024 elements

-   Linear Search: up to 1024 checks
-   Binary Search: about 10 checks

------------------------------------------------------------------------

# 7. Worst-Case Complexity

The maximum work an algorithm may ever perform.

### Example

Searching for the last element in:

    [5,8,2,7,9]

Every element is checked.

Worst case:

    5 comparisons

------------------------------------------------------------------------

# 8. Average-Case Complexity

The expected running time across all possible inputs.

### Example

Searching random elements in a list of 100 items.

On average, about 50 comparisons are needed.

------------------------------------------------------------------------

# 9. Best-Case Complexity

The minimum work under ideal conditions.

### Example

Searching for the first element.

Only one comparison is needed.

Best case:

    O(1)

------------------------------------------------------------------------

# 10. Insertion Sort Best Case

Occurs when the array is already sorted.

Example:

    [1,2,3,4,5]

Each element is compared once.

Comparisons:

    n - 1

Time:

    O(n)

------------------------------------------------------------------------

# 11. Insertion Sort Worst Case

Occurs when the array is reverse sorted.

Example:

    [5,4,3,2,1]

Every element shifts past all previous elements.

Maximum shifts:

n(n−1)/2

Time:

    O(n²)

------------------------------------------------------------------------

# Worked Example

Search for 18:

    [3,6,9,12,15,18,21]

Linear Search:

3 → 6 → 9 → 12 → 15 → 18

6 comparisons.

Binary Search:

Middle = 12

18 \> 12

Search right half.

Middle = 18

Found.

Only 2 comparisons.

------------------------------------------------------------------------

# Complexity Summary

  Algorithm          Best    Average      Worst
  ---------------- ------ ---------- ----------
  Linear Search      O(1)       O(n)       O(n)
  Binary Search      O(1)   O(log n)   O(log n)
  Insertion Sort     O(n)      O(n²)      O(n²)

------------------------------------------------------------------------

# Quick Summary

-   Algorithmic Efficiency: Measure time and memory growth.
-   Time Complexity: Relationship between input size and running time.
-   Comparative Analysis: Compare algorithms using complexity.
-   Egg Dropping Variant: Optimize worst-case strategy.
-   Sequential vs Binary Search: O(n) vs O(log n).
-   Worst Case: Maximum work.
-   Average Case: Typical work.
-   Best Case: Minimum work.
-   Insertion Sort Best: Already sorted, O(n).
-   Insertion Sort Worst: Reverse sorted, O(n²).
