Exercise 10.1-4

Rewrite the `Enqueue` and `Dequeue` to detect underflow and overflow of a queue.

## Solution

```
Enqueue(Q,x)
  if Q.tail + 1 == Q.head or (Q.head = 1 and Q.tail = Q.length)
    error("overflow")
  else
    Q[Q.tail] = x
    if Q.tail == Q.length
      Q.tail = 1
    else Q.tail = Q.tail + 1
```

```
Dequeue(Q, x)
  if Q.head == Q.tail
    error("underflow")
  else
    x = Q[Q.head]
    if Q.head == Q.length
      Q.head = 1
    else Q.head = Q.head + 1
```
