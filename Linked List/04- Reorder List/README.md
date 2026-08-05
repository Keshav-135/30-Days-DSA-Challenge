# Reorder List (LeetCode 143)

## Difficulty

**Medium**

---

## Problem Statement

Given the head of a singly linked list, reorder the list in-place as:

L₀ → L₁ → L₂ → ... → Lₙ

becomes

L₀ → Lₙ → L₁ → Lₙ₋₁ → L₂ → Lₙ₋₂ → ...

Return the reordered linked list without modifying the values of the nodes.

---

## Approach

This problem can be solved in three steps:

1. Find the middle of the linked list using the **Fast & Slow Pointer** technique.
2. Reverse the second half of the linked list.
3. Merge the first half and the reversed second half alternately.

This approach reorders the list in-place without using any extra data structure.

---

## Algorithm

1. Find the middle of the linked list using Fast & Slow pointers.
2. Split the linked list into two halves.
3. Reverse the second half.
4. Merge both halves alternately.
5. Return the reordered linked list.

---

## Time Complexity

**O(n)**

Each node is visited a constant number of times.

---

## Space Complexity

**O(1)**

The list is reordered in-place without using extra space.

---

## Key Concepts

- Linked List
- Fast & Slow Pointer
- Reverse Linked List
- Merge Linked Lists
- Pointer Manipulation

---

## What I Learned

- Multiple Linked List techniques can be combined to solve complex problems.
- Fast & Slow Pointers efficiently find the middle node.
- Reversing a linked list is an important reusable technique.
- Merging two linked lists can be done without creating new nodes.
- In-place algorithms help achieve optimal space complexity.
  
---

## Pattern

**Linked List**

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
