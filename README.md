# Linked List Implementation in Python (From Scratch)

This project contains a **complete Linked List implementation written from scratch in Python**, without using any built-in list methods. The goal of this project is to deeply understand how linked lists work at a **memory and pointer level**, which is critical for Data Structures & Algorithms (DSA).

---

## 📌 Why This Project?

Most beginners rely on Python lists without understanding what happens internally. This project was intentionally built **from zero** to:

* Strengthen logical thinking
* Understand node connections (references)
* Practice traversal and edge cases
* Build confidence in DSA fundamentals

This is not a copy–paste implementation. Every function is written manually to learn *how and why* linked lists work.

---

## 🧱 Structure Overview

### 1️⃣ Node Class

Each node contains:

* `data` → value stored in the node
* `next` → reference to the next node

```python
class node:
    def __init__(self, value):
        self.data = value
        self.next = None
```

---

### 2️⃣ LinkedList Class

The `linkedlist` class manages the entire list and provides multiple operations.

It maintains:

* `head` → starting node of the list
* `n` → total number of nodes

---

## 🔧 Implemented Operations

### 🔹 Insertion Operations

* `inserthead(value)` → Insert node at the beginning
* `append(value)` → Insert node at the end
* `insert_after(after, value)` → Insert node after a specific value

---

### 🔹 Deletion Operations

* `delete_head()` → Delete first node
* `pop()` → Delete last node
* `remove(value)` → Delete node by value
* `clear()` → Remove all nodes from the list

---

### 🔹 Searching & Access

* `search(item)` → Returns index of element (if found)
* `__getitem__(index)` → Access element using index (array-like access)
* `__len__()` → Returns length of linked list

---

### 🔹 Advanced Operations

* `reverse()` → Reverse linked list using iterative method
* `replace_max(value)` → Replace maximum value in list
* `odd_sum_index()` → Sum of elements at odd indices
* `remove_dupl()` → Remove duplicate elements
* `clear_data(value)` → Custom data-cleaning logic

---

## ▶️ Execution Flow

Example usage:

```python
l = linkedlist()

l.inserthead(2)
l.inserthead(5)
l.inserthead(10)
l.inserthead(15)
l.inserthead(25)
l.inserthead(35)

l.append(45)
l.insert_after(5, 6)

l.clear()

l.inserthead(2)
l.inserthead(5)
l.inserthead(10)
l.inserthead(15)
l.inserthead(25)
l.inserthead(35)

l.delete_head()

l.inserthead(45)
l.inserthead(6)
l.inserthead(4)
l.inserthead(456)

l.pop()
l.remove(45)

print(l.search(5))
print(l[2])
print(l)
```

---

## 🧠 Key Learnings

* How pointers (`next`) connect nodes
* How traversal works in linear data structures
* Handling edge cases (empty list, single node)
* Why linked lists are memory-efficient for insert/delete
* Difference between array indexing and linked list traversal

---

## 🚀 What’s Next?

Planned extensions:

* Stack using Linked List
* Queue using Linked List
* Doubly Linked List
* Circular Linked List
* Time & Space Complexity analysis

---

## 🧑‍💻 Author

Built with discipline, patience, and consistency.

If you are learning DSA and feel slow — you are not behind.
You are building foundations.

---

⭐ If this helped you understand Linked Lists better, feel free to star or fork this project.
