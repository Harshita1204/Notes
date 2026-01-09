Time complexity: It is the amount of time taken by an algorithm to run as a function of length of the input.

why we use time complexity? 
-> For making better programs.
-> comparison of algorithms.
-> To choose the best approach for large inputs

note*** we wont be judging the time complexity on the basis of machines that if the machine is slow or fast

# Units for time complexity:
1. Big-O Notation = upper bound
  -> Represents the upper bound
  -> Describes the worst-case time complexity
  -> Means: “algorithm will not take more than this time”
   
2. Theta θ Notation = for average case complexity
 -> Represents the tight bound
 -> Describes the exact growth rate
 -> Used when best, average, and worst case are same
   
3. omega notation Ω = lower bound
-> Represents the lower bound
-> Describes the best-case time complexity
-> Means: “algorithm will take at least this much time”

# Big-O notation (upper bound)
example: it take max to max this amount of time , not more than that.

-> constant time O(1)
-> linear time O(n)
-> logarithmetic time O(log n)
-> Quadratic time O(n^2)
-> cubic time O(n^3)

# Order of the time complexity
O(n!)        → Factorial   (High complexity)
O(2^n)       → Exponential
O(n^3)       → Cubic
O(n^2)       → Quadratic
O(n log n)   → Linearithmic
O(n)         → Linear
O(log n)     → Logarithmic
O(1)         → Constant   (low complexity)


