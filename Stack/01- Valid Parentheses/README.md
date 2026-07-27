# Valid Parentheses (LeetCode 20)

## Difficulty

**Easy**

---

## Problem Statement

Given a string `s` containing only the characters `'('`, `')'`, `'{'`, `'}'`, `'['`, and `']'`, determine whether the input string is valid.

A string is considered valid if:

- Every opening bracket has a corresponding closing bracket.
- Brackets are closed in the correct order.
- Every closing bracket matches the most recent unmatched opening bracket.

---

## Approach

Use a **Stack** to keep track of opening brackets.

- Traverse the string character by character.
- Push every opening bracket onto the stack.
- When a closing bracket is encountered:
  - Check if the stack is empty.
  - Pop the top element.
  - Verify that it matches the corresponding opening bracket.
- After processing the entire string, the stack should be empty for the string to be valid.

---

## Algorithm

- Create an empty stack.
- Traverse every character in the string.
- If the character is an opening bracket:
  - Push it onto the stack.
- Otherwise:
  - If the stack is empty, return `false`.
  - Pop the top element.
  - Check whether the popped bracket matches the current closing bracket.
  - If it does not match, return `false`.
- Return `true` if the stack is empty; otherwise return `false`.

---

## Time Complexity

**O(n)**

Each character is processed only once.

---

## Space Complexity

**O(n)**

In the worst case, all opening brackets are stored in the stack.

---

## Key Concepts

- Stack
- LIFO (Last In, First Out)
- Push
- Pop
- Bracket Matching
- String Traversal

---

## What I Learned

- Stack is the ideal data structure for matching pairs of brackets.
- The Last In, First Out (LIFO) property naturally handles nested structures.
- Checking for an empty stack before popping helps avoid runtime errors.
- This problem builds a strong foundation for more advanced Stack-based interview questions.

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
