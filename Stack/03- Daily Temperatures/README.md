# Daily Temperatures (LeetCode 739)

## Difficulty

**Medium**

---

## Problem Statement

Given an array `temperatures` where `temperatures[i]` represents the temperature on the `iᵗʰ` day, return an array `answer` such that `answer[i]` is the number of days you have to wait after the `iᵗʰ` day to get a warmer temperature.

If there is no future day with a warmer temperature, return `0` for that day.

---

## Approach

Use a **Monotonic Decreasing Stack** to store the indices of temperatures.

- Traverse the array from left to right.
- Store indices in the stack while maintaining a decreasing order of temperatures.
- Whenever a warmer temperature is found, pop indices from the stack and calculate the number of waiting days.
- Push the current index onto the stack.
- Any indices remaining in the stack have no warmer future day, so their answer remains `0`.

This approach processes each element only once, making it highly efficient.

---

## Algorithm

1. Create an answer array initialized with `0`.
2. Create an empty stack to store indices.
3. Traverse the temperature array.
4. While the stack is not empty and the current temperature is greater than the temperature at the top index:
   - Pop the index.
   - Store the difference between the current index and the popped index in the answer array.
5. Push the current index onto the stack.
6. Return the answer array.

---

## Time Complexity

**O(n)**

Each index is pushed and popped at most once.

---

## Space Complexity

**O(n)**

The stack stores indices of unresolved temperatures.

---

## Key Concepts

- Stack
- Monotonic Stack
- Next Greater Element
- Array Traversal
- Index-Based Processing

---

## What I Learned

- A Monotonic Stack helps solve "next greater element" type problems efficiently.
- Storing indices instead of values makes it easy to calculate the number of waiting days.
- Every element is processed only once, reducing the brute-force solution from **O(n²)** to **O(n)**.
- Monotonic Stack is a powerful interview pattern used in many advanced DSA problems.

---

## Pattern

**Stack (Monotonic Stack)**

---

## Difficulty

**Medium**

---

## Status

**Solved** ✅

---

## Language

**Java**

---

## Java Solution

See `Solution.java`.
