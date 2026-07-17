# Stacks

## Overview

A stack is a **linear data structure** that stores elements in a specific order based on the **Last In, First Out (LIFO)** principle. This means the last element added to the stack is the first one to be removed.

You can think of a stack as a pile of books. You place a new book on top of the pile, and when you remove one, you always take the top book first.

Stacks are widely used in programming to manage function calls, undo operations, expression evaluation, and many other tasks.

---

## Why It Matters

Stacks are important because they:

- Store data in a predictable order
- Make insertion and removal very efficient
- Support recursion and function calls
- Power undo and redo features
- Are used in compilers and expression evaluation
- Form the foundation for many algorithms

Almost every programming language uses stacks internally.

---

## How a Stack Works

A stack only allows operations at **one end**, called the **top**.

Example:

```text
Top
 ↓
+------+
|  30  |
+------+
|  20  |
+------+
|  10  |
+------+
```

If a new element (40) is added:

```text
Top
 ↓
+------+
|  40  |
+------+
|  30  |
+------+
|  20  |
+------+
|  10  |
+------+
```

If an element is removed, **40** is removed first because it was the last element added.

---

## The LIFO Principle

Stacks follow the **Last In, First Out (LIFO)** rule.

Example:

```text
Push 10

Push 20

Push 30
```

Stack:

```text
Top
 ↓
30
20
10
```

Removing elements:

```text
Pop → 30

Pop → 20

Pop → 10
```

The last value inserted is always the first one removed.

---

## Common Stack Operations

### Push

Adds a new element to the top of the stack.

Example:

Before:

```text
20
10
```

Push **30**

After:

```text
30
20
10
```

---

### Pop

Removes the top element.

Example:

Before:

```text
30
20
10
```

Pop

After:

```text
20
10
```

---

### Peek (or Top)

Returns the top element without removing it.

Example:

```text
30
20
10
```

Peek returns:

```text
30
```

The stack remains unchanged.

---

### Is Empty

Checks whether the stack contains any elements.

If the stack has no elements:

```text
True
```

Otherwise:

```text
False
```

---

## Advantages of Stacks

Stacks provide several benefits:

- Very fast insertion
- Very fast deletion
- Simple implementation
- Efficient memory usage
- Excellent for managing temporary data

---

## Disadvantages of Stacks

Stacks also have some limitations:

- Only the top element can be accessed directly.
- Random access is not possible.
- Searching requires checking elements one by one.
- Not suitable when data must be accessed in any order.

---

## Real-World Examples

Stacks appear in many everyday applications.

Examples include:

### Undo Feature

When editing a document:

```text
Type A

Type B

Type C
```

Undo removes:

```text
C

↓

B

↓

A
```

---

### Browser History

When using the Back button:

```text
Google

↓

YouTube

↓

GitHub
```

Pressing Back returns:

```text
GitHub

↓

YouTube

↓

Google
```

---

### Function Calls

Programming languages use a **call stack** to keep track of active functions.

Each function call is placed on the stack.

When the function finishes, it is removed from the stack.

---

### Expression Evaluation

Stacks help evaluate mathematical expressions such as:

```text
(5 + 3) × 2
```

Compilers and calculators use stacks for this purpose.

---

## Time Complexity

| Operation | Time Complexity |
|-----------|----------------:|
| Push | O(1) |
| Pop | O(1) |
| Peek | O(1) |
| Is Empty | O(1) |
| Search | O(n) |

Stacks are highly efficient because all operations occur at the top.

---

## Arrays vs Stacks

| Arrays | Stacks |
|--------|--------|
| Access any index | Access only the top |
| Random access | Sequential removal |
| Multiple insertion positions | Insert only at the top |
| Flexible access | Follows the LIFO principle |

A stack can be implemented using an array or a linked list.

---

## Common Mistakes Beginners Make

Beginners often:

- Confuse **LIFO** with **FIFO**.
- Try to remove elements from the bottom.
- Forget that only the top element is directly accessible.
- Attempt random access like an array.
- Pop from an empty stack without checking first.

Understanding the LIFO principle prevents these mistakes.

---

## Key Takeaways

- A stack is a linear data structure.
- It follows the **Last In, First Out (LIFO)** principle.
- Elements are added using **Push**.
- Elements are removed using **Pop**.
- **Peek** returns the top element without removing it.
- Stacks are widely used for function calls, undo operations, browser history, and expression evaluation.

---

## Summary

A stack is a simple yet powerful data structure that stores elements using the **Last In, First Out (LIFO)** principle. Because insertion and deletion occur only at the top, stack operations are extremely efficient. Stacks are used extensively in programming, from managing function calls and recursion to implementing undo features, browser history, and mathematical expression evaluation.
