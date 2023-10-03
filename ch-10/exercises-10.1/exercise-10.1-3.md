# Exercise 10.1-3

Using Figure 10.2 as a model, illustrate the result of each operation in the sequence `Enqueue(Q,4)`, `Enqueue(Q,1)`, `Enqueue(Q,3)`, `Dequeue(Q)`, `Enqueue(Q,8)` and `Dequeue(Q)` on an initially empty queue `Q` stored in array `Q[1..6]`.

## Solution

| Operation    | 1   | 2   | 3   | 4   | 5   | 6   | Q.head | Q.tail |
| ------------ | --- | --- | --- | --- | --- | --- | ------ | ------ |
| Enqueue(Q,4) | 4   |     |     |     |     |     | 1      | 2      |
| Enqueue(Q,1) | 4   | 1   |     |     |     |     | 1      | 3      |
| Enqueue(Q,3) | 4   | 1   | 3   |     |     |     | 1      | 4      |
| Dequeue(Q)   |     | 1   | 3   |     |     |     | 2      | 4      |
| Enqueue(Q,8) |     | 1   | 3   | 8   |     |     | 2      | 5      |
| Dequeue(Q)   |     |     | 3   | 8   |     |     | 3      | 5      |
