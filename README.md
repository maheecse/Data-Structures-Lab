# Sorted Linked List in C++

A menu-driven C++ project that implements a **Sorted Singly Linked List** using structures, pointers, and dynamic memory allocation.

The list automatically maintains elements in ascending order during insertion.

## Features

* **Sorted Insertion:** Inserts new nodes in ascending order automatically.
* **Delete by Position:** Deletes a node from a specified position.
* **Search:** Searches for a value and displays its position.
* **Display:** Prints all elements of the sorted linked list.
* **Random Data Generation:** Generates 20 random numbers when the program starts.
* **Menu-Driven Interface:** Provides an interactive console menu.
* **Empty List Handling:** Displays a message when the list is empty.
* **Dynamic Memory Allocation:** Uses `new` and `delete` to manage nodes.

## Menu Interface

The program displays the following menu:

```text
============================
     SORTED LINKED LIST
============================
1. Insert
2. Delete
3. Search
4. Display
5. Exit
============================
Enter choice:
```

## Sample Output

```text
--------- SORTED LINKED LIST ---------

       [1] Insert Node
       [2] Delete by Position
       [3] Search Value
       [4] Display List
       [5] Exit Program

Enter your choice: 4

Sorted Linked List: 125 340 567 890 1234 ...
```

*Note: The numbers shown above are examples. Actual values may vary because the program generates random numbers.*

### Example: Insertion

```text
Enter your choice: 1

Enter value: 250
Value inserted!
```

The new value is inserted into its correct position to maintain ascending order.

### Example: Deletion

```text
Enter your choice: 2

Enter position: 3
Node deleted successfully

After Deletion:
Sorted Linked List: ...
```

The node at the specified position is removed from the list.

### Example: Searching

```text
Enter your choice: 3

Enter value: 250
Item found!
Position: 2
```

If the value does not exist, the program displays `Item not found!`.

## Technologies Used

* **Language:** C++
* **Data Structure:** Singly Linked List
* **Concepts:** Structures, Pointers, Dynamic Memory Allocation, Loops, Functions, and Conditional Statements.

## How to Run

1. Clone or download this repository.
2. Open `main.cpp` in a C++ IDE or editor.
3. Compile and run the program using a C++ compiler.

### Compile with GCC

```bash
g++ main.cpp -o main
```

### Run

```bash
./main
```

On Windows, run:

```bash
main.exe
```

## Learning Objectives

* Understand the structure and operation of a singly linked list.
* Practice inserting nodes in sorted order.
* Learn how to delete nodes by position.
* Implement searching and displaying operations.
* Understand pointers and dynamic memory allocation in C++.

---

**Language:** C++
**Project Type:** Data Structures
**Author:** Mahee
