# Uncommon JavaScript Bug: Stack Overflow in Recursive Function

This repository demonstrates a subtle stack overflow error in a seemingly simple recursive JavaScript function. The error arises from the function's failure to correctly define a base case, leading to infinite recursion.

## Bug Description

The `foo` function is intended to recursively process inputs `a` and `b`.  However, the logic within the function does not guarantee a termination condition under all circumstances, resulting in a stack overflow.

## How to Reproduce

1. Clone this repository.
2. Open `bug.js`.
3. Run the code using a JavaScript environment (e.g., Node.js).
4. Observe the stack overflow error.

## Solution

The solution involves carefully reviewing the function's logic and ensuring it always has a defined base case that terminates the recursion. The `bugSolution.js` file provides a corrected version.

## Lessons Learned

This example highlights the importance of:

* **Careful base case definition in recursive functions.**
* **Thorough testing to cover various input scenarios.**
* **Understanding potential pitfalls of recursion, such as stack overflow errors.**