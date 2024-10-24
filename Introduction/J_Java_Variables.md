# Java Variables

A variable is a **container** that holds a value during the execution of a Java program. It is assigned with a data type and refers to a **memory location**. There are two types of data types in Java: **primitive** and **non-primitive**.

## Types of Variables
Java has three types of variables:

1. **Local Variable**
   - Declared inside a method body.
   - Only accessible within that method.
   - Cannot be declared with the `static` keyword.

2. **Instance Variable**
   - Declared inside a class but outside the method body.
   - Its value is specific to an instance of the class (not shared across instances).
   - Cannot be declared as `static`.

3. **Static Variable**
   - Declared with the `static` keyword.
   - A single copy is shared among all instances of the class.
   - Memory allocation happens once when the class is loaded.

### Example of Variable Types:
```java
public class A {
    static int m = 100; // static variable
    void method() {
        int n = 90; // local variable
    }
    public static void main(String[] args) {
        int data = 50; // instance variable
    }
}
```
## 1. Add Two Numbers
```java
public class Simple {
    public static void main(String[] args) {
        int a = 10;
        int b = 10;
        int c = a + b;
        System.out.println(c); // Output: 20
    }
}
```

## 2. Widening Example

```java
public class Simple {
    public static void main(String[] args) {
        int a = 10;
        float f = a;
        System.out.println(a); // Output: 10
        System.out.println(f); // Output: 10.0
    }
}
```

### 3. Narrowing (Typecasting)
```java
public class Simple {
    public static void main(String[] args) {
        float f = 10.5f;
        int a = (int) f;
        System.out.println(f); // Output: 10.5
        System.out.println(a); // Output: 10
    }
}
```
### 4. Overflow Example
```java
class Simple {
    public static void main(String[] args) {
        int a = 130;
        byte b = (byte) a;
        System.out.println(a); // Output: 130
        System.out.println(b); // Output: -126
    }
}
```
### 5. Adding Lower Type
```java
class Simple {
    public static void main(String[] args) {
        byte a = 10;
        byte b = 10;
        byte c = (byte) (a + b);
        System.out.println(c); // Output: 20
    }
}
```
