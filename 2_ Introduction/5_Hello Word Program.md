# First Java Program | Hello World Example

## Software Requirements
- **Install the JDK** if not already installed. Download it from the official website.
- **Set the path** of the `jdk/bin` directory. Refer to this [guide](http://www.javatpoint.com/how-to-set-path-in-java).
- **Create** the Java program.
- **Compile and run** the Java program.

## Creating Hello World Example
In this section, we will learn how to write a simple Java program. After installing the JDK, you can easily create a "Hello Java" program.

### Hello World Program Code
```java
class Simple{  
    public static void main(String args[]){  
        System.out.println("Hello Java");  
    }  
}
```
- Save the file as Simple.java

## Compilation and Execution

### To Compile
```bash
- javac Simple.java
```
### To Execute
```bash
- java Simple
```
### Output
```bash
- Hello Java
```

## Parameters Used in First Java Program

Let’s understand the meaning of the following components in the program:

- **`class`**: 
  - Used to declare a class in Java.

- **`public`**: 
  - An access modifier indicating visibility (visible to all).

- **`static`**: 
  - A keyword indicating that the method can be called without creating an object. 
  - The `main()` method is executed by the JVM without needing an object, saving memory.

- **`void`**: 
  - The return type of the method, indicating it does not return any value.

- **`main`**: 
  - Represents the starting point of the program.

- **`String[] args`**: 
  - Used for command-line arguments.

- **`System.out.println()`**: 
  - A method used to print statements. Here:
    - `System` is a class.
    - `out` is an object of the `PrintStream` class.
    - `println()` is a method of the `PrintStream` class.

## Why Use `String[] args` in Java

- **String Representation:** In Java, all command-line arguments are passed as strings. This is because the JVM treats inputs from the command line as text, regardless of the intended data type.

- **Type Conversion:** If you need to use the command-line arguments as other data types (e.g., integers), you must convert them from strings to the desired type within the program.

- **Compulsory Requirement:** The `String[] args` parameter is a compulsory part of the `main` method signature because the JVM requires this format to start the program.






