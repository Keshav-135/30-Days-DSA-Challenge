# Two Sum (LeetCode 1)

## Difficulty
**Easy**

## Pattern
**Hashing**

---

## Problem Statement

Given an integer array `nums` and an integer `target`, return the indices of the two numbers such that they add up to the target.

You may assume that each input has exactly one solution, and you may not use the same element twice.

You can return the answer in any order.

---

## Approach

Instead of checking every possible pair, use a **HashMap** to store each number along with its index while traversing the array.

For every element:

1. Calculate the required complement:
   ```
   need = target - nums[i]
   ```

2. Check if the complement already exists in the HashMap.
   - If it exists, return the stored index and the current index.
   - Otherwise, store the current element and its index in the HashMap.

This allows us to find the answer in a single traversal.

---

## Algorithm

- Create an empty `HashMap<Integer, Integer>`.
- Traverse the array from left to right.
- Calculate the required complement.
- If the complement exists in the HashMap:
  - Return both indices.
- Otherwise:
  - Store the current number and its index.
- If no solution exists, return an empty array.

---

## Time Complexity

**O(n)**

Each element is processed only once, and HashMap operations take **O(1)** on average.

---

## Space Complexity

**O(n)**

The HashMap stores at most one entry for each element.

---

## Key Concepts

- HashMap
- One-Pass Hashing
- Complement Technique
- Array Traversal
- Constant Time Lookup

---

## What I Learned

- HashMap can significantly reduce the time complexity of searching problems.
- Instead of comparing every pair, storing previously seen elements allows finding the answer in a single pass.
- The complement technique is widely used in many interview questions involving arrays and hashing.
- Choosing the right data structure can improve a brute-force solution from **O(n²)** to **O(n)**.

---


## Pattern

**Hashing**

---

## Difficulty

**Easy**

---

## Status

**Solved** ✅

---

## Language

**Java**

---

## Java Solution

See `Solution.java`.
