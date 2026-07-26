# Median of Two Sorted Arrays (LeetCode 4)

## Difficulty

**Hard**

---

## Problem Statement

Given two sorted arrays `nums1` and `nums2` of sizes `m` and `n`, return the median of the two sorted arrays.

The overall run time complexity should be **O(log(min(m, n)))**.

---

## Approach

Instead of merging both arrays, use **Binary Search** on the smaller array to find the correct partition.

1. Always perform Binary Search on the smaller array.
2. Partition both arrays into left and right halves.
3. Compare the boundary elements of both partitions.
4. If the partition is valid, calculate the median.
5. Otherwise, adjust the Binary Search range and repeat.

This approach avoids merging the arrays and satisfies the required logarithmic time complexity.

---

## Algorithm

- Perform Binary Search on the smaller array.
- Calculate partition indices for both arrays.
- Find the left and right boundary elements.
- Check whether:
  - `left1 <= right2`
  - `left2 <= right1`
- If the partition is valid:
  - For an odd total number of elements, return the maximum element of the left partition.
  - For an even total number of elements, return the average of the maximum left element and the minimum right element.
- Otherwise, adjust the Binary Search boundaries.

---

## Time Complexity

**O(log(min(m, n)))**

Binary Search is performed only on the smaller array.

---

## Space Complexity

**O(1)**

No extra space is used.

---

## Key Concepts

- Binary Search
- Partition Technique
- Divide and Conquer
- Median
- Sorted Arrays
- Optimized Searching

---

## What I Learned

- Binary Search can solve more than searching problems.
- Partitioning two sorted arrays eliminates the need for merging.
- Searching on the smaller array guarantees optimal performance.
- Correct partitioning helps calculate the median directly in logarithmic time.

---

## Pattern

**Binary Search**

---

## Difficulty

**Hard**

---

## Status

**Solved** ✅

---

## Language

**Java**

---

## Java Solution

See `Solution.java`.
