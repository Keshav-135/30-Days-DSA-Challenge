# Remove Nth Node From End of List (LeetCode 19)

## Difficulty

**Medium**

---

## Problem Statement

Given the head of a linked list, remove the nth node from the end of the list and return the updated head.

---

## Approach

Use the **Fast & Slow Pointer** technique along with a **Dummy Node**.

- Create a dummy node before the head to handle edge cases.
- Move the `fast` pointer `n + 1` steps ahead.
- Move both `fast` and `slow` pointers together until `fast` reaches the end.
- The `slow` pointer will now be just before the node that needs to be removed.
- Update the links to skip the target node.

This approach removes the node in a single traversal.

---

## Algorithm

1. Create a dummy node and connect it to the head.
2. Initialize both `fast` and `slow` pointers at the dummy node.
3. Move the `fast` pointer `n + 1` steps ahead.
4. Move both pointers together until `fast` becomes `null`.
5. Remove the target node by updating `slow.next`.
6. Return `dummy.next`.

---

## Time Complexity

**O(n)**

The linked list is traversed only once.

---

## Space Complexity

**O(1)**

Only constant extra space is used.

---

## Key Concepts

- Linked List
- Fast & Slow Pointer
- Dummy Node
- Pointer Manipulation
- One Pass Algorithm

---

## What I Learned

- Fast & Slow Pointers help solve Linked List problems efficiently.
- A Dummy Node simplifies edge cases, especially when deleting the head node.
- The target node can be removed in a single traversal.
- Pointer manipulation is an essential Linked List interview skill.

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
