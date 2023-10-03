# Exercise 10.1-1

Using Figure 10.1 as a model, illustrate the result of each operation in the sequence `Push(S,4)`, `Push(S,1)`, `Push(S,3)`, `Pop(S)`, `Push(S,8)`, and `Pop(S)` on an initially empty stack `S` stored in an array `S[1..6]`.

## Solution

| Operation | 1   | 2   | 3   | 4   | 5   | 6   |
| --------- | --- | --- | --- | --- | --- | --- |
| Push(S,4) | 4   |     |     |     |     |     |
| Push(S,1) | 4   | 1   |     |     |     |     |
| Push(S,3) | 4   | 1   | 3   |     |     |     |
| Pop(S)    | 4   | 1   |     |     |     |     |
| Push(S,8) | 4   | 1   | 8   |     |     |     |
| Pop(S)    | 4   | 1   |     |     |     |     |
