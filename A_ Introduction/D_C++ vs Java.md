# C++ vs Java

## Key Differences

- **Platform Dependency**
  - **C++**: Platform-dependent, compiled directly to machine code.
  - **Java**: Platform-independent, compiled to bytecode and run on the Java Virtual Machine (JVM).

- **Usage**
  - **C++**: Primarily used for system programming.
  - **Java**: Widely used for application programming, including web, enterprise, and mobile applications.

- **Memory Management**
  - **C++**: Manual memory management with support for pointers.
  - **Java**: Automatic garbage collection, no direct pointer access.

- **Inheritance**
  - **C++**: Supports multiple inheritance and structures.
  - **Java**: No multiple inheritance through classes, only via interfaces.

- **Execution Model**
  - **C++**: Uses only a compiler.
  - **Java**: Uses both a compiler and an interpreter.

- **Concurrency**
  - **C++**: Lacks built-in thread support.
  - **Java**: Built-in support for multithreading.

- **Documentation**
  - **C++**: No support for documentation comments.
  - **Java**: Supports documentation comments (/** ... */).

- **Object Orientation**
  - **C++**: Object-oriented but not all types are objects.
  - **Java**: Everything (except primitive types) is an object, forming a single inheritance hierarchy.

## Note
- Java does not support default arguments or header files; it uses the `import` statement instead.

## Example Programs

### C++ Example
```cpp
#include <iostream>
using namespace std;
int main() {
   cout << "Hello C++ Programming";  
   return 0;  
}
```
- Output: Hello C++ Programming
  
### Java Example
```java
class Simple {  
    public static void main(String args[]) {  
     System.out.println("Hello Java");  
    }  
}
```
- Output: Hello Java