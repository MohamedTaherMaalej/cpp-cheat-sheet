# Control Flow Cheat Sheet

Control flow structures allow you to control the flow of execution in your C++ program. These structures include conditional statements, loops, and branching mechanisms.

## Conditional Statements

### 1. If Statement

```cpp
if (condition) {
    // Code to execute if the condition is true
} else {
    // Code to execute if the condition is false
}
```

### 2. Switch Statement

```cpp
switch (expression) {
    case value1:
        // Code to execute if expression equals value1
        break;
    case value2:
        // Code to execute if expression equals value2
        break;
    // ... more cases ...
    default:
        // Code to execute if no case matches
}
```

## Loops

### 1. For Loop

```cpp
for (initialization; condition; update) {
    // Code to repeat as long as the condition is true
}
```

### 2. While Loop

```cpp
while (condition) {
    // Code to repeat as long as the condition is true
}
```

### 3. Do-While Loop

```cpp
do {
    // Code to repeat at least once, and then as long as the condition is true
} while (condition);
```

## Branching

### 1. Break Statement

Used to exit from a loop or switch statement.

```cpp
while (true) {
    // Code
    if (condition) {
        break; // Exit the loop
    }
    // More code
}
```

### 2. Continue Statement

Used to skip the rest of the loop's body and move to the next iteration.

```cpp
for (int i = 0; i < 10; ++i) {
    if (i % 2 == 0) {
        continue; // Skip even numbers
    }
    // Code for odd numbers
}
```

### 3. Goto Statement (Avoid if possible)

```cpp
goto label;
// Code
label:
// More code
```

Note: The use of the `goto` statement is generally discouraged, as it can make code less readable and harder to maintain.

Remember to use control flow structures wisely to create clear and efficient code. Improper use may lead to code that is difficult to understand and maintain.

Happy coding!
