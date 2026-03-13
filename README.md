# Palindrome Checker - UC6 (Stack & Queue)

## Overview
This module implements a palindrome validation logic by utilizing the contrasting behaviors of **Stacks (LIFO)** and **Queues (FIFO)**.

## Logical Flow
1.  **Normalization**: The input string is stripped of special characters and converted to lowercase.
2.  **Storage**:
    * Each character is added to a `Queue` (maintaining original order).
    * Each character is added to a `Stack` (reversing the order).
3.  **Comparison**: The app iterates through both structures. Since `queue.poll()` returns the front and `stack.pop()` returns the back, a palindrome is confirmed if every pair matches.

## Key Concepts
* **Queue**: First-In-First-Out (FIFO) - Used for forward traversal.
* **Stack**: Last-In-First-Out (LIFO) - Used for backward traversal.
* **Time Complexity**: $O(n)$ where $n$ is the length of the string.
* **Space Complexity**: $O(n)$ to store characters in both data structures.

## How to Run in IntelliJ
1. Right-click `PalindromeCheckerUC6.java`.
2. Select **Run 'PalindromeCheckerUC6.main()'**.
3. Enter your text in the console terminal at the bottom.