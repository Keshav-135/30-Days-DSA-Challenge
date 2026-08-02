# Reverse Linked List (LeetCode 206)

## Difficulty

**Easy**

---

## Problem Statement

Given the head of a singly linked list, reverse the linked list and return the new head.

---

## Approach

Use **three pointers** to reverse the linked list in-place.

- `prev` points to the previous node.
- `curr` points to the current node.
- `next` temporarily stores the next node before changing the link.

Traverse the list while reversing each node's pointer until the end of the list is reached.

This approach reverses the linked list without using any extra data structure.

---

## Algorithm

1. Initialize:
   - `prev = null`
   - `curr = head`
2. Traverse the linked list until `curr` becomes `null`.
3. Store the next node in `next`.
4. Reverse the current node's pointer (`curr.next = prev`).
5. Move `prev` to `curr`.
6. Move `curr` to `next`.
7. Repeat until the end of the list.
8. Return `prev` as the new head of the reversed linked list.

---

## Time Complexity

**O(n)**

Each node is visited exactly once.

---

## Space Complexity

**O(1)**

The reversal is performed in-place using only three pointers.

---

## Key Concepts

- Linked List
- Pointer Manipulation
- In-place Reversal
- Iteration
- Three-Pointer Technique

---

## What I Learned

- Pointer manipulation is the foundation of Linked List problems.
- A linked list can be reversed without creating a new list.
- Using `prev`, `curr`, and `next` pointers makes the implementation simple and efficient.
- In-place algorithms help reduce extra space usage.

---

## Pattern

**Linked List**

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
