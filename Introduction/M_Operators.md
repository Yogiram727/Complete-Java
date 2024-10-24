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

