# DATA STRUCTURES AND ALGORITHMS  
# UNIT 2 – STACKS AND QUEUES 

---

# 1. STACK

---

## 1.1 Definition of Stack

A Stack is a linear data structure that follows the principle:

LIFO – Last In First Out

This means the element inserted last will be removed first.

Real Life Example:
- Stack of plates
- Undo/Redo feature
- Browser back button

---

## 1.2 Basic Terminology

- Top → Points to the topmost element of stack
- Push → Insert element into stack
- Pop → Remove element from stack
- Peek/Top → View top element without removing
- Overflow → When stack is full
- Underflow → When stack is empty and pop is attempted

---

## 1.3 Basic Operations on Stack

### 1. Push Operation

Insert an element at the top.

Steps:
1. Check if stack is full.
2. Increment top.
3. Insert element.

Time Complexity → O(1)

---

### 2. Pop Operation

Remove the top element.

Steps:
1. Check if stack is empty.
2. Return top element.
3. Decrement top.

Time Complexity → O(1)

---

### 3. Peek Operation

Returns the top element without removing it.

Time Complexity → O(1)

---

## 1.4 Implementation of Stack

### 1. Using Array

- Fixed size
- Uses index as top pointer
- Simple implementation

Disadvantage:
- Size limitation

---

### 2. Using Linked List

- Dynamic size
- Top points to head node
- No overflow until memory is full

---

## 1.5 Applications of Stack

---

### 1. Parenthesis Checker

Used to check whether an expression has balanced parentheses.

Example:
{[()]}

Algorithm:
1. Create empty stack.
2. Traverse expression.
3. If opening bracket → push.
4. If closing bracket:
   - If stack empty → unbalanced.
   - Else check top.
   - If matches → pop.
5. If stack empty at end → balanced.

Time Complexity → O(n)

---

### 2. Infix to Postfix Conversion

Types of Expressions:

- Infix → A + B
- Prefix → +AB
- Postfix → AB+

Computers prefer postfix because:
- No need for precedence rules.
- Easy evaluation.

Algorithm for Infix to Postfix:

1. If operand → add to output.
2. If '(' → push to stack.
3. If ')' → pop until '('.
4. If operator:
   - Pop operators with higher or equal precedence.
   - Push current operator.

Time Complexity → O(n)

---

### 3. Evaluation of Postfix Expression

Example:
23*54*+9-

Steps:
1. Scan left to right.
2. If operand → push.
3. If operator:
   - Pop two operands.
   - Apply operator.
   - Push result.

Time Complexity → O(n)

---

### 4. Role of Stack in Recursion

Recursion uses system stack.

Each recursive call:
- Creates activation record (stack frame).
- Stores local variables.
- Stores parameters.
- Stores return address.

When function returns:
- Stack frame is removed.

Example:
Factorial using recursion.

Space Complexity → O(n)

---

### 5. Tower of Hanoi

Problem:
Move n disks from source to destination using auxiliary rod.

Rules:
1. Move one disk at a time.
2. Larger disk cannot be placed on smaller disk.
3. Use auxiliary rod.

Recurrence Relation:
T(n) = 2T(n-1) + 1

Time Complexity → O(2^n)

Space Complexity → O(n)

---

### 6. Quick Sort and Stack

Quick Sort uses recursion.

Recursion internally uses stack.

Average Case → O(log n) space  
Worst Case → O(n) space

---

# 2. QUEUE

---

## 2.1 Definition of Queue

A Queue is a linear data structure that follows:

FIFO – First In First Out

Example:
- Queue at ticket counter
- Printer queue
- Call center

---

## 2.2 Basic Terminology

- Front → Points to first element
- Rear → Points to last element
- Enqueue → Insert element at rear
- Dequeue → Remove element from front
- Overflow → Queue full
- Underflow → Queue empty

---

## 2.3 Operations on Queue

### 1. Enqueue

Insert element at rear.

Steps:
1. Check if queue is full.
2. Increment rear.
3. Insert element.

Time Complexity → O(1)

---

### 2. Dequeue

Remove element from front.

Steps:
1. Check if queue is empty.
2. Return front element.
3. Increment front.

Time Complexity → O(1)

---

### 3. Peek

Return front element.

Time Complexity → O(1)

---

## 2.4 Implementation of Queue

### 1. Using Array

- Simple implementation
- Wastes space after deletions

---

### 2. Circular Queue

Solves space wastage problem.

Uses circular indexing:
rear = (rear + 1) % size

Efficient memory usage.

---

### 3. Using Linked List

- Dynamic size
- No overflow unless memory full

---

## 2.5 Priority Queue

In a Priority Queue:
- Each element has a priority.
- Element with highest priority removed first.
- If priorities equal → follow FIFO.

Implementation:
- Binary Heap (most efficient)
- Array

Applications:
- CPU Scheduling
- Dijkstra’s Algorithm
- Event-driven simulation
- Operating systems

---

## 2.6 Applications of Queue

1. CPU Scheduling
2. Breadth First Search (BFS)
3. Printer Queue
4. Network packet processing
5. Web server request handling
6. Task scheduling systems

---

# 3. STACK VS QUEUE (COMPARISON)

| Feature | Stack | Queue |
|----------|--------|--------|
| Principle | LIFO | FIFO |
| Insertion | Push | Enqueue |
| Deletion | Pop | Dequeue |
| Access | Top | Front |
| Used in | Recursion, Expression Evaluation | Scheduling, BFS |

