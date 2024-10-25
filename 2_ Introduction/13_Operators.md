# Operators in Java

An operator in Java is a symbol used to perform operations, such as `+`, `-`, `*`, `/`, etc.

## Types of Operators in Java

- **Unary Operator**
- **Arithmetic Operator**
- **Shift Operator**
- **Relational Operator**
- **Bitwise Operator**
- **Logical Operator**
- **Ternary Operator**
- **Assignment Operator**

## Java Operator Precedence

### Operator Type | Category | Precedence
- **Unary**
  - **Postfix**: `expr++`, `expr--`
  - **Prefix**: `++expr`, `--expr`, `+expr`, `-expr`, `~`, `!`
  
- **Arithmetic**
  - **Multiplicative**: `*`, `/`, `%`
  - **Additive**: `+`, `-`
  
- **Shift**
  - **Shift**: `<<`, `>>`, `>>>`
  
- **Relational**
  - **Comparison**: `<`, `>`, `<=`, `>=`, `instanceof`
  - **Equality**: `==`, `!=`
  
- **Bitwise**
  - **AND**: `&`
  - **Exclusive OR**: `^`
  - **Inclusive OR**: `|`
  
- **Logical**
  - **Logical AND**: `&&`
  - **Logical OR**: `||`
  
- **Ternary**
  - **Ternary**: `? :`
  
- **Assignment**
  - **Assignment**: `=`, `+=`, `-=`, `*=`, `/=`, `%=`, `&=`, `^=`, `|=`, `<<=`, `>>=`, `>>>=`

## Java Unary Operator

The Java unary operators require only one operand. Unary operators are used to perform various operations such as:

- Incrementing/decrementing a value by one
- Negating an expression
- Inverting the value of a boolean


## Java Unary Operator Examples

### Java Unary Operator Example 1: `++` and `--`

```java
public class OperatorExample {  
    public static void main(String args[]) {  
        int x = 10;  
        System.out.println(x++);  // 10 (then becomes 11)  
        System.out.println(++x);  // 12  
        System.out.println(x--);  // 12 (then becomes 11)  
        System.out.println(--x);  // 10  
    }  
}
```

### Java Unary Operator Example 2: `++` and `--`

```java
public class OperatorExample {  
    public static void main(String args[]) {  
        int a = 10;  
        int b = 10;  
        System.out.println(a++ + ++a);  // 10 + 12 = 22  
        System.out.println(b++ + b++);  // 10 + 11 = 21  
    }  
}
```
### Java Unary Operator Example: `~` and `!`

```java
public class OperatorExample {  
    public static void main(String args[]) {  
        int a = 10;  
        int b = -10;  
        boolean c = true;  
        boolean d = false;  
        System.out.println(~a);  // -11 (negation of 10)  
        System.out.println(~b);  // 9 (negation of -10)  
        System.out.println(!c);  // false (negation of true)  
        System.out.println(!d);  // true (negation of false)  
    }  
}
```
## Java Arithmetic Operators

Java arithmetic operators are used to perform addition, subtraction, multiplication, and division. They act as basic mathematical operations.

### Java Arithmetic Operator Example

```java
public class OperatorExample {  
    public static void main(String args[]) {  
        int a = 10;  
        int b = 5;  
        System.out.println(a + b);  // 15  
        System.out.println(a - b);  // 5  
        System.out.println(a * b);  // 50  
        System.out.println(a / b);  // 2  
        System.out.println(a % b);  // 0  
    }  
}
```
### Java Arithmetic Operator Example: Expression

```java
public class OperatorExample {  
    public static void main(String args[]) {  
        System.out.println(10 * 10 / 5 + 3 - 1 * 4 / 2);  // 21  
    }  
}
```
## Java Left Shift Operator
The Java left shift operator `<<` is used to shift all of the bits in a value to the left by a specified number of positions.

### Java Left Shift Operator Example
```java
public class OperatorExample {  
    public static void main(String args[]) {  
        System.out.println(10 << 2);  // 10 * 2^2 = 10 * 4 = 40  
        System.out.println(10 << 3);  // 10 * 2^3 = 10 * 8 = 80  
        System.out.println(20 << 2);  // 20 * 2^2 = 20 * 4 = 80  
        System.out.println(15 << 4);  // 15 * 2^4 = 15 * 16 = 240  
    }  
}
```
## Java Right Shift Operator
The Java right shift operator `>>` is used to move the value of the left operand to the right by the number of bits specified by the right operand.

### Java Right Shift Operator Example
```java
public class OperatorExample {  
    public static void main(String args[]) {  
        System.out.println(10 >> 2);  // 10 / 2^2 = 10 / 4 = 2  
        System.out.println(20 >> 2);  // 20 / 2^2 = 20 / 4 = 5  
        System.out.println(20 >> 3);  // 20 / 2^3 = 20 / 8 = 2  
    }  
}
```
## Java Shift Operator Example: `>>` vs `>>>`
The `>>` operator preserves the sign bit when shifting, while the `>>>` operator shifts the bits and fills the leftmost bits with zeros, affecting negative numbers differently.

### Example:
```java
public class OperatorExample {  
    public static void main(String args[]) {  
        // For positive numbers, `>>` and `>>>` work the same  
        System.out.println(20 >> 2);   // 5  
        System.out.println(20 >>> 2);  // 5  
        // For negative numbers, `>>>` changes the most significant bit (MSB) to 0  
        System.out.println(-20 >> 2);   // -5  
        System.out.println(-20 >>> 2);  // 1073741819  
    }  
}
```
## Java AND Operator Example: Logical `&&` and Bitwise `&`
The logical `&&` operator doesn't check the second condition if the first condition is false. It checks the second condition only if the first one is true.

The bitwise `&` operator always checks both conditions whether the first condition is true or false.

### Example:
```java
public class OperatorExample {  
    public static void main(String args[]) {  
        int a = 10;  
        int b = 5;  
        int c = 20;  
        System.out.println(a < b && a < c);  // false && true = false  
        System.out.println(a < b & a < c);    // false & true = false  
    }  
}
```
## Java AND Operator Example: Logical `&&` vs Bitwise `&`
The logical `&&` operator doesn't evaluate the second condition if the first condition is false, whereas the bitwise `&` operator evaluates both conditions regardless.

### Example:
```java
public class OperatorExample {  
    public static void main(String args[]) {  
        int a = 10;  
        int b = 5;  
        int c = 20;  
        System.out.println(a < b && a++ < c); // false && true = false  
        System.out.println(a);                  // 10 because the second condition is not checked  
        System.out.println(a < b & a++ < c);   // false & true = false  
        System.out.println(a);                  // 11 because the second condition is checked  
    }  
}
```
## Java OR Operator Example: Logical `||` and Bitwise `|`
The logical `||` operator doesn't evaluate the second condition if the first condition is true. It checks the second condition only if the first one is false.

The bitwise `|` operator always checks both conditions regardless of the outcome of the first condition.

### Example:
```java
public class OperatorExample {  
    public static void main(String args[]) {  
        int a = 10;  
        int b = 5;  
        int c = 20;  
        System.out.println(a > b || a < c);   // true || true = true  
        System.out.println(a > b | a < c);     // true | true = true  
        // || vs |  
        System.out.println(a > b || a++ < c);  // true || true = true  
        System.out.println(a);                   // 10 because the second condition is not checked  
        System.out.println(a > b | a++ < c);    // true | true = true  
        System.out.println(a);                   // 11 because the second condition is checked  
    }  
}
```
## Java Ternary Operator
The Java Ternary operator is used as a one-line replacement for the `if-then-else` statement and is widely used in Java programming. It is the only conditional operator that takes three operands.

### Java Ternary Operator Example
```java
public class OperatorExample {  
    public static void main(String args[]) {  
        int a = 2;  
        int b = 5;  
        int min = (a < b) ? a : b;  
        System.out.println(min);  // Output: 2  
    }  
}
```
### Another Example:
```java
public class OperatorExample {  
    public static void main(String args[]) {  
        int a = 10;  
        int b = 5;  
        int min = (a < b) ? a : b;  
        System.out.println(min);  // Output: 5  
    }  
}
```
## Java Assignment Operator
The Java assignment operator is one of the most common operators. It is used to assign the value on its right to the operand on its left.

### Java Assignment Operator Example
```java
public class OperatorExample {  
    public static void main(String args[]) {  
        int a = 10;  
        int b = 20;  
        a += 4; // a = a + 4 (a = 10 + 4)  
        b -= 4; // b = b - 4 (b = 20 - 4)  
        System.out.println(a);  
        System.out.println(b);  
    }  
}
```
## Java Assignment Operator Example
```java
public class OperatorExample {  
    public static void main(String[] args) {  
        int a = 10;  
        a += 3; // 10 + 3  
        System.out.println(a);  
        a -= 4; // 13 - 4  
        System.out.println(a);  
        a *= 2; // 9 * 2  
        System.out.println(a);  
        a /= 2; // 18 / 2  
        System.out.println(a);  
    }  
}
```
## Java Assignment Operator Example: Adding short
```java
public class OperatorExample {  
    public static void main(String args[]) {  
        short a = 10;  
        short b = 10;  
        // a += b; // a = a + b internally so fine  
        a = a + b; // Compile time error because 10 + 10 = 20 now int  
        System.out.println(a);  
    }  
}
```
### After type cast:
```java
public class OperatorExample {  
    public static void main(String args[]) {  
        short a = 10;  
        short b = 10;  
        a = (short)(a + b); // 20 which is int now converted to short  
        System.out.println(a);  
    }  
}
```
