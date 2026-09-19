# Basic Calculator Using Hard Coding in Java

## Objective

This program demonstrates how to perform basic arithmetic operations in Java using hard coded values.

The program performs:

* Addition (+)
* Subtraction (-)
* Multiplication (*)
* Division (/)

and displays the results on the console.

---

## Program

```java
// CalculatorHC program performing basic arithmetic operations using hard coded values

// Define a public class named CalculatorHC
public class CalculatorHC {

    // Main method - JVM starts execution from here
    public static void main(String[] args) {

        // Calculator program using hard coded values

        // Declare integer variable num1 and assign value 100
        int num1 = 100;

        // Declare integer variable num2 and assign value 50
        int num2 = 50;

        // Perform addition and store result in add
        int add = num1 + num2;

        // Perform subtraction and store result in sub
        int sub = num1 - num2;

        // Perform multiplication and store result in mul
        int mul = num1 * num2;

        // Perform division and store result in div
        int div = num1 / num2;

        // Display addition result
        System.out.println("Addition Result: " + add);

        // Display subtraction result
        System.out.println("Subtraction Result: " + sub);

        // Display multiplication result
        System.out.println("Multiplication Result: " + mul);

        // Display division result
        System.out.println("Division Result: " + div);

    } // End of main method

} // End of CalculatorHC class
```

---

## Output

```text
Addition Result: 150
Subtraction Result: 50
Multiplication Result: 5000
Division Result: 2
```

---

## Pseudocode

```text
START

Declare num1 = 100

Declare num2 = 50

Calculate:

add = num1 + num2

sub = num1 - num2

mul = num1 * num2

div = num1 / num2

Display Addition Result

Display Subtraction Result

Display Multiplication Result

Display Division Result

STOP
```

---

## Line-by-Line Explanation

### Line 1

```java
public class CalculatorHC
```

Explanation:

* `public` → The class is accessible from anywhere.
* `class` → Keyword used to define a class.
* `CalculatorHC` → Name of the class.

**HC stands for Hard Coding.**

---

### Line 2

```java
public static void main(String[] args)
```

Explanation:

* `public` → Accessible from anywhere.
* `static` → JVM calls this method without creating an object.
* `void` → Does not return any value.
* `main` → Entry point of Java application.
* `String[] args` → Stores command line arguments.

---

### Line 3

```java
int num1 = 100;
```

Explanation:

* `int` → Primitive integer data type.
* `num1` → Variable name.
* `100` → Assigned integer value.

---

### Line 4

```java
int num2 = 50;
```

Explanation:

Creates another integer variable and stores value `50`.

---

### Line 5

```java
int add = num1 + num2;
```

Explanation:

Performs addition.

Calculation:

```text
100 + 50 = 150
```

Stores result in:

```java
add
```

---

### Line 6

```java
int sub = num1 - num2;
```

Explanation:

Performs subtraction.

Calculation:

```text
100 - 50 = 50
```

Stores result in:

```java
sub
```

---

### Line 7

```java
int mul = num1 * num2;
```

Explanation:

Performs multiplication.

Calculation:

```text
100 × 50 = 5000
```

Stores result in:

```java
mul
```

---

### Line 8

```java
int div = num1 / num2;
```

Explanation:

Performs division.

Calculation:

```text
100 / 50 = 2
```

Stores result in:

```java
div
```

---

### Output Statements

```java
System.out.println("Addition Result: " + add);
```

Prints:

```text
Addition Result: 150
```

---

```java
System.out.println("Subtraction Result: " + sub);
```

Prints:

```text
Subtraction Result: 50
```

---

```java
System.out.println("Multiplication Result: " + mul);
```

Prints:

```text
Multiplication Result: 5000
```

---

```java
System.out.println("Division Result: " + div);
```

Prints:

```text
Division Result: 2
```

---

## Arithmetic Operators Used

| Operator | Meaning        | Example  |
| -------- | -------------- | -------- |
| `+`      | Addition       | 100 + 50 |
| `-`      | Subtraction    | 100 - 50 |
| `*`      | Multiplication | 100 * 50 |
| `/`      | Division       | 100 / 50 |

---

## Why Do We Use Hard Coding?

Hard Coding means:

Values are written directly inside the source code.

Example:

```java
int num1 = 100;
int num2 = 50;
```

Advantages:

* Easy to understand.
* Suitable for beginners.
* Quick for small programs.

Disadvantages:

* Values cannot be changed during execution.
* Requires editing code and recompiling.
* Not suitable for real-world applications.

---

## Hard Coding vs Soft Coding

| Hard Coding                | Soft Coding                     |
| -------------------------- | ------------------------------- |
| Values are fixed           | Values are entered by user      |
| Less flexible              | More flexible                   |
| Code modification required | No modification required        |
| Used for simple examples   | Used in real-world applications |

Hard Coding Example:

```java
int num1 = 100;
```

Soft Coding Example:

```java
int num1 = sc.nextInt();
```

---

## Special Method Used

### println()

Syntax:

```java
System.out.println(data);
```

Purpose:

* Prints output on console.
* Moves cursor to next line automatically.

---

## Summary

This program demonstrates:

* Integer variable declaration.
* Arithmetic operators.
* Addition, subtraction, multiplication and division.
* Hard Coding concept.
* String concatenation.
* Output using `System.out.println()`.

This is one of the most important beginner-level Java programs for understanding arithmetic operations and hard coded values.
