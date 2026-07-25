# Search in Rotated Sorted Array (LeetCode 33)

## Difficulty
**Medium**

## Pattern
**Binary Search**

---

## Problem Statement

Given a rotated sorted array `nums` with distinct integers and an integer `target`, return the index of `target` if it exists in the array. Otherwise, return `-1`.

Your solution must run in **O(log n)** time.

---

## Approach

A rotated sorted array always has at least one half that is sorted.

1. Initialize two pointers:
   - `left = 0`
   - `right = nums.length - 1`

2. Find the middle index using the overflow-safe formula:

   ```
   mid = left + (right - left) / 2
   ```

3. If the middle element is the target, return its index.

4. Check which half is sorted:
   - If the left half is sorted:
     - Check whether the target lies within that range.
     - Search the left half if it does; otherwise, search the right half.
   - Otherwise, the right half is sorted:
     - Check whether the target lies within that range.
     - Search the right half if it does; otherwise, search the left half.

5. Continue until the target is found or the search space becomes empty.

6. Return `-1` if the target does not exist.

---

## Algorithm

- Initialize `left` and `right`.
- Repeat while `left <= right`:
  - Calculate the middle index.
  - If the middle element equals the target, return its index.
  - Determine which half is sorted.
  - Check whether the target belongs to the sorted half.
  - Eliminate the other half.
- Return `-1` if the target is not found.

---

## Time Complexity

**O(log n)**

The search space is reduced by half during every iteration.

---

## Space Complexity

**O(1)**

No extra space is used.

---

## Key Concepts

- Binary Search
- Modified Binary Search
- Rotated Sorted Array
- Divide and Conquer
- Sorted Half Identification
- Overflow-safe Mid Calculation

---

## What I Learned

- Binary Search can be applied even when a sorted array has been rotated.
- At every iteration, at least one half of the array remains sorted.
- Identifying the sorted half helps determine where the target can exist.
- This problem strengthened my understanding of applying Binary Search beyond standard sorted arrays.

---
Pattern
Binary Search
---
Status
✅ Solved

## Java Solution

See `Solution.java`.
