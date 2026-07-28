# Remove All Adjacent Duplicates In String (LeetCode 1047)

## Difficulty

**Easy**

---

## Problem Statement

Given a string `s`, repeatedly remove adjacent duplicate characters until no adjacent duplicates remain.

Return the final string after all possible removals.

---

## Approach

Use a **Stack** to efficiently process the characters.

- Traverse the string one character at a time.
- If the current character matches the top of the stack, remove the top element using `pop()`.
- Otherwise, push the current character onto the stack.
- After processing all characters, build the final string from the remaining characters in the stack.

This approach removes adjacent duplicates in a single traversal without repeatedly scanning the string.

---

## Algorithm

1. Create an empty stack.
2. Traverse each character of the string.
3. If the stack is not empty and the current character equals the top element:
   - Pop the top element.
4. Otherwise:
   - Push the current character onto the stack.
5. After traversal, pop all remaining characters into a `StringBuilder`.
6. Reverse the `StringBuilder` and return the final string.

---

## Time Complexity

**O(n)**

Each character is pushed and popped at most once.

---

## Space Complexity

**O(n)**

The stack stores the characters during processing.

---

## Key Concepts

- Stack
- LIFO (Last In, First Out)
- Push
- Pop
- String Traversal
- StringBuilder

---

## What I Learned

- Stack is an efficient data structure for handling adjacent duplicate removal.
- Every character is processed only once, making the solution linear.
- Using `StringBuilder` helps construct the final answer efficiently.
- The LIFO property naturally solves problems involving recently processed elements.

---

## Pattern

**Stack**

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
