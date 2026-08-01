# Merge Two Sorted Lists (LeetCode 21)

## Difficulty

**Easy**

---

## Problem Statement

You are given the heads of two sorted linked lists.

Merge the two lists into one sorted linked list and return its head.

---

## Approach

Use a **Dummy Node** to simplify the merging process.

- Create a dummy node and use a pointer to build the merged list.
- Compare the current nodes of both linked lists.
- Append the smaller node to the merged list.
- Move the corresponding pointer forward.
- Once one list is exhausted, attach the remaining nodes of the other list.

---

## Algorithm

1. Create a dummy node.
2. Create a pointer pointing to the dummy node.
3. Compare nodes from both lists.
4. Add the smaller node to the merged list.
5. Move the corresponding pointer.
6. Attach the remaining nodes after one list ends.
7. Return `dummy.next`.

---

## Time Complexity

**O(n + m)**

Where:

- n = length of first list
- m = length of second list

---

## Space Complexity

**O(1)**

No extra space is used.

---

## Key Concepts

- Linked List
- Dummy Node
- Pointer Manipulation
- Iteration
- Merging Sorted Lists

---

## What I Learned

- Dummy nodes simplify Linked List problems.
- Pointer manipulation is the key to solving Linked List questions.
- Linked Lists can be merged efficiently without creating new nodes.
- Iterative solutions often provide better space efficiency.

---

## Interview Takeaways

This is one of the most frequently asked Linked List interview questions.

It helps build a strong understanding of:

- Linked List Traversal
- Pointer Manipulation
- Dummy Node Technique
- Efficient Merging

Mastering this problem makes it easier to solve advanced Linked List questions like Merge K Sorted Lists, Reverse Linked List, and Sort List.

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
