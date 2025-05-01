# 🧠 C Programming Complete Roadmap

## 🔰 1. Introduction to C
- History of C
- Features of C
- Structure of a C program
- Compilation & Execution process (preprocessing, compiling, linking)

## 📘 2. Basics of C
- Keywords & Identifiers
- Variables & Constants
- Data Types (int, float, char, double, etc.)
- `printf()` and `scanf()`
- Comments (`//`, `/* */`)
- Typecasting

## 🧮 3. Operators and Expressions
- Arithmetic Operators
- Relational Operators
- Logical Operators
- Bitwise Operators
- Assignment Operators
- Unary Operators
- Ternary Operator
- Operator Precedence & Associativity

## 🔁 4. Control Flow / Decision Making
- `if`, `if-else`, `if-else-if`
- `switch-case`
- `goto`, `break`, `continue`

## 🔄 5. Loops
- `for`, `while`, `do-while` loops
- Nested loops
- Loop optimization tricks

## 📂 6. Functions
- Function declaration & definition
- Call by value vs call by reference
- Recursion
- Inline functions (using macros)
- Scope & lifetime of variables (`auto`, `static`, `extern`, `register`)

## 📚 7. Arrays
- One-dimensional arrays
- Multi-dimensional arrays
- Array manipulation (search, sort)
- Array as function arguments

## 🔤 8. Strings
- Character arrays
- String functions (`strlen`, `strcpy`, `strcmp`, etc.)
- Manual string operations (without using `<string.h>`)

## 🎯 9. Pointers
- Introduction to pointers
- Pointer arithmetic
- Pointers and arrays
- Pointers and functions
- Pointers to pointers
- Pointers and strings
- Void pointers
- Function pointers
- Wild pointers, Dangling pointers
- Pointers to const and const pointers

## 🧱 10. Structures and Unions
- Defining and using structures
- Nested structures
- Array of structures
- Structure padding & packing
- Unions and memory optimization
- Bitfields in structures

## 📦 11. Dynamic Memory Allocation
- `malloc()`, `calloc()`, `realloc()`, `free()`
- Memory leaks & management
- Custom memory allocator (for advanced mastery)

## 🗃️ 12. File Handling
- File pointers
- `fopen`, `fclose`, `fscanf`, `fprintf`, `fgets`, `fputs`, `fread`, `fwrite`
- Binary vs text file operations
- Random access in files (`fseek`, `ftell`, `rewind`)
- Error handling in files

## ⚙️ 13. Preprocessor Directives
- `#define`, `#include`, `#ifdef`, `#ifndef`, `#endif`
- Macros with arguments
- Conditional compilation
- `#undef`, `#pragma`

## 🧩 14. Advanced C Topics
- Memory segmentation (stack, heap, data, text)
- Command line arguments
- Variable argument functions (`stdarg.h`)
- Dynamic arrays with realloc
- Function pointers & callback functions
- Modular programming (multiple source files)
- Linking static and dynamic libraries

## 🏗️ 15. Data Structures in C
- Linked List (Singly, Doubly, Circular)
- Stack & Queue (with arrays & linked list)
- Trees (Binary Trees, BSTs, AVL Trees)
- Graphs (Adjacency matrix/list)
- Hash tables (basic implementation)
- Searching and Sorting algorithms

## 🧪 16. Debugging and Testing
- Using `gdb` (GNU Debugger)
- Debugging segmentation faults
- Writing test cases
- Memory checkers (`valgrind`)

## 🧠 17. Compilation Process and Internals
- Preprocessor, Compiler, Assembler, Linker
- Compilation stages and `.o` files
- Understanding symbol tables
- Assembly code from C code

## 🖥️ 18. System Programming (Advanced)
- Using system calls (like `fork`, `exec`, `wait`, `pipe`, etc.)
- File descriptors
- Signals
- Interprocess Communication (IPC)
- Threading (using `pthreads`)

## 📲 19. Embedded C Concepts (Optional but Powerful)
- Register-level programming
- Accessing hardware
- Interrupts
- Memory-mapped I/O
- Bare-metal programming

## 🏁 20. Projects to Solidify Mastery
- Bank Management System
- Custom Shell in C
- Mini Compiler
- Library Management System
- Student Record System using Files
- Memory Allocator (malloc implementation)
- Text Editor like Nano
- TCP/UDP Chat App using Sockets

## 🧰 21. Important Tools, Libraries, and Frameworks Used in Industry

### 🧪 Development Tools
- **GCC (GNU Compiler Collection)** – Standard C compiler
- **Clang/LLVM** – Modern, fast compiler used in many open source projects
- **Make & CMake** – Build systems to compile and link large C projects
- **GDB (GNU Debugger)** – Powerful debugging tool for C
- **Valgrind** – Memory leak detector and profiling tool
- **gcov / lcov** – Code coverage analysis tools
- **strace** – Traces system calls made by a program
- **ltrace** – Traces library calls

### 📚 Libraries to Learn
- **GLib** – Low-level core library (used in GNOME)
- **libcurl** – Transfer data with URL syntax (HTTP, FTP, etc.)
- **zlib** – Compression library
- **OpenSSL** – Cryptographic library used in secure communications
- **SQLite** – Lightweight, embedded SQL database engine written in C
- **cJSON** – Lightweight JSON parser in C
- **ncurses** – Terminal-based user interfaces
- **libevent / libev** – Event-driven programming for network applications
- **ZeroMQ** – High-performance messaging library
- **pthread** – POSIX threading library (used in multi-threaded apps)

### 🧱 Frameworks & Systems-Level Libraries
- **Linux Kernel Development** – Low-level system development in C
- **Embedded C frameworks** (e.g., **CMSIS**, **FreeRTOS**)
- **Contiki OS** – Operating system for IoT devices
- **Zephyr RTOS** – Scalable real-time OS used in embedded devices
- **GNOME/GTK** – GUI framework for Linux (uses C)
- **Apache APR (Portable Runtime)** – Utility library used in the Apache web server

### 🧑‍💻 IDEs and Editors (C Friendly)
- **Visual Studio Code** with C/C++ extensions
- **CLion** (JetBrains)
- **Code::Blocks**
- **Eclipse CDT**
- **Vim / Neovim** with C plugins

### 🧠 Version Control and Collaboration Tools
- **Git**
- **GitHub / GitLab / Bitbucket**
- **CI/CD Tools (e.g., Jenkins, Travis CI)** – Automating builds & tests for C projects

### 🔒 Security-Focused Tools
- **AddressSanitizer (ASan)** – Finds memory errors like buffer overflows
- **Coverity** – Static analysis tool used in companies
- **Fortify** – Enterprise security analysis suite
