# Data Types in Java

Data types specify the different sizes and values that can be stored in a variable. In Java, there are two main categories of data types:

1. **Primitive Data Types**: Include `boolean`, `char`, `byte`, `short`, `int`, `long`, `float`, and `double`.
2. **Non-Primitive Data Types**: Include Classes, Interfaces, and Arrays.

## Java Primitive Data Types

Primitive data types are the building blocks of data manipulation in Java. All variables must be declared before use, as Java is a statically-typed programming language. There are eight primitive data types:

- **boolean**: Represents true or false.
- **byte**: An 8-bit signed integer, range: -128 to 127.
- **char**: A single 16-bit Unicode character.
- **short**: A 16-bit signed integer, range: -32,768 to 32,767.
- **int**: A 32-bit signed integer, range: -2,147,483,648 to 2,147,483,647.
- **long**: A 64-bit signed integer, range: -9,223,372,036,854,775,808 to 9,223,372,036,854,775,807.
- **float**: A single-precision 32-bit IEEE 754 floating-point.
- **double**: A double-precision 64-bit IEEE 754 floating-point.

### Java Primitive Data Type Summary

| Data Type | Default Value | Default Size  |
|-----------|---------------|---------------|
| boolean   | false         | 1 bit         |
| char      | '\u0000'     | 2 bytes       |
| byte      | 0             | 1 byte        |
| short     | 0             | 2 bytes       |
| int       | 0             | 4 bytes       |
| long      | 0L            | 8 bytes       |
| float     | 0.0f          | 4 bytes       |
| double    | 0.0d          | 8 bytes       |

### Data Type Details

- **Boolean**: Represents true or false; used in control flow.
  
  ```java
  boolean a = false;  
  boolean b = true;


# Data Types in Java

Java has two main categories of data types: primitive and non-primitive. Below is a summary of the primitive data types:

## Primitive Data Types

- **Byte**: Represents an 8-bit signed integer; useful for binary data.
  ```java
  byte a = 10, b = -20;
  ```

- **Short**: Represents a 16-bit signed integer; used when conserving memory.
  ```java
  short s = 10000, r = -5000;
  ```

- **Int**: Represents a 32-bit signed integer; commonly used for whole numbers.
  ```java
  int a = 100000, b = -200000;
  ```

- **Long**: Represents a 64-bit signed integer; used for larger values.
  ```java
  long a = 100000L, b = -200000L;
  ```

- **Float**: Represents single-precision 32-bit floating-point numbers.
  ```java
  float f1 = 234.5f;
  ```

- **Double**: Represents double-precision 64-bit floating-point numbers; used for high precision.
  ```java
  double d1 = 12.3;
  ```

- **Char**: Represents a single 16-bit Unicode character; supports internationalization.
  ```java
  char letterA = 'A';
  ```

# Non-Primitive Data Types in Java

Non-primitive data types, or reference data types, are used to store complex objects. They store references to memory locations rather than actual values. Key non-primitive data types include:

- **Class**: Defines the properties and behaviors of objects; e.g., Person.
- **Interface**: Defines a contract for what classes must provide without implementation.
- **Arrays**: Stores multiple values of the same type; fixed size and indexed.
- **Enum**: Defines a set of named constants.

## Importance of Non-Primitive Data Types
Non-primitive data types are essential for creating complex and flexible programs. They enable object-oriented programming and complex data structure representation.

## Why Char Uses 2 Bytes in Java
Java uses the Unicode system, allowing support for a wider range of characters compared to the ASCII code system. The `\u0000 ` represents the lowest range of the Unicode system.
