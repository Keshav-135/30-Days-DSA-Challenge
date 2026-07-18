# Contains Duplicate II (LeetCode 219)

## Difficulty
**Easy**

## Pattern
**Sliding Window + HashSet**

---

## Problem Statement

Given an integer array `nums` and an integer `k`, determine whether there are two distinct indices `i` and `j` such that:

- `nums[i] == nums[j]`
- `|i - j| <= k`

Return `true` if such a pair exists, otherwise return `false`.

---

## Approach

1. Use a `HashSet` to represent the current sliding window.
2. Traverse the array from left to right.
3. If the current element already exists in the `HashSet`, return `true`.
4. Otherwise, add the current element to the window.
5. If the window size exceeds `k`, remove the leftmost element to maintain a window of size `k`.
6. If no duplicate is found within the allowed distance, return `false`.

---

## Time Complexity

**O(n)**

Each element is added and removed from the HashSet at most once.

---

## Space Complexity

**O(k)**

The HashSet stores at most `k` elements.

---

## Concepts Learned

- Sliding Window
- HashSet
- Window Size Maintenance
- Efficient Duplicate Detection

---

## Java Solution

See `Solution.java`.
