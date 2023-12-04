# Classes and Objects Cheat Sheet

Classes and objects in C++ provide a way to structure and organize code through encapsulation. Here's a quick reference guide.

## Classes

### Declaring a Class

```cpp
class MyClass {
public:
    // Member variables
    int myInt;
    double myDouble;

    // Member functions
    void printValues();
};
```

### Defining Class Functions

```cpp
void MyClass::printValues() {
    std::cout << "Int: " << myInt << ", Double: " << myDouble << std::endl;
}
```

### Constructors and Destructors

```cpp
class MyClass {
public:
    // Constructor
    MyClass(int i, double d) : myInt(i), myDouble(d) {
        // Initialization code
    }

    // Destructor
    ~MyClass() {
        // Cleanup code
    }
};
```

### Access Modifiers

- `public`: Members are accessible from outside the class.
- `private`: Members are only accessible within the class.

### Encapsulation

Encapsulation hides the implementation details of a class from the outside world.

```cpp
class BankAccount {
private:
    double balance;

public:
    void deposit(double amount) {
        // Implementation
    }

    void withdraw(double amount) {
        // Implementation
    }
};
```

## Objects

### Creating Objects

```cpp
MyClass obj; // Default constructor
MyClass objWithValues(10, 3.14); // Constructor with parameters
```

### Accessing Members

```cpp
obj.myInt = 42;
obj.myDouble = 2.718;

obj.printValues();
```

### Member Functions

```cpp
obj.printValues();
```

### Dynamic Objects

```cpp
MyClass* dynamicObj = new MyClass(5, 1.618);
dynamicObj->printValues();

delete dynamicObj; // Don't forget to free the memory
```

## Inheritance

### Base Class

```cpp
class Animal {
public:
    void eat() {
        std::cout << "Animal is eating" << std::endl;
    }
};
```

### Derived Class

```cpp
class Dog : public Animal {
public:
    void bark() {
        std::cout << "Dog is barking" << std::endl;
    }
};
```

### Polymorphism

```cpp
Animal* myDog = new Dog();
myDog->eat(); // Calls the eat() method from the base class
delete myDog;
```

Understanding classes and objects is fundamental to object-oriented programming in C++. Use them to model real-world entities and create well-organized, maintainable code.

Happy coding!
