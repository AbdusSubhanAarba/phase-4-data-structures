# Queues

## Overview

A queue is a **linear data structure** that stores elements in a specific order based on the **First In, First Out (FIFO)** principle. This means the first element added to the queue is the first one to be removed.

You can think of a queue as a line of people waiting at a supermarket checkout. The first person to join the line is the first person to be served.

Queues are widely used in operating systems, networking, scheduling, and many real-world applications where tasks must be processed in the order they arrive.

---

## Why It Matters

Queues are important because they:

- Process data in a fair order
- Efficiently manage waiting tasks
- Schedule jobs and requests
- Handle asynchronous operations
- Manage resources in operating systems
- Are widely used in networking and web servers

Many modern software systems rely on queues behind the scenes.

---

## How a Queue Works

A queue has two ends:

- **Front** → The first element to be removed.
- **Rear** → The position where new elements are added.

Example:

```text
Front                           Rear
  ↓                               ↓
+------+------+------+------+
|  10  |  20  |  30  |  40  |
+------+------+------+------+
```

If a new element (**50**) is added, it goes to the **rear**.

```text
Front                               Rear
  ↓                                   ↓
+------+------+------+------+------+
|  10  |  20  |  30  |  40  |  50  |
+------+------+------+------+------+
```

If an element is removed, **10** is removed first because it entered the queue first.

---

## The FIFO Principle

Queues follow the **First In, First Out (FIFO)** rule.

Example:

```text
Enqueue 10

Enqueue 20

Enqueue 30
```

Queue:

```text
Front → 10 → 20 → 30 ← Rear
```

Removing elements:

```text
Dequeue → 10

Dequeue → 20

Dequeue → 30
```

The first element inserted is always the first one removed.

---

## Common Queue Operations

### Enqueue

Adds a new element to the rear of the queue.

Example:

Before:

```text
Front → 10 → 20 ← Rear
```

Enqueue **30**

After:

```text
Front → 10 → 20 → 30 ← Rear
```

---

### Dequeue

Removes the element at the front of the queue.

Example:

Before:

```text
Front → 10 → 20 → 30 ← Rear
```

Dequeue

After:

```text
Front → 20 → 30 ← Rear
```

---

### Front (Peek)

Returns the first element without removing it.

Example:

```text
Front → 10 → 20 → 30
```

Front returns:

```text
10
```

The queue remains unchanged.

---

### Is Empty

Checks whether the queue contains any elements.

If the queue has no elements:

```text
True
```

Otherwise:

```text
False
```

---

## Advantages of Queues

Queues provide several benefits:

- Fair processing order
- Fast insertion at the rear
- Fast removal from the front
- Efficient task scheduling
- Simple implementation

---

## Disadvantages of Queues

Queues also have some limitations:

- Only the front element can be removed.
- Random access is not possible.
- Searching requires checking elements one by one.
- Not suitable when the newest element should be processed first.

---

## Real-World Examples

Queues are used in many everyday situations.

### Supermarket Checkout

Customers join the line in order.

The first customer in line is served first.

---

### Printer Queue

When several documents are sent to a printer:

```text
Document A

↓

Document B

↓

Document C
```

The printer prints them in the same order they were received.

---

### Customer Support

Support tickets are often handled in the order they arrive.

The oldest request is usually processed first.

---

### CPU Task Scheduling

Operating systems use queues to decide which task should run next.

Tasks wait in a queue until the CPU is ready to process them.

---

### Web Servers

When thousands of users visit a website simultaneously, incoming requests are often placed in queues and processed one by one.

---

## Time Complexity

| Operation | Time Complexity |
|-----------|----------------:|
| Enqueue | O(1) |
| Dequeue | O(1) |
| Front (Peek) | O(1) |
| Is Empty | O(1) |
| Search | O(n) |

Queues are efficient because insertion and deletion happen at opposite ends.

---

## Stacks vs Queues

| Stacks | Queues |
|--------|--------|
| Last In, First Out (LIFO) | First In, First Out (FIFO) |
| Insert and remove from the top | Insert at the rear, remove from the front |
| Used for undo operations | Used for scheduling and task processing |
| Browser Back button | Printer queues and waiting lines |

Although both are linear data structures, they solve different types of problems.

---

## Common Mistakes Beginners Make

Beginners often:

- Confuse **FIFO** with **LIFO**.
- Try to remove elements from the rear.
- Assume queues allow random access like arrays.
- Forget that only the front element is removed.
- Dequeue from an empty queue without checking first.

Understanding the FIFO principle helps avoid these mistakes.

---

## Key Takeaways

- A queue is a linear data structure.
- It follows the **First In, First Out (FIFO)** principle.
- Elements are added using **Enqueue**.
- Elements are removed using **Dequeue**.
- **Front (Peek)** returns the first element without removing it.
- Queues are widely used in scheduling, networking, operating systems, and real-world waiting systems.

---

## Summary

A queue is a linear data structure that follows the **First In, First Out (FIFO)** principle, ensuring that elements are processed in the order they arrive. This makes queues ideal for task scheduling, request handling, printer management, customer service systems, and many other real-world applications. Understanding queues is essential because they are one of the most widely used data structures in software engineering and computer science.
