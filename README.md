# Palindrome Checker - UC8 (Singly Linked List)

## Overview
This use case demonstrates a deep dive into manual memory management and pointer manipulation. By using a **Singly Linked List**, we validate a palindrome with optimal space complexity.

## Key Techniques
* **Fast and Slow Pointers**: A technique where one pointer moves twice as fast as the other to find the middle of the list in one pass.
* **In-Place Reversal**: Reversing the second half of the linked list without creating a new list, keeping space complexity at $O(1)$ (excluding the initial list creation).

## Logical Flow
1.  **Normalization**: Strip non-alphanumeric characters.
2.  **List Creation**: Convert the string into a custom `Node` based structure.
3.  **Find Midpoint**: Use `slow` and `fast` pointers to locate the center.
4.  **Reverse**: Flip the `next` pointers of the second half.
5.  **Validation**: Compare the data values of the first half and the reversed second half.

## Data Structure Details
* **Structure**: Singly Linked List (Data + Next Reference).
* **Time Complexity**: $O(n)$ - one pass for creation, one for middle finding, one for reversal, and one for comparison.
* **Space Complexity**: $O(1)$ additional space beyond the initial list storage.

## How to Run in IntelliJ
1. Create a new class `PalindromeCheckerUC8.java`.
2. Paste the provided source code.
3. Click the green **Play** button next to the `main` method.