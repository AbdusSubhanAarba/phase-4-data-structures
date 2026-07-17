# Arrays

## Overview

An array is a **linear data structure** that stores multiple values of the same type in a single collection. Each value is stored in a specific position called an **index**, allowing it to be accessed quickly.

Arrays are one of the most fundamental data structures in computer science and are widely used in programming because they provide fast access to data.

---

## Why It Matters

Arrays are important because they:

- Store multiple values efficiently
- Provide fast access to elements using indexes
- Are simple to understand and use
- Form the foundation for many other data structures
- Are commonly used in algorithms and real-world applications

Nearly every programming language supports arrays.

---

## How an Array Works

Imagine you have a row of numbered lockers.

Each locker stores one item, and each locker has its own number.

An array works the same way.

Example:

```text
Index:   0    1    2    3    4

Array:  [10] [25] [30] [45] [50]
```

The computer uses the index to locate an element directly.

---

## Array Indexing

The position of each element is called its **index**.

Most programming languages start counting from **0**.

Example:

```text
Array = [Apple, Banana, Orange, Mango]

Index:

0 → Apple
1 → Banana
2 → Orange
3 → Mango
```

To access **Orange**, you use index **2**.

---

## Characteristics of Arrays

Arrays have several important characteristics:

- Elements are stored in contiguous memory locations.
- Every element has an index.
- Elements are accessed directly using their index.
- Arrays usually have a fixed size after creation (depending on the programming language).
- All elements typically store the same data type.

---

## Common Array Operations

### Access

Retrieve an element using its index.

Example:

```text
Array = [5, 10, 15, 20]

Access index 2

Result:

15
```

Accessing an element is extremely fast.

---

### Update

Replace the value stored at an index.

Example:

```text
Before:

[10, 20, 30]

Update index 1 to 25

After:

[10, 25, 30]
```

---

### Traversal

Visit every element one by one.

Example:

```text
[10, 20, 30, 40]

↓

10

20

30

40
```

Traversal is commonly performed using loops.

---

### Insertion

Adding a new element may require shifting existing elements.

Example:

```text
Before:

[10, 20, 40]

Insert 30

After:

[10, 20, 30, 40]
```

Elements after the insertion point must move one position.

---

### Deletion

Removing an element also requires shifting elements.

Example:

```text
Before:

[10, 20, 30, 40]

Delete 20

After:

[10, 30, 40]
```

The remaining elements move to fill the empty space.

---

## Advantages of Arrays

Arrays provide several benefits:

- Very fast access to elements
- Easy to use
- Memory-efficient
- Simple to traverse
- Excellent for storing ordered data

---

## Disadvantages of Arrays

Arrays also have some limitations:

- Fixed size in many programming languages
- Inserting elements can be slow
- Deleting elements can be slow
- Wasted memory if the array is larger than needed
- All elements are usually the same data type

Other data structures, such as linked lists, solve some of these limitations.

---

## Real-World Examples

Arrays are used in many everyday applications.

Examples include:

- Monthly sales figures
- Student grades
- Product prices
- High-score lists in games
- Temperature readings
- Daily expenses
- Lists of usernames

Any ordered collection of similar items can often be stored using an array.

---

## Time Complexity

| Operation | Time Complexity |
|-----------|----------------:|
| Access | O(1) |
| Search | O(n) |
| Update | O(1) |
| Insert | O(n) |
| Delete | O(n) |

Fast access is one of the biggest advantages of arrays.

---

## Common Mistakes Beginners Make

Beginners often:

- Forget that indexing usually starts at 0.
- Access an index that does not exist.
- Confuse an index with the value stored at that index.
- Assume inserting or deleting elements is always fast.
- Try to store different data types in arrays that require a single type.

---

## Key Takeaways

- An array is a linear data structure.
- Elements are stored in contiguous memory locations.
- Each element has an index.
- Arrays provide very fast random access.
- Insertion and deletion are generally slower because elements may need to be shifted.
- Arrays are one of the most widely used data structures in programming.

---

## Summary

Arrays are one of the most important data structures in computer science. They store collections of data in contiguous memory and allow fast access using indexes. While arrays are simple and efficient for reading and updating data, inserting or removing elements can be more expensive because other elements may need to shift. Understanding arrays provides the foundation for learning more advanced data structures and algorithms.
