# Merge Sort

These notes explain Merge Sort and its supporting concepts using simple
language, diagrams, analogies, and step-by-step examples.

## 1. Two-List Merging Technique

Two already sorted lists are combined into one sorted list by repeatedly
comparing their front elements and copying the smaller one first.

Example: - \[2,5,8\] + \[1,3,7\] - Result: \[1,2,3,5,7,8\]

Analogy: Two people each hold sorted cards. Always take the smaller top
card.

------------------------------------------------------------------------

## 2. Pointer Movement Constraint

Only one pointer moves forward after an element is copied. Pointers
never skip elements or move backward.

Example: A=\[2,5\] B=\[3,4\]

Copy 2 → move pointer A only.

------------------------------------------------------------------------

## 3. Merge Linear Time Complexity

If one list has m elements and the other has n elements, merging takes
O(m+n) time because each element is copied once.

Example: 3 elements + 5 elements = 8 total element moves.

------------------------------------------------------------------------

## 4. Exhaustion Handling (Empty List Copy)

When one list becomes empty, copy all remaining elements from the other
list directly.

Example: A=\[2,5\] B=\[3\]

Output: \[2,3,5\]

------------------------------------------------------------------------

## 5. Divide-and-Conquer Splitting Concept

Split a large problem into two smaller halves, solve each independently,
then merge them.

Example: \[8,3,5,1\] → \[8,3\] and \[5,1\] → sort each half → merge

------------------------------------------------------------------------

## 6. Continuous Splitting (Divide Phase)

Keep splitting until every sublist contains exactly one element.

Example: \[8,3,5,1\] → \[8,3\] \[5,1\] → \[8\] \[3\] \[5\] \[1\]

------------------------------------------------------------------------

## 7. Single-Entry Baseline

A list containing one element is already sorted.

Examples: \[8\] \[42\]

------------------------------------------------------------------------

## 8. Level-by-Level Merging (Combine Phase)

Merge neighboring sorted sublists until one final sorted list remains.

Example: \[8\]\[3\]\[5\]\[1\] → \[3,8\] \[1,5\] → \[1,3,5,8\]

------------------------------------------------------------------------

## 9. Ceiling Function Balance (⌈x⌉)

For an odd-sized list, the extra element is placed in the left half.

Example: 5 elements

⌈5/2⌉ = 3

Left: \[9,4,7\]

Right: \[2,6\]

------------------------------------------------------------------------

## 10. Merge Sort Algorithm

Steps: 1. Split the array. 2. Recursively sort each half. 3. Merge the
sorted halves.

Worked Example:

Original: \[8,3,5,1\]

Split: \[8,3\] \[5,1\]

Split again: \[8\] \[3\] \[5\] \[1\]

Merge: \[3,8\] \[1,5\]

Final merge: \[1,3,5,8\]

------------------------------------------------------------------------

## Time Complexity

Best: O(n log n)

Average: O(n log n)

Worst: O(n log n)

Space Complexity: O(n)

------------------------------------------------------------------------

## Merge Sort vs Quick Sort

  Merge Sort          Quick Sort
  ------------------- ---------------------------------
  Always O(n log n)   Average O(n log n), worst O(n²)
  Uses extra memory   Usually in-place
  Stable              Usually not stable
  Uses merging        Uses partitioning

------------------------------------------------------------------------

## Quick Summary

-   Two-List Merging: Combine two sorted lists.
-   Pointer Movement: Move one pointer at a time.
-   Merge Time: O(m+n).
-   Exhaustion Handling: Copy remaining elements.
-   Divide and Conquer: Split, solve, combine.
-   Continuous Splitting: Keep splitting to one element.
-   Single-Entry Baseline: One element is already sorted.
-   Level-by-Level Merging: Merge upward.
-   Ceiling Function: Left half gets the extra element.
-   Merge Sort: Recursive divide-and-conquer sorting algorithm.
