# No Return Type No Argument Method in Java

## Objective

This program demonstrates a **No Return Type No Argument Method** in Java.

This type of method:

* Does not return any value.
* Does not accept any arguments (parameters).
* Uses `void` as the return type.
* Performs all operations using local variables.

It is the simplest form of a User Defined Method in Java.

---

# Definition

A method with:

* **No Return Type** → Does not send back any value.
* **No Arguments** → Does not receive any input values.

Syntax:

```java
void methodName(){

    // Statements

}
```

---

## Program

```java
/*
 * No Return Type No Argument Method Example
 */

public class Method1 {

    // Main method - JVM starts execution here
    public static void main(String[] args) {

        // Calling the findSum() method
        findSum();

    }

    // Method with no return type and no arguments
    public static void findSum() {

        // Declare first integer variable
        int a = 10;

        // Declare second integer variable
        int b = 20;

        // Calculate sum of two numbers
        int sum = a + b;

        // Display the result
        System.out.println("Sum: " + sum);

    }

}
```

---

## Output

```text
Sum: 30
```

---

## Pseudocode

```text
START

Call findSum()

STOP


findSum()

a = 10

b = 20

sum = a + b

Display sum

END
```

---

# Line-by-Line Explanation

### Line 1

```java
public class Method1
```

Explanation:

* `public` → Class can be accessed from anywhere.
* `class` → Keyword used to create a class.
* `Method1` → Name of the class.

---

### Line 2

```java
public static void main(String[] args)
```

Explanation:

* `public` → Accessible from anywhere.
* `static` → JVM calls it without creating an object.
* `void` → Does not return anything.
* `main` → Entry point of Java application.
* `String[] args` → Stores command line arguments.

---

### Line 3

```java
findSum();
```

Explanation:

This statement calls the method:

```text
findSum()
```

When called:

Control transfers from:

```text
main()

↓

findSum()
```

After execution:

```text
findSum()

↓

main()
```

---

### Line 4

```java
public static void findSum()
```

Explanation:

This method:

* Uses `void` return type.
* Does not accept any parameters.
* Performs addition internally.

---

### Line 5

```java
int a = 10;
```

Creates an integer variable:

```text
a = 10
```

---

### Line 6

```java
int b = 20;
```

Creates another integer variable:

```text
b = 20
```

---

### Line 7

```java
int sum = a + b;
```

Adds:

```text
10 + 20
```

Stores:

```text
sum = 30
```

---

### Line 8

```java
System.out.println("Sum: " + sum);
```

Displays:

```text
Sum: 30
```

on the console.

---

# Why is Return Type void?

The method:

```java
findSum()
```

does not return anything.

Hence:

```java
void
```

is used.

---

# Why are there No Arguments?

Because:

```java
int a = 10;

int b = 20;
```

are declared inside the method itself.

No values are received from outside.

Hence:

```java
findSum()
```

contains:

```text
No Parameters

No Arguments
```

---

# Method Calling Flow

```text
main()

↓

findSum()

↓

Perform Addition

↓

Display Result

↓

Return to main()
```

---

# Advantages of No Return Type No Argument Methods

* Easy to understand.
* Suitable for beginners.
* Improves code modularity.
* Reusable multiple times.
* Useful for displaying information.

---

# Real Life Example

Example:

```text
Display Welcome Message

welcome()

↓

Welcome to Java Programming
```

No input required.

No output returned.

Only displays information.

---

# Important Points

1. Uses:

```java
void
```

2. Does not contain parameters.

3. Does not return any value.

4. Must be called explicitly.

Example:

```java
findSum();
```

---

# Summary

This program demonstrates:

* No Return Type No Argument Method
* Method Declaration
* Method Calling
* Local Variables
* void Return Type
* Execution Flow of Methods
* Console Output using println()

This is the simplest and most fundamental type of User Defined Method in Java and serves as the foundation for understanding all other method types.
