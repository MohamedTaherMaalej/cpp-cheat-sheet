# Functions Cheat Sheet

Functions in C++ allow you to modularize your code by dividing it into smaller, manageable pieces. Here's an overview of creating and using functions.

## Function Declaration and Definition

### Function Declaration

```cpp
// Syntax: return_type function_name(parameter_type parameter_name);
int add(int a, int b);
```

### Function Definition

```cpp
// Syntax: return_type function_name(parameter_type parameter_name) {
//     // Function body
//     return expression;
// }
int add(int a, int b) {
    return a + b;
}
```

## Function Parameters

### Pass by Value

```cpp
void printNumber(int num) {
    // Code
}
```

### Pass by Reference

```cpp
void increment(int &num) {
    num++;
}
```

### Default Parameters

```cpp
void greet(std::string name = "Guest") {
    // Code
}
```

## Return Statement

```cpp
int square(int x) {
    return x * x;
}
```

## Function Overloading

You can define multiple functions with the same name but different parameters.

```cpp
int add(int a, int b) {
    return a + b;
}

double add(double a, double b) {
    return a + b;
}
```

## Recursion

A function calling itself.

```cpp
int factorial(int n) {
    if (n <= 1) {
        return 1;
    }
    return n * factorial(n - 1);
}
```

## Inline Functions

```cpp
inline int multiply(int a, int b) {
    return a * b;
}
```

## Lambda Expressions (C++11 and later)

```cpp
auto sum = [](int a, int b) -> int {
    return a + b;
};
```

## Function Pointers

```cpp
int add(int a, int b) {
    return a + b;
}

int (*functionPointer)(int, int) = add;
int result = functionPointer(5, 3); // result is 8
```

Functions play a crucial role in structuring your code and promoting reusability. Use them judiciously to enhance the readability and maintainability of your programs.

Happy coding!
