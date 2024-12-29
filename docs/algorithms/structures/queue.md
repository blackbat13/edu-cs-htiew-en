# Queue

A queue is a basic data structure that, like a stack, organizes elements in a linear fashion. A key feature of a queue is the FIFO (*First In, First Out*) principle, which means that the first element added to the queue is the first element to be removed from it. This behavior is analogous to an actual queue, for example in a store - the first person to join the queue is the first person to leave the queue.

The basic operations performed on a queue are:

- **Enqueue** (add to queue): adds an item to the end of the queue.
- **Dequeue** (remove from queue): removes an element from the beginning of the queue.

Additional operations that may be available in some queue implementations are:

- **Front/Peek**: returns the first element of the queue without deleting it.
- **IsEmpty**: checks if the queue is empty.
- **Size**: returns the number of elements in the queue.

## Applications

Queues are widely used in computer science, including:

- **Data synchronization**: queues are often used to synchronize data between processes. For example, they can be used to securely transfer requests from a producer thread to a consumer thread.
- **Data buffering**: queues can serve as buffers for data transferred between two CPU units or between a peripheral and the CPU.
- **CPU scheduling**: operating systems often use queues to manage processes that are waiting to access resources such as CPU, memory, disk, etc.
- **Graph algorithms**: queues are used in graph search algorithms such as breadth-first search (BFS).

By knowing the basics of queues, we can understand many key aspects of data management in computing, both in operating systems and in more complex algorithms.

## Implementation

Queues can be implemented using various data structures, including arrays and linked lists. The choice of data structure to implement a queue depends on specific requirements, such as efficiency of operations, memory consumption and ease of implementation.

Below you will find examples of queue implementations in selected programming languages.

### [:simple-cplusplus: C++](../../programming/c++/algorithms/structures/queue.md){ .md-button }

### [:simple-python: Python](../../programming/python/algorithms/structures/queue.md){ .md-button }

## Implementations - other

### [:simple-c:](../../programming/c/algorithms/structures/stack.md){ .md-button }