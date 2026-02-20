# DATA STRUCTURES AND ALGORITHMS  
# UNIT 1 – INTRODUCTION 

---

# 1. INTRODUCTION TO DATA STRUCTURES

## 1.1 What is Data?

Data refers to raw facts and figures that can be processed to generate meaningful information.

Examples:
- Student roll numbers
- Bank account balances
- Marks list
- Employee salary records
- Website user data

When the size of data increases, managing it efficiently becomes challenging. This is where Data Structures are required.

---

## 1.2 What is a Data Structure?

A Data Structure is a specific way of organizing, storing, and managing data in memory so that it can be accessed and modified efficiently.

In simple words:

Data Structure = Organized way of storing data in memory for efficient use.

---

## 1.3 Classification of Data Structures

Data structures are mainly classified into:

### 1. Linear Data Structures
Elements are arranged sequentially.

Examples:
- Array
- Linked List
- Stack
- Queue

### 2. Non-Linear Data Structures
Elements are arranged hierarchically.

Examples:
- Trees
- Graphs

---

## 1.4 Why Do We Need Data Structures?

### 1. Efficient Searching

If we store 1 million records randomly, searching will be slow.

Example:
- Linear Search → O(n)
- Binary Search → O(log n)

Binary Search is much faster for large datasets.

---

### 2. Efficient Insertion and Deletion

In Array:
- Insertion in middle → O(n)

In Linked List:
- Insertion at beginning → O(1)

Choosing the correct data structure improves performance.

---

### 3. Better Memory Utilization

Some data structures allocate memory dynamically (Linked List), reducing wastage.

---

### 4. Real-Life Applications

Data structures are used in:
- Operating Systems
- Databases
- Web Browsers
- Compilers
- Artificial Intelligence
- Networking

---

# 2. INTRODUCTION TO ALGORITHMS

## 2.1 What is an Algorithm?

An Algorithm is a step-by-step procedure to solve a problem in a finite amount of time.

---

## 2.2 Characteristics of an Algorithm

1. Input – Takes zero or more inputs.
2. Output – Produces at least one output.
3. Definiteness – Clear and unambiguous steps.
4. Finiteness – Must terminate.
5. Effectiveness – Each step must be simple and executable.

---

## 2.3 Why Do We Need Algorithms?

- To solve problems systematically
- To compare multiple approaches
- To choose the most efficient solution
- To optimize performance

---

# 3. TIME COMPLEXITY

## 3.1 Definition

Time Complexity measures how the running time of an algorithm increases as input size increases.

We do not measure time in seconds.  
We count the number of operations.

---

## 3.2 Example Analysis

### Example 1: Single Loop

If a loop runs n times:

Time Complexity = O(n)

---

### Example 2: Nested Loop

If two nested loops each run n times:

Time Complexity = O(n²)

---

## 3.3 Rules for Calculating Time Complexity

1. Ignore constant values  
   5n → O(n)

2. Ignore lower order terms  
   n² + 3n + 2 → O(n²)

3. Focus on worst case unless specified.

---

## 3.4 Types of Time Complexity

### Best Case
Minimum time taken by algorithm.

### Average Case
Expected time taken.

### Worst Case
Maximum time taken.

Example: Linear Search

Best Case → O(1)  
Worst Case → O(n)  
Average Case → O(n)

---

# 4. SPACE COMPLEXITY

## 4.1 Definition

Space Complexity measures the total memory used by an algorithm.

It includes:
- Input space
- Auxiliary space

---

## 4.2 Example

### Iterative Approach
Uses fixed number of variables  
Space Complexity = O(1)

### Recursive Approach
Uses function call stack  
Space Complexity = O(n)

---

# 5. ASYMPTOTIC NOTATIONS

Asymptotic notations describe the growth rate of an algorithm as input size becomes very large.

---

## 5.1 Big-O Notation (O)

Represents Upper Bound (Worst Case).

If f(n) grows slower or equal to g(n), then:

f(n) = O(g(n))

Example:
3n² + 4n + 5 → O(n²)

---

## 5.2 Big Omega (Ω)

Represents Lower Bound (Best Case).

If f(n) grows at least as fast as g(n):

f(n) = Ω(g(n))

---

## 5.3 Big Theta (Θ)

Represents Tight Bound.

If f(n) is bounded above and below by g(n):

f(n) = Θ(g(n))

---

# 6. AVERAGE AND WORST CASE ANALYSIS

Example: Linear Search

Worst Case:
Element at last position  
Time Complexity = O(n)

Average Case:
Element somewhere in middle  
Approximately n/2 comparisons  
Still O(n)

---

# 7. ARRAYS

## 7.1 Definition

An Array is a collection of elements stored in contiguous memory locations.

Each element is accessed using index.

---

## 7.2 Advantages

- Direct access → O(1)
- Simple implementation
- Better cache performance

---

## 7.3 Disadvantages

- Fixed size
- Insertion and deletion costly
- Possible memory wastage

---

## 7.4 Operations on Arrays

Traversal → O(n)  
Insertion at end → O(1)  
Insertion at middle → O(n)  
Deletion → O(n)  
Searching:
- Linear → O(n)
- Binary → O(log n)

---

# 8. LINKED LIST

## 8.1 Definition

A Linked List is a collection of nodes where each node contains:
- Data
- Pointer to next node

Memory is not contiguous.

---

## 8.2 Advantages

- Dynamic size
- Easy insertion and deletion
- No memory wastage due to pre-allocation

---

## 8.3 Disadvantages

- No direct access
- Extra memory for pointer
- Slower traversal compared to arrays

---

## 8.4 Operations on Linked List

Traversal → O(n)  
Insertion at head → O(1)  
Insertion at tail → O(n)  
Deletion (if pointer given) → O(1)  
Searching → O(n)

---

# 9. ARRAY VS LINKED LIST (DETAILED COMPARISON)

| Feature | Array | Linked List |
|----------|--------|-------------|
| Memory | Contiguous | Non-contiguous |
| Access | O(1) | O(n) |
| Size | Fixed | Dynamic |
| Insertion | Costly | Easy |
| Deletion | Costly | Easy |
| Extra Memory | No | Yes (pointer) |

