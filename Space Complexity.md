# What is Space Complexity?
Space Complexity is the amount of extra memory used by an algorithm as a function of input size n.
It tells us how much additional space an algorithm needs to execute.

Why Do We Use Space Complexity?
-> To write memory-efficient programs
-> To avoid memory overflow
-> To compare algorithms based on memory usage
-> Important when memory is limited (embedded systems, large data)

Important Note************

We do NOT judge space complexity based on machine RAM size.
-> RAM size 
-> Computer type 
-> Programming language 
-> Space complexity depends on algorithm design only

What is Counted in Space Complexity?
Space complexity includes:
Variables
Arrays
Data structures
Recursion stack
Function call stack

Common Space Complexities:
O(1) — Constant Space
-> Uses a fixed amount of extra memory
-> Does NOT depend on input size
for example: int sum = 0;

O(n) — Linear Space
-> Extra memory grows with input size
for example: int temp[n];
Recursion with depth n

O(n²) — Quadratic Space
Uses a 2D structure
int matrix[n][n];

O(log n) — Logarithmic Space
Recursion depth reduces by half

Example:
Binary Search (recursive)

Important Concept********: Auxiliary Space

Auxiliary Space is the extra space used excluding input space.
Example:
Input array → not counted
Extra variables / arrays → counted

Time vs Space Trade-off
Sometimes we:
Use more space to reduce time
Use less space but increase time
Example:
Recursion → slower & more space
Iteration → faster & less space
