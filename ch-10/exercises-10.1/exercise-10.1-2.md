# Exercise 10.1-2

Explain how to implement two stacks in one array `A[1..n]` such that neither stack overflows unless the total number of elements in both stacks together is `n`. The `Push` and `Pop` operations should run in `O(1)` time.

## Solution

For implementing two stacks in a single array, we can start one stack at the beginning of the array and another stack at the end of the array. For the first stack, we increase the top pointer for push and decrease it for pop operations. For the second stack, we decrease the top pointer for push and increase it for pop operations.

If the top of the first array is one index less than the top of the second array, the stack is full, and we can prevent overflow.

The complete solution is implement in [DualStack](https://raw.githubusercontent.com/iusmaharjan/dsa-python/main/datastructures/dual_stack.py).

