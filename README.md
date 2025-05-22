
#  BigInt: 1024-bit Integer Arithmetic in C

This project implements a custom `BigInt` data type in C that supports **1024-bit** integers. It includes operations for **addition (+)**, **subtraction (-)**, and **multiplication (*)**, supporting signed numbers and handling values much larger than native C data types can store.

##  Problem Statement

> Implement a `BigInt` data type with operations **+**, **-**, and **×**, capable of representing and manipulating **1024-bit integers** (up to 308 decimal digits).

---

##  Features

- Custom `BigInt` structure to represent 1024-bit numbers
- Operations supported:
  - ➕ Addition
  - ➖ Subtraction
  - ✖️ Multiplication
- Handles **positive** and **negative** integers
- Detects **overflow** when result exceeds 1024-bit limit
- Ignores leading zeros for output clarity

---

##  Data Structure

```c
typedef struct {
    char s[309]; // Supports up to 308 decimal digits + null terminator
    int sign;    // 1 for positive, -1 for negative
} bigint;
