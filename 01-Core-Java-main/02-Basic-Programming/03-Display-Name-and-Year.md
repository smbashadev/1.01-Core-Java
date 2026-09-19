# Display Programming Language Name and Release Year in Java

## Objective

This program demonstrates how to declare variables in Java, assign values to them and display the values using string concatenation with `System.out.println()`.

The program stores a programming language name and its release year in variables and displays them on the console.

---

## Program

```java
// Display program showing a programming language name and release year

// Define a public class named Display
public class Display {

    // Main method - JVM starts execution from here
    public static void main(String[] args) {

        // Declare a String variable name and assign the value "Java"
        String name = "Java";

        // Declare an integer variable year and assign the value 1995
        int year = 1995;

        // Print the programming language name using string concatenation
        System.out.println("Programming Language: " + name);

        // Print the release year using string concatenation
        System.out.println("Year: " + year);

    } // End of main method

} // End of Display class
```

---

## Output

```text
Programming Language: Java
Year: 1995
```

---

## Pseudocode

```text
START

Declare String variable name and assign "Java"

Declare integer variable year and assign 1995

Display "Programming Language: " followed by name

Display "Year: " followed by year

STOP
```

---

## Line-by-Line Explanation

### Line 1

```java
public class Display
```

Explanation:

* `public` → The class is accessible from anywhere.
* `class` → Keyword used to create a class.
* `Display` → Name of the class.

---

### Line 2

```java
public static void main(String[] args)
```

Explanation:

* `public` → Accessible from anywhere.
* `static` → JVM can call this method without creating an object.
* `void` → This method does not return any value.
* `main` → Entry point of Java application.
* `String[] args` → Stores command-line arguments.

---

### Line 3

```java
String name = "Java";
```

Explanation:

* `String` → Non-primitive data type used to store text.
* `name` → Variable name.
* `"Java"` → String literal assigned to the variable.

Meaning:

Stores the programming language name in memory.

---

### Line 4

```java
int year = 1995;
```

Explanation:

* `int` → Primitive data type used to store integer values.
* `year` → Variable name.
* `1995` → Integer value assigned to the variable.

Meaning:

Stores the release year of Java.

---

### Line 5

```java
System.out.println("Programming Language: " + name);
```

Explanation:

* `System` → Predefined class in Java.
* `out` → Static PrintStream object.
* `println()` → Prints output and moves the cursor to the next line.
* `+` → Concatenation operator used to combine text and variable values.

Output:

```text
Programming Language: Java
```

---

### Line 6

```java
System.out.println("Year: " + year);
```

Explanation:

Prints the year value with descriptive text.

Output:

```text
Year: 1995
```

---

## Why Do We Use Variables in Java?

Variables are used to:

* Store values in memory.
* Reuse values multiple times.
* Make programs dynamic.
* Improve readability and maintainability.

Example:

```java
String name = "Java";
int year = 1995;
```

Instead of writing the values repeatedly, they are stored once and reused.

---

## Why Do We Use String Concatenation?

Java uses the `+` operator to combine:

* String + String
* String + Variable
* String + Integer

Example:

```java
"Programming Language: " + name
```

Result:

```text
Programming Language: Java
```

This process is called **String Concatenation**.

---

## Special Methods Used

### println()

Syntax:

```java
System.out.println(data);
```

Purpose:

* Prints output to the console.
* Moves the cursor to the next line automatically.

---

## Special Operator Used

### + Operator

Purpose:

* Performs addition for numeric values.
* Performs concatenation when one operand is a String.

Example:

```java
"Year: " + year
```

Output:

```text
Year: 1995
```

---

## Summary

This program demonstrates:

* Class creation in Java.
* Main method.
* String variable declaration.
* Integer variable declaration.
* String concatenation using `+`.
* Console output using `System.out.println()`.

It is a beginner-friendly program used to understand variables, output statements and concatenation in Core Java.
