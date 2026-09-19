# What is Java?

## Definition

Java is a **high-level, class-based, object-oriented programming language** designed to have as few implementation dependencies as possible.

Java is a general-purpose programming language that follows the principle of **WORA (Write Once, Run Anywhere)**. A Java program compiled on one platform can run on another platform without recompilation.

Java programs are compiled into **Bytecode**, which is executed by the **Java Virtual Machine (JVM)**, making Java platform-independent.

---

## Key Characteristics of Java

* High-Level Programming Language
* Class-Based Language
* Object-Oriented Programming Language
* Platform Independent
* Secure and Robust
* Portable
* Dynamic Runtime Environment
* Supports Write Once Run Anywhere (WORA)

---

## Important Points

1. Java programs are compiled into bytecode.
2. Bytecode runs on JVM irrespective of the operating system.
3. Java syntax is similar to C and C++.
4. Java provides fewer low-level facilities compared to C/C++.
5. Java provides dynamic runtime capabilities.
6. Java is widely used in enterprise and web application development.

---

# History of Java

| Property        | Value                              |
| --------------- | ---------------------------------- |
| Author          | James Gosling                      |
| Vendor          | Sun Microsystems                   |
| Project         | Green Project                      |
| Initial Name    | Oak                                |
| Present Name    | Java                               |
| Objective       | To develop any kind of application |
| Type            | Open Source and Free Software      |
| Slogan          | Write Once Run Anywhere (WORA)     |
| Current Version | JDK 21                             |

---

# Case Sensitivity in Java

Java is a case-sensitive programming language.

This means uppercase and lowercase letters are treated differently.

### Variable Names

```java
int age = 25;
int Age = 30;
int AGE = 35;
```

All three are different variables.

### Class Names

```java
public class HelloWorld {}
public class helloworld {}
```

Both are different classes.

### Main Method

```java
public static void main(String[] args) {}
```

Correct entry point.

```java
public static void Main(String[] args) {}
```

Not recognized as the entry point.

---

## Naming Conventions

### Class Names

Use PascalCase

```java
StudentManagement
EmployeeDetails
```

### Variables and Methods

Use camelCase

```java
studentName
calculateSalary()
```

### Constants

Use UPPER_SNAKE_CASE

```java
MAX_SIZE
PI_VALUE
```

---

# Flow of Java Program

1. Programmer writes source code (`HelloWorld.java`)
2. Java Compiler (`javac`) converts source code into bytecode (`HelloWorld.class`)
3. Bytecode is loaded into JVM.
4. JVM converts bytecode into machine code.
5. Processor executes machine code.
6. Output is displayed.

---

# Portability of Java

A Java program compiled on one platform can run on another platform without recompilation.

This is possible because Java programs execute on JVM.

**WORA = Write Once Run Anywhere**

---

# Platform in Java

A Platform is the environment where programs execute.

Types:

1. Hardware Platform
2. Software Platform

Java is a Software Platform containing:

* JVM
* JRE
* JDK

---

# Architecture of Java

JDK

├── Java Compiler (javac)

└── JRE

  ├── JVM

  │ ├── JIT Compiler

  │ ├── Interpreter

  │ └── Runtime System

  ├── Class Loader

  ├── Byte Code Verifier

  └── Library Files

---

## JDK (Java Development Kit)

JDK is the official software development kit used to develop Java applications.

Contents:

* Java Compiler (javac)
* JRE
* jar tool
* javadoc
* javap
* Debugger

Purpose:

* Write Java programs
* Compile programs
* Debug programs
* Package applications

---

## JRE (Java Runtime Environment)

JRE provides the runtime environment required to execute Java applications.

It contains:

* JVM
* Core Java Libraries

---

## JVM (Java Virtual Machine)

JVM converts bytecode into executable machine code.

Responsibilities:

* Load classes
* Verify bytecode
* Execute bytecode
* Manage memory
* Garbage Collection

---

## Summary

Java is a high-level, object-oriented, platform-independent programming language.

Its major strength is:

**Write Once Run Anywhere (WORA)**

This is achieved through:

* Bytecode
* JVM
* JRE
* JDK

which together make Java portable, secure and platform independent.
