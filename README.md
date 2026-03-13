# Palindrome Checker - UC13 (Performance Benchmarking)

## Overview
UC13 focuses on quantitative analysis. While all algorithms achieve the same result ($O(n)$ time complexity), the **constant factors** (memory allocation, object creation, and method overhead) vary significantly between approaches.

## Key Concepts
* **System.nanoTime()**: Provides the most precise time available from the system timer (1 nanosecond = $10^{-9}$ seconds).
* **Overhead**: Comparing how manual array manipulation (Two-Pointer) is faster than using high-level objects like `Stack` or `LinkedList`.
* **Benchmarking**: The process of running a computer program to assess the relative performance of an object.

## Expected Findings
1.  **Two-Pointer**: Usually the fastest because it avoids object creation and operates directly on the primitive `char` array.
2.  **Deque**: Often faster than the Stack/Queue approach because `ArrayDeque` is more efficient than `LinkedList`.
3.  **Stack/Queue**: Usually the slowest due to the creation of two separate collections and double the insertions.

## How to Setup in IntelliJ
1. Create `PalindromePerformanceUC13.java` in your `src` folder.
2. Run the file.
3. For best results, use a very long string (copy/paste a paragraph) to see the performance gap clearly.