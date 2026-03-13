# Palindrome Checker - UC12 (Strategy Pattern)

## Overview
UC12 implements the **Strategy Design Pattern**, allowing the application to switch between different data structure implementations (Stack vs. Deque) at runtime without changing the core application logic.

## Key Concepts
* **Interface**: Defines a common contract (`isValid`) that all algorithms must follow.
* **Polymorphism**: The `PalindromeContext` treats all strategies as the same type, even though they behave differently internally.
* **Loose Coupling**: The main application doesn't need to know *how* the check happens; it just knows it *can* happen.

## Pattern Structure
1.  **Strategy Interface**: The "Contract."
2.  **Concrete Strategies**: The specific algorithms (Stack-based, Deque-based, etc.).
3.  **Context**: The class that uses the strategy and allows it to be swapped via `setStrategy()`.

## How to Run in IntelliJ
1.  Create the four files: `PalindromeStrategy`, `StackStrategy`, `DequeStrategy`, and `PalindromeContext`.
2.  Ensure they are in the same package.
3.  Run `PalindromeContext`.
4.  Observe how you can choose your algorithm via the console menu.