# Variables and Data Types Cheat Sheet

## Variables

In C++, variables are used to store and manipulate data. They must be declared before use, specifying their data type.

### Variable Declaration

```cpp
// Syntax: data_type variable_name;
int age;
double price;
char grade;
```

### Initializing Variables

```cpp
// Syntax: data_type variable_name = value;
int count = 0;
double pi = 3.14;
char initial = 'A';
```

### Constants

Use `const` keyword to define constants.

```cpp
const double PI = 3.1415926535;
const int MAX_VALUE = 100;
```

## Data Types

C++ supports various data types, including fundamental types and user-defined types.

### Fundamental Data Types

- **Integers**: `int`, `short`, `long`, `long long`
- **Floating-point Numbers**: `float`, `double`
- **Characters**: `char`
- **Boolean**: `bool`

### Modifiers

- **Signed and Unsigned**: `signed`, `unsigned`
- **Size Modifiers**: `short`, `long`, `long long`

### User-Defined Data Types

- **Enumerations**

```cpp
enum Color { RED, GREEN, BLUE };
Color myColor = GREEN;
```

- **Structures**

```cpp
struct Person {
    std::string name;
    int age;
};
Person student = {"Alice", 20};
```

- **Classes**

```cpp
class Car {
public:
    std::string brand;
    int year;
    // Constructors, methods, etc.
};
Car myCar;
```

## Type Casting

C++ allows converting one data type to another.

### Implicit Casting

```cpp
int intValue = 10;
double doubleValue = intValue; // Implicit casting from int to double
```

### Explicit Casting

```cpp
double doubleValue = 3.14;
int intValue = static_cast<int>(doubleValue); // Explicit casting from double to int
```

## Sizeof Operator

The `sizeof` operator returns the size (in bytes) of a variable or data type.

```cpp
int sizeOfInt = sizeof(int);
```

Remember to choose the appropriate data type based on the requirements of your program to optimize memory usage and ensure accurate representation of data.

Happy coding!
