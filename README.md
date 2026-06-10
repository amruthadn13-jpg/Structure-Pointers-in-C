# Structure Pointers in C

## Overview

This project demonstrates the use of **pointers with structures in C**. Instead of accessing structure members directly, a pointer is used to reference a structure and access its members using the **arrow (`->`) operator**.

Structure pointers are commonly used in large applications and embedded systems to improve memory efficiency and simplify data handling.

---

## Concepts Covered

- Structures (`struct`)
- Structure variables
- Pointers
- Structure pointers
- Address operator (`&`)
- Arrow operator (`->`)
- Formatted output using `printf()`

---

## Project Description

The program defines a structure named `Car` containing:

- Brand Name
- Manufacturing Year

A structure variable is initialized with sample data, and a pointer is created to store the address of that structure.

The pointer is then used to access and display the structure members.

---

## Structure Definition

```c
struct Car {
    char brand[30];
    int year;
};
```

The structure stores information about a car.

---

## Structure Initialization

```c
struct Car car = {"Toyota", 2020};
```

A structure variable is created and initialized with values.

---

## Creating a Structure Pointer

```c
struct Car *ptr = &car;
```

Here:

- `ptr` is a pointer to the structure
- `&car` returns the memory address of the structure variable

---

## Accessing Members Using Pointer

```c
ptr->brand
ptr->year
```

The arrow (`->`) operator is used to access structure members through a pointer.

It is equivalent to:

```c
(*ptr).brand
(*ptr).year
```

---

## Sample Output

```text
Brand: Toyota
Year: 2020
```

---

## Learning Outcomes

- Understanding structure pointers
- Using memory addresses with structures
- Accessing structure members through pointers
- Working with the arrow (`->`) operator

---

## Real-World Applications

- Embedded Systems Programming
- Device Driver Development
- Operating Systems
- Linked Lists
- Dynamic Memory Allocation
- Database and Record Management Systems

---

## Time Complexity

```text
O(1)
```

Accessing structure members through a pointer takes constant time.

---

## Space Complexity

```text
O(1)
```

Only one structure variable and one pointer are used.

---

## Key Takeaway

Structure pointers allow efficient access to structure data using memory addresses. The `->` operator provides a convenient way to access structure members through pointers and is widely used in real-world C programming.

---

## Author

**Amrutha D N**
