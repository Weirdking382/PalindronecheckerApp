# Palindrome Checker - UC10 (Normalization)

## Overview
UC10 focuses on **Data Preprocessing**. In real-world scenarios, "Race Car" should be considered a palindrome, even though it contains a space and a capital 'C'. This module ensures the logic is "fuzzy" enough to handle human input while remaining technically accurate.

## Key Concepts
* **Normalization**: Transforming data into a standard format (e.g., all lowercase).
* **Regular Expressions (Regex)**: Using patterns like `[^a-z0-9]` to filter out unwanted characters (whitespace, punctuation, symbols).
* **Immutability**: Understanding that `String` methods like `toLowerCase()` return a *new* string rather than modifying the original.

## Logical Flow
1.  **Lowercasing**: Convert the entire input to lowercase to eliminate case sensitivity.
2.  **Filtering**: Use `replaceAll` with a regex pattern to strip out everything except letters and numbers.
3.  **Validation**: Use a simple two-pointer approach to compare the "cleaned" string.

## How to Test in IntelliJ
1. Create `PalindromeCheckerUC10.java`.
2. Run the application.
3. Try these "Tricky" inputs:
    * `Step on no pets`
    * `No 'x' in Nixon`
    * `Was it a car or a cat I saw?`
    * `12321`