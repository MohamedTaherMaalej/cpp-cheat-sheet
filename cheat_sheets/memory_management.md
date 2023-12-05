# Memory Management Cheat Sheet

Memory management in C++ is a crucial aspect of programming. Understanding how to allocate and deallocate memory is essential for creating efficient and robust applications.

## Dynamic Memory Allocation

### 1. `new` Operator

```cpp
int* myInt = new int; // Allocate memory for an integer
*myInt = 42;          // Assign a value
delete myInt;         // Deallocate memory
```

### 2. `new[]` Operator (Arrays)

```cpp
int* myArray = new int[5]; // Allocate memory for an integer array
myArray[2] = 3;           // Assign a value to the third element
delete[] myArray;         // Deallocate memory for the array
```

### 3. `malloc` and `free` Functions

```cpp
int* myInt = static_cast<int*>(malloc(sizeof(int))); // Allocate memory
*myInt = 42;                                       // Assign a value
free(myInt);                                       // Deallocate memory
```

### 4. `calloc` and `realloc` Functions

```cpp
int* myArray = static_cast<int*>(calloc(5, sizeof(int))); // Allocate and zero-initialize memory for an integer array
myArray = static_cast<int*>(realloc(myArray, 10 * sizeof(int))); // Reallocate memory for a larger array
free(myArray);                                            // Deallocate memory
```

## Automatic Memory Management

### 1. Stack Memory

```cpp
int stackVariable = 10; // Memory allocated on the stack
```

### 2. Automatic Arrays

```cpp
int myArray[5]; // Memory allocated on the stack
```

### 3. RAII (Resource Acquisition Is Initialization)

Use smart pointers and other RAII principles to manage resources automatically.

```cpp
#include <memory>

std::unique_ptr<int> myInt = std::make_unique<int>(42);
// Memory is automatically deallocated when myInt goes out of scope
```

## Memory Leaks

Avoiding memory leaks is crucial for maintaining the performance of your application.

```cpp
// Memory leak example
int* myInt = new int;
// Missing delete or delete[] statement
```

Use smart pointers and follow best practices to minimize the risk of memory leaks.

## Pointers and Ownership

Understand and manage ownership to prevent dangling pointers and memory access issues.

```cpp
int* myInt = new int;
std::unique_ptr<int> mySmartPtr = std::make_unique<int>(42);

// Avoid mixing raw pointers and smart pointers
```

Memory management is a critical skill in C++. Make sure to free memory properly and use modern C++ features, such as smart pointers, to automate memory management when possible.

Happy coding!

