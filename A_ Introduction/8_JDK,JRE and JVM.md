# Difference Between JDK, JRE, and JVM

Understanding the distinctions between JDK, JRE, and JVM is essential before delving deeper into Java.

## JVM (Java Virtual Machine)

- **Abstract machine** that provides a runtime environment to execute Java bytecode.
- JVM is **platform dependent** but Java is platform-independent.
- Notions of JVM:
  - **Specification**: Defines what the JVM should do.
  - **Implementation**: Actual realization of the JVM.
  - **Instance**: Running JVM instance.
- JVM can run programs written in other languages that compile to Java bytecode.
- **Main tasks**:
  - Loads code
  - Verifies code
  - Executes code
  - Provides a runtime environment

## JRE (Java Runtime Environment)

- **JRE** is a set of software tools used for developing and running Java applications.
- It provides the **runtime environment** and is the **implementation of JVM**.
- Contains **libraries** and other files required by the JVM at runtime.
- **Physically exists**, unlike the JVM.
- Other companies besides Sun Microsystems also release JRE implementations.

## JDK (Java Development Kit)

- **JDK** is a software development environment used to develop Java applications.
- It includes the **JRE + development tools**.
- Contains resources like:
  - Private JVM
  - Compiler (`javac`)
  - Interpreter/loader (`java`)
  - Archiver (`jar`)
  - Documentation generator (`Javadoc`)
- **Platforms supported** by JDK:
  - Standard Edition (SE)
  - Enterprise Edition (EE)
  - Micro Edition (ME)

