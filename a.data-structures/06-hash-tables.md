# Hash Tables

## Overview

A hash table is a **data structure** that stores data as **key-value pairs**, allowing information to be stored and retrieved extremely quickly. Instead of searching through every element one by one, a hash table uses a **hash function** to calculate where a value should be stored.

Hash tables are one of the fastest and most commonly used data structures in computer science. They power features such as dictionaries, caches, databases, search engines, and user authentication systems.

---

## Why It Matters

Hash tables are important because they:

- Provide very fast data lookup
- Store information using key-value pairs
- Support efficient insertion and deletion
- Are widely used in real-world software
- Improve application performance

Many programming languages include built-in hash tables, such as **HashMap**, **Dictionary**, **Map**, or **Object**.

---

## How a Hash Table Works

A hash table stores data using two parts:

- **Key** → Used to identify the data.
- **Value** → The actual information being stored.

Example:

```text
Key           Value

"Name"   →    "Subhan"

"Age"    →    20

"Country"→    "Bahrain"
```

Instead of searching every entry, the hash table quickly finds the correct value using its key.

---

## What Is a Hash Function?

A **hash function** takes a key and converts it into a number called a **hash value**.

That number determines where the value will be stored in memory.

Example:

```text
Key

"Apple"

↓

Hash Function

↓

Hash Value

↓

Memory Location
```

The process happens automatically and is extremely fast.

---

## Key-Value Pairs

Every piece of data inside a hash table is stored as a **key-value pair**.

Example:

```text
Username

↓

"subhan123"

↓

Email

↓

subhan@email.com
```

The key uniquely identifies the stored value.

---

## Common Hash Table Operations

### Insert

Add a new key-value pair.

Example:

```text
Key:

"City"

Value:

"Manama"
```

The hash table stores the value using the key.

---

### Search

Retrieve a value using its key.

Example:

```text
Key:

"Country"

↓

Result:

"Bahrain"
```

Searching is usually extremely fast.

---

### Update

Change the value associated with an existing key.

Example:

Before:

```text
Age → 20
```

After:

```text
Age → 21
```

---

### Delete

Remove a key-value pair.

Example:

Before:

```text
Name → Ahmed
Age → 20
```

Delete:

```text
Age
```

Remaining:

```text
Name → Ahmed
```

---

## Hash Collisions

Sometimes two different keys produce the same hash value.

This is called a **collision**.

Example:

```text
Key A

↓

Hash Value 25

Key B

↓

Hash Value 25
```

Both keys want to use the same memory location.

Hash tables use techniques such as **chaining** or **open addressing** to handle collisions efficiently.

---

## Advantages of Hash Tables

Hash tables provide several benefits:

- Extremely fast searching
- Fast insertion
- Fast deletion
- Efficient for large amounts of data
- Easy to organize information using keys

These advantages make hash tables one of the most popular data structures.

---

## Disadvantages of Hash Tables

Hash tables also have some limitations:

- Performance depends on a good hash function.
- Collisions can reduce efficiency.
- Keys must usually be unique.
- Data is not stored in sorted order.

If ordered data is required, another data structure may be more suitable.

---

## Real-World Examples

Hash tables are used in many applications.

### User Accounts

```text
Username

↓

User Information
```

The username acts as the key.

---

### Phone Contacts

```text
Contact Name

↓

Phone Number
```

Searching for a contact is very fast because the name acts as the key.

---

### Dictionary

```text
Word

↓

Definition
```

Digital dictionaries use hash tables for fast lookups.

---

### Web Browser Cache

```text
Website URL

↓

Saved Web Page
```

The browser quickly checks whether a page is already stored.

---

### Databases

Many databases use hashing to quickly locate records.

---

## Time Complexity

| Operation | Average Time | Worst Case |
|-----------|-------------:|-----------:|
| Search | O(1) | O(n) |
| Insert | O(1) | O(n) |
| Delete | O(1) | O(n) |

In most real-world situations, hash tables provide nearly constant-time performance.

---

## Arrays vs Hash Tables

| Arrays | Hash Tables |
|--------|-------------|
| Access by index | Access by key |
| Ordered | Unordered |
| Search is usually O(n) | Search is usually O(1) |
| Best for sequential data | Best for quick lookups |

Each data structure is useful for different types of problems.

---

## Common Mistakes Beginners Make

Beginners often:

- Confuse keys with values.
- Assume hash tables keep data sorted.
- Forget that keys should usually be unique.
- Ignore the possibility of collisions.
- Think hash tables are always faster in every situation.

Understanding how hashing works helps avoid these misconceptions.

---

## Key Takeaways

- A hash table stores data as **key-value pairs**.
- A **hash function** determines where data is stored.
- Searching, inserting, and deleting are usually **O(1)**.
- Collisions occur when different keys map to the same location.
- Hash tables are widely used in databases, caches, search engines, and authentication systems.

---

## Summary

A hash table is one of the fastest and most powerful data structures in computer science. By using a hash function to map keys to memory locations, it allows data to be stored and retrieved efficiently. Although collisions can occur, modern collision-handling techniques keep performance high, making hash tables essential for building fast and scalable software applications.
