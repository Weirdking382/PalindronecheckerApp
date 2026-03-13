# UC5: Stack-Based Palindrome Checker

## Description
This module implements a palindrome validation logic using a **Stack** data structure. By leveraging the Last-In, First-Out (LIFO) property, we can easily compare a string against its reversed version.



## How it Works
1.  **Normalization**: The input string is cleaned of special characters and converted to lowercase.
2.  **Push Phase**: Each character of the string is pushed onto the stack.
3.  **Pop & Compare Phase**: As we iterate through the original string again, we `pop()` characters from the stack. Since the stack pops in reverse order, any mismatch indicates the string is not a palindrome.

## Key Concepts
* **Stack**: A linear data structure following LIFO.
* **Push**: Adding the character to the top.
* **Pop**: Removing the top character (the last one added).
* **Time Complexity**: $O(n)$ where $n$ is the length of the string.
* **Space Complexity**: $O(n)$ to store the characters in the stack.

## Setup Instructions for IntelliJ
1.  **Open IntelliJ IDEA** and your Palindrome project.
2.  **Create a new class**: Right-click `src` > `New` > `Java Class`.
3.  **Name the class**: `PalindromeStack`.
4.  **Paste the code**: Copy the provided Java code into the file.
5.  **Run**: Right-click inside the editor and select `Run 'PalindromeStack.main()'`.