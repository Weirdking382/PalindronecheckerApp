# Palindrome Checker - UC9 (Recursion)

## Overview
This implementation uses **Recursion** to validate palindromes. Instead of using a loop or an external data structure, the function calls itself with a smaller version of the original problem until it reaches a base case.

## Logical Flow
1.  **Normalization**: The input is cleaned of non-alphanumeric characters.
2.  **Recursive Call**: The function `isPalindromeRecursive` is called with the full string indices (`0` and `length - 1`).
3.  **Character Comparison**:
    * Compare `str[start]` and `str[end]`.
    * If they match, call the function again for the range `(start + 1, end - 1)`.
4.  **Base Cases**:
    * **Success**: If `start >= end`, the entire string has been checked.
    * **Failure**: If `str[start] != str[end]`, the string is not a palindrome.

## Key Concepts
* **Recursion**: Solving a problem by breaking it down into smaller sub-problems of the same type.
* **Base Condition**: The essential "exit strategy" that prevents an infinite loop (StackOverflowError).
* **Call Stack**: The JVM uses its internal stack to keep track of each active recursive call.
* **Time Complexity**: $O(n)$ where $n$ is the length of the string.
* **Space Complexity**: $O(n)$ due to the recursion depth on the call stack.

## How to Run in IntelliJ
1. Create `PalindromeCheckerUC9.java` in your `src` folder.
2. Paste the code above.
3. Click the green **Run** arrow in the gutter next to the class name.
4. Input test cases like "Racecar" or "Hello".