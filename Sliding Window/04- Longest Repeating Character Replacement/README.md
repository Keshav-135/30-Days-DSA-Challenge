# Longest Repeating Character Replacement (LeetCode 424)

## Difficulty
**Medium**

## Pattern
**Sliding Window (Variable Size)**

---

## Problem Statement

Given a string `s` and an integer `k`, return the length of the longest substring that can be obtained by replacing at most `k` characters so that all characters in the substring are the same.

---

## Approach

1. Use a frequency array to count the occurrence of each character inside the current window.
2. Maintain two pointers (`left` and `right`) to represent the sliding window.
3. Track the frequency of the most common character (`maxFreq`) in the current window.
4. Expand the window by moving the `right` pointer.
5. If the number of characters that need to be replaced (`window size - maxFreq`) becomes greater than `k`, shrink the window from the left.
6. Update the maximum window length whenever the window is valid.
7. Return the maximum length found.

---

## Time Complexity

**O(n)**

Each character is processed at most twice while expanding and shrinking the sliding window.

---

## Space Complexity

**O(1)**

A fixed-size frequency array of 26 uppercase English letters is used.

---

## Key Concepts

- Sliding Window (Variable Size)
- Frequency Array
- Two Pointers
- Window Validation
- Greedy Optimization

---

## What I Learned

- How to apply the Variable Size Sliding Window pattern.
- How to use a frequency array for efficient character counting.
- How the condition `(window size - maxFreq) <= k` determines whether the current window is valid.
- How to optimize substring problems from brute-force solutions to linear time complexity.

---

## Java Solution

See `Solution.java`.
