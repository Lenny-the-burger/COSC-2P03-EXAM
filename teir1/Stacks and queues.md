-   Chapter 3 covers the topics of stacks and queues.
-   Understand the usage and implementation of stacks and queues.
-   Be familiar with the concept of a double-ended queue (deque).
-   Know how to implement a priority queue, including different representations.

```
  stack:
  -----
  | 5 |
  -----
  | 4 |
  -----
  | 3 |
  -----
  | 2 |
  -----
  | 1 |
  -----

  queue:
  -----
  | 1 |
  -----
  | 2 |
  -----
  | 3 |
  -----
  | 4 |
  -----
  | 5 |
  -----
```

Stacks and queues are data structures that store and retrieve items in a particular order. Stacks use the last-in, first-out (LIFO) order, while queues use the first-in, first-out (FIFO) order. These data structures are useful for a variety of applications, such as evaluating arithmetic expressions, implementing undo/redo functions, and simulating real-world scenarios such as call center queues.

## Usage

Stacks and queues have different uses depending on the order in which items are stored and retrieved. Stacks are typically used when the most recently added item is the one that should be accessed first, such as in a undo/redo function or in a depth-first search algorithm. Queues are typically used when the oldest item is the one that should be accessed first, such as in a call center queue or in a breadth-first search algorithm.

## Deques

A deque, also known as a double-ended queue, is a data structure that allows items to be added or removed from either end. This makes deques more flexible than stacks and queues, which only allow items to be added or removed from one end. Deques are useful in situations where it's necessary to have the ability to add or remove items from either end, such as in a round-robin scheduling algorithm.

## Priority Queues

A priority queue is a data structure that allows items to be added with a priority value, and retrieves items in order of their priority. This makes priority queues useful in situations where certain items should be processed before others, such as in a scheduling algorithm or in a pathfinding algorithm.

There are several different ways to implement a priority queue, including using a binary heap, a sorted array, or a binary search tree. The appropriate implementation will depend on the specific requirements of the application. For example, a binary heap is a good choice for a priority queue that needs to support fast insertion and deletion of items, while a binary search tree is a good choice for a priority queue that needs to support fast retrieval of the highest priority item.