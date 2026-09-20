# Square of an Integer in Java

## Objective

This program demonstrates how to calculate the square of an integer using the multiplication operator (`*`) in Java.

The program declares an integer variable, multiplies it by itself and stores the result in another variable before displaying the output.

---

## Program

```java
// SquareOfInteger program calculating the square of an integer

// Define a public class named SquareOfInteger
public class SquareOfInteger {

    // Main method - JVM starts execution from here
    public static void main(String[] args) {

        // Declare an integer variable num and assign the value 8
        int num = 8;

        // Multiply num by itself and store the result in sq
        int sq = num * num;

        // Display the square value with descriptive text
        System.out.println("Square of Integer: " + sq);

    } // End of main method

} // End of SquareOfInteger class
```

---

## Output

```text
Square of Integer: 64
```

---

## Pseudocode

```text
START

Declare integer variable num and assign 8

Calculate sq = num × num

Display "Square of Integer: " followed by sq

STOP
```

---

## Line-by-Line Explanation

### Line 1

```java
public class SquareOfInteger
```

Explanation:

* `public` → The class is accessible from anywhere.
* `class` → Keyword used to create a class.
* `SquareOfInteger` → Name of the class.

---

### Line 2

```java
public static void main(String[] args)
```

Explanation:

* `public` → Accessible from anywhere.
* `static` → JVM can call the method without creating an object.
* `void` → The method does not return any value.
* `main` → Entry point of Java application.
* `String[] args` → Stores command-line arguments.

---

### Line 3

```java
int num = 8;
```

Explanation:

* `int` → Primitive data type used to store integer values.
* `num` → Variable name.
* `8` → Integer value assigned to the variable.

Meaning:

Stores the number whose square is to be calculated.

---

### Line 4

```java
int sq = num * num;
```

Explanation:

* `sq` → Variable used to store square value.
* `*` → Multiplication operator.
* `num * num` → Multiplies the number by itself.

Calculation:

```text
8 × 8 = 64
```

The result is stored in:

```java
sq
```

---

### Line 5

```java
System.out.println("Square of Integer: " + sq);
```

Explanation:

* `System` → Predefined class in Java.
* `out` → Static object of PrintStream class.
* `println()` → Prints output and moves cursor to next line.
* `+` → Concatenation operator used to combine text and variable value.

Output:

```text
Square of Integer: 64
```

---

## Why Do We Use Variables?

Variables help to:

* Store values in memory.
* Reuse values throughout the program.
* Improve readability.
* Make programs easier to maintain.

Example:

```java
int num = 8;
int sq = num * num;
```

---

## Why Do We Use the Multiplication Operator (*)?

The multiplication operator is used to multiply two values.

Syntax:

```java
value1 * value2
```

Example:

```java
8 * 8
```

Output:

```text
64
```

In this program:

```java
num * num
```

calculates the square of the number.

---

## Why Do We Store the Result in Another Variable?

```java
int sq = num * num;
```

Advantages:

* Result can be reused.
* Improves code readability.
* Avoids recalculating the expression multiple times.

---

## Special Methods Used

### println()

Syntax:

```java
System.out.println(data);
```

Purpose:

* Displays output on the console.
* Automatically moves the cursor to the next line.

Example:

```java
System.out.println("Java");
```

Output:

```text
Java
```

---

## Special Operators Used

### Multiplication Operator (*)

Purpose:

* Multiplies two numeric values.

Example:

```java
8 * 8
```

Output:

```text
64
```

---

### Concatenation Operator (+)

Purpose:

Combines String and variable values.

Example:

```java
"Square of Integer: " + sq
```

Output:

```text
Square of Integer: 64
```

---

## Summary

This program demonstrates:

* Integer variable declaration.
* Variable initialization.
* Multiplication operator (`*`).
* Calculating square of a number.
* Storing results in another variable.
* String concatenation.
* Displaying output using `System.out.println()`.

This is one of the most fundamental arithmetic programs in Java and is frequently asked in beginner-level programming interviews.
