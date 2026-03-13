# Palindrome Checker - UC7 (Deque Optimized)

## Overview
This implementation uses a **Deque (Double-Ended Queue)** to optimize the palindrome checking process. Unlike UC6, which required two separate data structures, UC7 performs the check using a single structure by accessing both ends simultaneously.

## Logical Flow
1.  **Input Cleaning**: Special characters are removed and the string is lowercased.
2.  **Character Insertion**: All characters are added to the Deque in sequence.
3.  **Front-Rear Comparison**:
    * The first element (`removeFirst()`) and the last element (`removeLast()`) are removed and compared.
    * This continues until the Deque has 0 elements (even length string) or 1 element (odd length string).
    * If any pair fails to match, the string is not a palindrome.

## Key Concepts
* **Deque**: A linear collection that supports element insertion and removal at both endpoints.
* **Efficiency**: Reduces the memory overhead of maintaining two separate collections (Stack and Queue).
* **Time Complexity**: $O(n)$
* **Space Complexity**: $O(n)$

## Setup Instructions for IntelliJ
1. Create a new Java class named `PalindromeCheckerUC7`.
2. Copy and paste the code into the class.
3. Right-click the file and select **Run 'PalindromeCheckerUC7.main()'**.
4. Test with words like "radar", "level", or phrases like "A man, a plan, a canal: Panama".