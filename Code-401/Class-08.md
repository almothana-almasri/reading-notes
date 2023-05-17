[Back to Home](../README.md)

## Stacks and Queues

In computer science, Stacks and Queues are dynamic sets that represent collections of elements and support various operations. 

A Stack is a data structure that follows the Last-In-First-Out (LIFO) principle, meaning the last element added is the first one to be removed. Key operations in a stack include `push` (adds an element to the stack), `pop` (removes the top element), `peek` or `top` (returns the top element without removing it), and `isEmpty` (checks if the stack is empty). Here's an example of how you might implement a simple stack in Python:

```python
class Stack:
    def __init__(self):
        self.stack = []

    def push(self, item):
        self.stack.append(item)

    def pop(self):
        if len(self.stack) < 1:
            return None
        return self.stack.pop()

    def peek(self):
        if self.stack:
            return self.stack[-1]
        return None

    def isEmpty(self):
        return len(self.stack) == 0
```

A Queue is another data structure that follows the First-In-First-Out (FIFO) principle, meaning the first element added is the first one to be removed. The primary operations in a queue are `enqueue` (adds an element to the end of the queue), `dequeue` (removes an element from the front), `peek` or `front` (returns the first element without removing it), and `isEmpty` (checks if the queue is empty). Here's how you might implement a simple queue in Python:

```python
class Queue:
    def __init__(self):
        self.queue = []

    def enqueue(self, item):
        self.queue.append(item)

    def dequeue(self):
        if len(self.queue) < 1:
            return None
        return self.queue.pop(0)

    def peek(self):
        if self.queue:
            return self.queue[0]
        return None

    def isEmpty(self):
        return len(self.queue) == 0
```

Both stacks and queues are fundamental data structures used in various types of algorithms and applications such as parsing, task scheduling, and more.