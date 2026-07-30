# Min Stack (LeetCode 155)

## Difficulty

**Medium**

---

## Problem Statement

Design a stack that supports the following operations in constant time:

- `push(int val)`
- `pop()`
- `top()`
- `getMin()`

Implement the `MinStack` class so that every operation runs in **O(1)** time.

---

## Approach

Use **two stacks** to achieve constant-time operations.

- The first stack stores all the elements.
- The second stack keeps track of the minimum element at every stage.
- While pushing, insert the value into the minimum stack if it is smaller than or equal to the current minimum.
- While popping, remove the top element from the minimum stack if it matches the element being removed from the main stack.
- The top of the minimum stack always represents the minimum element.

This approach avoids traversing the stack to find the minimum element.

---

## Algorithm

1. Create two stacks:
   - Main Stack
   - Minimum Stack
2. Push every element into the main stack.
3. If the minimum stack is empty or the current element is smaller than or equal to its top element, push it into the minimum stack.
4. During `pop()`, if the top of both stacks is the same, pop from both stacks.
5. `top()` returns the top element of the main stack.
6. `getMin()` returns the top element of the minimum stack.

---

## Time Complexity

- **push()** → O(1)
- **pop()** → O(1)
- **top()** → O(1)
- **getMin()** → O(1)

---

## Space Complexity

**O(n)**

An additional stack is used to store minimum elements.

---

## Key Concepts

- Stack
- Auxiliary Stack
- Data Structure Design
- Constant Time Operations
- Minimum Element Tracking

---

## What I Learned

- A single stack cannot efficiently return the minimum element in O(1) after multiple operations.
- Using an auxiliary stack makes it possible to maintain the current minimum at every step.
- Multiple data structures can work together to optimize performance.
- Designing efficient data structures is an important interview skill.

---

## Pattern

**Stack**

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
