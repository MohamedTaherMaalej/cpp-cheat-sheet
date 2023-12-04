# STL (Standard Template Library) Cheat Sheet

The Standard Template Library (STL) is a powerful set of C++ template classes to provide general-purpose classes and functions with templates that implement many popular and commonly used algorithms and data structures.

## Containers

### 1. Vector

```cpp
#include <vector>

std::vector<int> myVector = {1, 2, 3, 4, 5};

myVector.push_back(6);   // Add element to the end
myVector.pop_back();     // Remove element from the end
int size = myVector.size(); // Get the size
```

### 2. List

```cpp
#include <list>

std::list<int> myList = {1, 2, 3, 4, 5};

myList.push_back(6);    // Add element to the end
myList.push_front(0);   // Add element to the beginning
myList.pop_back();      // Remove element from the end
```

### 3. Map

```cpp
#include <map>

std::map<std::string, int> myMap;

myMap["one"] = 1;
myMap["two"] = 2;
int value = myMap["two"]; // Access value by key
```

### 4. Set

```cpp
#include <set>

std::set<int> mySet = {1, 2, 3, 4, 5};

mySet.insert(6);  // Add element
mySet.erase(3);   // Remove element
```

### 5. Stack

```cpp
#include <stack>

std::stack<int> myStack;

myStack.push(1);  // Push element onto the stack
myStack.pop();    // Pop element from the stack
int topElement = myStack.top(); // Get the top element
```

### 6. Queue

```cpp
#include <queue>

std::queue<int> myQueue;

myQueue.push(1);  // Enqueue element
myQueue.pop();    // Dequeue element
int frontElement = myQueue.front(); // Get the front element
```

## Algorithms

### 1. Sort

```cpp
#include <algorithm>

std::vector<int> myVector = {5, 2, 8, 1, 7};
std::sort(myVector.begin(), myVector.end());
```

### 2. Find

```cpp
#include <algorithm>

auto it = std::find(myVector.begin(), myVector.end(), 8);

if (it != myVector.end()) {
    // Element found
} else {
    // Element not found
}
```

### 3. Binary Search

```cpp
#include <algorithm>

bool result = std::binary_search(myVector.begin(), myVector.end(), 8);
```

### 4. For Each

```cpp
#include <algorithm>

std::for_each(myVector.begin(), myVector.end(), [](int& element) {
    // Do something with each element
});
```

The STL provides a rich set of containers and algorithms, enabling you to write more efficient and maintainable code. Explore the various containers and algorithms based on your specific programming needs.

Happy coding!
