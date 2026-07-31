# Largest Rectangle in Histogram (LeetCode 84)

## Difficulty

**Hard**

---

## Problem Statement

Given an array `heights` representing the heights of bars in a histogram, return the area of the largest rectangle that can be formed.

---

## Approach

Use a **Monotonic Increasing Stack** to efficiently calculate the largest rectangle.

- Store the indices of histogram bars in increasing order of height.
- Traverse the histogram from left to right.
- Whenever the current bar is smaller than the bar at the top of the stack:
  - Pop the top index.
  - Treat the popped bar as the height of the rectangle.
  - Calculate the width using the current index and the new top of the stack.
  - Update the maximum rectangle area.
- Continue until all bars are processed.
- Perform one extra iteration to process any remaining bars in the stack.

This approach ensures every bar is processed only once.

---

## Algorithm

1. Create an empty stack to store indices.
2. Initialize `maxArea` as `0`.
3. Traverse the histogram from index `0` to `n` (inclusive).
4. While the stack is not empty and the current bar is smaller than the top bar:
   - Pop the top index.
   - Calculate the rectangle height.
   - Calculate the rectangle width.
   - Update the maximum area.
5. Push the current index into the stack.
6. Return the maximum rectangle area.

---

## Time Complexity

**O(n)**

Each index is pushed and popped at most once.

---

## Space Complexity

**O(n)**

The stack stores indices of histogram bars.

---

## Key Concepts

- Stack
- Monotonic Increasing Stack
- Previous Smaller Element (PSE)
- Next Smaller Element (NSE)
- Histogram
- Area Calculation

---

## What I Learned

- A Monotonic Increasing Stack helps solve histogram problems efficiently.
- Previous Smaller and Next Smaller boundaries can be determined implicitly using a stack.
- Every histogram bar is processed only once, reducing the brute-force solution from **O(n²)** to **O(n)**.
- Stack is useful for solving advanced interval and range problems.

---

## Pattern

**Stack (Monotonic Stack)**

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
