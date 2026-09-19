# Hello World Program in Java

## Objective

The Hello World program is the first and most fundamental Java program. It demonstrates the basic structure of a Java application and explains how to display output on the console using `System.out.println()`.

---

## Program

```java
// Hello World Program in Java

// Define a public class named HelloWorld
public class HelloWorld {

    // Main method - JVM starts program execution from here
    public static void main(String[] args) {

        // Print the text "Hello World!" followed by a new line
        System.out.println("Hello World!");

    } // End of main method

} // End of HelloWorld class
```

---

## Output

```text
Hello World!
```

---

## Pseudocode

```text
START

Create a class named HelloWorld

Define the main method

Display "Hello World!" on the console

STOP
```

---

## Line-by-Line Explanation

### Line 1

```java
public class HelloWorld
```

Explanation:

* `public` → The class can be accessed from anywhere.
* `class` → Keyword used to create a class.
* `HelloWorld` → Name of the class.

---

### Line 2

```java
public static void main(String[] args)
```

Explanation:

* `public` → Accessible from anywhere.
* `static` → JVM can call the method without creating an object.
* `void` → Method does not return any value.
* `main` → Entry point of every Java application.
* `String[] args` → Stores command-line arguments.

---

### Line 3

```java
System.out.println("Hello World!");
```

Explanation:

* `System` → Predefined class in the `java.lang` package.
* `out` → Static object of `PrintStream`.
* `println()` → Prints output and moves the cursor to the next line.
* `"Hello World!"` → String literal to be displayed.

---

## Why Do We Use main() in Java?

Java programs begin execution from:

```java
public static void main(String[] args)
```

Reason:

* JVM searches for the `main()` method.
* Without the `main()` method, JVM cannot start execution.
* It acts as the entry point of a Java application.

---

## Special Method Used

### println()

**Syntax**

```java
System.out.println(data);
```

**Purpose**

* Displays output on the console.
* Automatically moves the cursor to the next line after printing.

**Belongs To**

```text
PrintStream Class
```

---

## Why Do We Use System.out.println()?

* `System` provides access to system resources.
* `out` represents the standard output stream.
* `println()` prints the message and appends a newline character.

It is the most commonly used output statement in Java.

---

## Summary

The Hello World program demonstrates:

* Basic structure of a Java program.
* Class declaration.
* Main method.
* Console output using `System.out.println()`.
* Entry point of Java execution.

It is the first program every Java developer learns and serves as the foundation for understanding Core Java.
