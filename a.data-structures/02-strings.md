# Strings

## Overview

A string is a **sequence of characters** used to represent text. Characters can include letters, numbers, symbols, and spaces. In programming, strings are one of the most commonly used data types because they allow applications to store and manipulate textual information.

Although a string may look like a single piece of text, it is actually a collection of individual characters stored in order.

---

## Why It Matters

Strings are important because they:

- Store text and words
- Represent user input
- Display messages to users
- Process names, emails, and passwords
- Handle file names and web addresses
- Are used in almost every software application

Without strings, programs would not be able to work with text.

---

## How a String Works

Think of a string as a row of characters placed next to each other.

Example:

```text
"HELLO"
```

Internally, it is stored like this:

```text
Index:      0    1    2    3    4

Characters: H    E    L    L    O
```

Each character has its own position (index).

---

## String Indexing

Just like arrays, most programming languages start indexing strings from **0**.

Example:

```text
String = "Computer"

Index:

0 → C
1 → o
2 → m
3 → p
4 → u
5 → t
6 → e
7 → r
```

To access the letter **m**, use index **2**.

---

## Characteristics of Strings

Strings have several important characteristics:

- Store characters in order
- Each character has an index
- Can contain letters, numbers, symbols, and spaces
- Have a specific length
- Can be accessed character by character

Some programming languages allow strings to be modified directly, while others treat them as immutable (unchangeable).

---

## Common String Operations

### Access

Retrieve a character using its index.

Example:

```text
String:

"Apple"

Access index 1

Result:

p
```

---

### Concatenation

Join two or more strings together.

Example:

```text
"Hello"

+

" World"

↓

"Hello World"
```

---

### Length

Find the total number of characters.

Example:

```text
"Programming"

Length:

11
```

Spaces and punctuation also count as characters.

---

### Search

Find whether a character or word exists inside a string.

Example:

```text
"Software Engineering"

Search:

"Engineering"

↓

Found
```

---

### Comparison

Check whether two strings are the same.

Example:

```text
"apple"

==

"apple"

↓

True
```

---

## Advantages of Strings

Strings offer many benefits:

- Easy to store text
- Simple to display information
- Efficient for handling user input
- Supported by every programming language
- Provide many built-in operations

---

## Limitations of Strings

Strings also have some limitations:

- Large strings use more memory.
- Searching long strings can take time.
- Some programming languages do not allow direct modification of strings.
- Frequent modifications may reduce performance.

---

## Real-World Examples

Strings are used everywhere in software.

Examples include:

- Usernames
- Passwords
- Email addresses
- Phone numbers
- File names
- Website URLs
- Chat messages
- Search queries
- Product names

Almost every application processes strings.

---

## Time Complexity

| Operation | Time Complexity |
|-----------|----------------:|
| Access Character | O(1) |
| Search | O(n) |
| Compare | O(n) |
| Concatenate | O(n) |
| Traverse | O(n) |

The exact performance depends on the programming language and implementation.

---

## Strings vs Arrays

| Strings | Arrays |
|---------|--------|
| Store characters | Store any data type |
| Represent text | Represent collections of data |
| Indexed | Indexed |
| Usually used for words and sentences | Used for numbers, objects, and many other values |

A string can be thought of as a specialized array of characters.

---

## Common Mistakes Beginners Make

Beginners often:

- Forget that string indexing starts at 0.
- Confuse the length of a string with its last index.
- Forget that spaces count as characters.
- Assume strings can always be modified directly.
- Access indexes that do not exist.

Understanding how strings are stored helps avoid these mistakes.

---

## Key Takeaways

- A string is a sequence of characters.
- Each character has an index.
- Strings are used to store and process text.
- Common operations include access, concatenation, searching, comparison, and finding length.
- Strings are among the most frequently used data types in programming.

---

## Summary

Strings are one of the most essential data types in computer science. They allow programs to store, process, and manipulate text efficiently. By understanding how strings are organized, indexed, and operated on, software engineers can build applications that handle everything from usernames and passwords to documents, websites, and communication systems.
