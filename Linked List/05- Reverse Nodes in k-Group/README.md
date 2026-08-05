# Reverse Nodes in k-Group (LeetCode 25)

## Difficulty

**Hard**

---

## Problem Statement

Given the head of a linked list, reverse the nodes of the list **k at a time** and return the modified linked list.

If the number of remaining nodes is less than `k`, leave them as they are.

You must modify the links between nodes without changing their values.

---

## Approach

This problem is solved using a combination of a **Dummy Node** and **Pointer Manipulation**.

- Create a dummy node before the head to simplify edge cases.
- Find the kth node from the current group.
- If fewer than `k` nodes remain, stop the process.
- Reverse the current group of `k` nodes in-place.
- Connect the reversed group back to the remaining linked list.
- Repeat until all possible groups are reversed.

This approach performs the reversal without using any extra data structure.

---

## Algorithm

1. Create a dummy node pointing to the head.
2. Initialize a pointer to the start of the current group.
3. Find the kth node of the current group.
4. If the kth node does not exist, return the list.
5. Reverse the nodes in the current group.
6. Connect the reversed group with the previous and next groups.
7. Move to the next group and repeat.
8. Return `dummy.next`.

---

## Time Complexity

**O(n)**

Each node is visited only once.

---

## Space Complexity

**O(1)**

The linked list is modified in-place.

---

## What I Learned

- A Dummy Node helps simplify complex Linked List operations.
- Group-wise reversal requires careful pointer updates.
- In-place reversal avoids using extra memory.
- Combining multiple Linked List techniques leads to efficient solutions.
- Hard problems are often built by combining simpler concepts.
  
---

## Pattern

**Linked List**

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
