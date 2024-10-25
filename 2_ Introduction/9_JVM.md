# JVM (Java Virtual Machine) Architecture

## Overview
JVM is an **abstract machine** that provides a runtime environment to execute Java bytecode. JVM is **platform dependent**, and its implementation is known as **JRE (Java Runtime Environment)**. Every time a Java program runs, a **JVM instance** is created.

### Key Operations of JVM:
- Loads code
- Verifies code
- Executes code
- Provides runtime environment

### JVM Provides:
- Memory area
- Class file format
- Register set
- Garbage-collected heap
- Fatal error reporting

## Components of JVM Architecture

### 1. Classloader
- **Loads class files** into memory when a Java program runs.
- **Types of Classloaders**:
  - **Bootstrap ClassLoader**: Loads core Java libraries from `rt.jar`.
  - **Extension ClassLoader**: Loads JAR files from `$JAVA_HOME/jre/lib/ext`.
  - **System/Application ClassLoader**: Loads class files from the classpath (default: current directory).

Example to print classloader names:
```java
public class ClassLoaderExample {
    public static void main(String[] args) {
        Class c = ClassLoaderExample.class;
        System.out.println(c.getClassLoader());
        System.out.println(String.class.getClassLoader()); // prints null
    }
}

```

### 2. Class (Method) Area
- Stores per-class structures such as:
  - **Runtime constant pool**
  - **Field and method data**
  - **Method code**

### 3. Heap
- Runtime data area where objects are **allocated**.

### 4. Stack
- **Java Stack** stores:
  - Frames
  - Local variables
  - Partial results
  - Manages **method invocation** and return.
- Each thread has a **private JVM stack**.

### 5. Program Counter (PC) Register
- Contains the **address** of the currently executing JVM instruction.

### 6. Native Method Stack
- Stores all the **native methods** used by the application.

### 7. Execution Engine
- Contains:
  - **Virtual processor**
  - **Interpreter**: Reads bytecode and executes instructions.
  - **Just-In-Time (JIT) Compiler**: Compiles frequently used bytecode to improve performance.

### 8. Java Native Interface (JNI)
- A framework to **interact with native applications** (e.g., C, C++).
- Java uses JNI to:
  - Send output to the **console**
  - Interact with **OS libraries**
