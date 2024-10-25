# Internal Details of Hello Java Program

In the previous section, we have created a Java Hello World program and learned how to compile and run a Java program. In this section, we will explore what happens when we compile and run the Java program. We will also address some common questions related to the first Java program.

## What Happens at Compile Time?

- At compile time, the Java file is compiled by the **Java Compiler**.
- The Java Compiler does **not interact with the Operating System**.
- The Java code is converted into **bytecode** during compilation.

### Compilation of a Simple Java Program
The process of compiling the program involves converting the human-readable Java code into bytecode that the Java Virtual Machine (JVM) can execute.

## What Happens at Runtime?

At runtime, the following steps are performed by the Java Runtime Environment (JRE):

1. **Classloader**: 
   - It is a subsystem of the JVM.
   - It is responsible for loading class files into memory.
  
2. **Bytecode Verifier**:
   - It checks the bytecode for any illegal code fragments.
   - This ensures that access rights to objects are not violated.

3. **Interpreter**:
   - It reads the bytecode stream and executes the instructions.

## Common Questions

### Q) Can You Save a Java Source File with a Different Name than the Class Name?

- Yes, you can save a Java source file with a different name, but **only if the class is not public**.
- For example:
  
  - Save the file as `Hard.java`.
  - Compile it with:  
    ```bash
    javac Hard.java
    ```
  - Execute it using the class name:
    ```bash
    java Simple
    ```
- In this case, we compile the code using the file name but run the program using the class name.

### Q) Can You Have Multiple Classes in a Java Source File?

- Yes, a single Java source file can contain multiple classes.
- However, only **one public class** is allowed, and the file name must match that public class.
