# Sorted Linked List in C++

A menu-driven C++ program that implements a **Sorted Singly Linked List** using structures, pointers, and dynamic memory allocation.

Every insertion keeps the list in **ascending order**. Duplicate values are allowed.

## Features

* **Random Data Generation:** Asks for the number of nodes `n`, generates `n` random numbers, and displays the list **before** and **after** sorting.
* **Sorted Insertion:** Inserts each new node at its correct position. If the value already exists, the new node is placed **after the last occurrence**.
* **Delete by Value:** Deletes the **last occurrence** of the given value, or shows `Value not found!`.
* **Search:** Finds the **first occurrence** of a value and shows its position.
* **Display:** Prints all elements in sorted order.
* **Efficient Traversal:** Delete and search stop early once `data > value`, since the list is sorted.
* **Memory Safety:** Handles allocation failure (`new (nothrow)`), frees nodes on deletion, and clears the whole list on exit.
* **Input Validation:** Invalid (non-numeric) input never crashes or freezes the menu.
* **Empty List Handling:** Shows `List is empty!` when there is nothing to display or delete.

## Menu Interface

```text
+-+-+-+-+-+-+-+-+-+-+-+-+-+-
     Sorted Linked List
+-+-+-+-+-+-+-+-+-+-+-+-+-+-

1. Insert
2. Delete
3. Search
4. Display
5. Exit
----------------------------
Enter choice:
```

## Sample Output

Values are random, so your output will differ.

### Initial List Creation

```text
Enter number of nodes: 8

Before Sorting: 41 67 34 0 69 24 78 58

After Sorting:
Sorted Linked List: 0 24 34 41 58 67 69 78
```

### Insertion

```text
Enter choice: 1
Enter value: 41
Value inserted!
```

The new `41` is placed after the existing `41`:

```text
Sorted Linked List: 0 24 34 41 41 58 67 69 78
```

### Deletion

```text
Enter choice: 2
Enter value: 41
Value deleted!
```

Only the **last** `41` is removed.

### Search

```text
Enter choice: 3
Enter value: 41
Item found!
Position: 4
```

Position of the **first** occurrence. If the value does not exist, the program prints `Item not found!`.

## Functions

| Function | Purpose |
|---|---|
| `readInt(int &x)` | Safely reads an integer; returns `false` on invalid input. |
| `insert(int val)` | Creates a node and inserts it in sorted order (after the last duplicate). |
| `print()` | Displays the list in sorted order. |
| `Delete(int val)` | Deletes the last occurrence of `val` and frees its memory. |
| `search(int item)` | Shows the position of the first occurrence of `item`. |
| `clearList()` | Deletes all remaining nodes before exit. |
| `randomInsert()` | Generates random numbers, shows before/after sorting. |
| `menu()` | Displays the menu and calls the chosen operation. |
| `main()` | Calls `randomInsert()` and then `menu()`. |

## Technologies Used

* **Language:** C++
* **Data Structure:** Singly Linked List
* **Concepts:** Structures, Pointers, Dynamic Memory Allocation, Loops, Functions, Conditional Statements

## How to Run

1. Clone or download this repository.
2. Open `main.cpp` in a C++ IDE or editor.
3. Compile and run.

### Compile with GCC

```bash
g++ main.cpp -o main
```

### Run

```bash
main.exe
```

> **Note:** The program uses `system("cls")` and `system("pause")`, so it is intended for **Windows**. On Linux/macOS, replace them with `system("clear")` and `cin.get()`.

## Time Complexity

| Operation | Complexity |
|---|---|
| Insert | O(n) |
| Delete | O(n) |
| Search | O(n) |
| Display | O(n) |

## Learning Objectives

* Understand the structure and operation of a singly linked list.
* Practice inserting nodes in sorted order, including duplicates.
* Implement deletion of the last occurrence and search for the first occurrence.
* Understand pointers, dynamic memory allocation, and memory cleanup in C++.

---

**Language:** C++
**Project Type:** Data Structures
**Author:** Mahee
