# Sum of Two Integers in Java

## Objective

This program demonstrates how to declare integer variables, perform arithmetic addition using the `+` operator and display the result using `System.out.println()`.

It is one of the most fundamental programs in Java and helps beginners understand variables, arithmetic operators and output statements.

---

## Program

```java
// SumIntegers program calculating and printing the sum of two integers

// Define a public class named SumIntegers
public class SumIntegers {

    // Main method - JVM starts execution from here
    public static void main(String[] args) {

        // Declare integer variable num1 and assign value 20
        int num1 = 20;

        // Declare integer variable num2 and assign value 30
        int num2 = 30;

        // Calculate the sum of num1 and num2 and store the result in sum
        int sum = num1 + num2;

        // Display the sum with descriptive text
        System.out.println("Sum of Two Integers: " + sum);

    } // End of main method

} // End of SumIntegers class
```

---

## Output

```text
Sum of Two Integers: 50
```

---

## Pseudocode

```text
START

Declare integer variable num1 and assign 20

Declare integer variable num2 and assign 30

Calculate sum = num1 + num2

Display "Sum of Two Integers: " followed by sum

STOP
```

---

## Line-by-Line Explanation

### Line 1

```java
public class SumIntegers
```

Explanation:

* `public` → The class is accessible from anywhere.
* `class` → Keyword used to define a class.
* `SumIntegers` → Name of the class.

---

### Line 2

```java
public static void main(String[] args)
```

Explanation:

* `public` → Accessible from anywhere.
* `static` → JVM can call the method without creating an object.
* `void` → No return value.
* `main` → Entry point of Java application.
* `String[] args` → Stores command line arguments.

---

### Line 3

```java
int num1 = 20;
```

Explanation:

* `int` → Primitive data type used for integer values.
* `num1` → Variable name.
* `20` → Value assigned to variable.

Meaning:

Creates an integer variable named `num1` and stores value `20`.

---

### Line 4

```java
int num2 = 30;
```

Explanation:

Creates another integer variable named `num2` and stores value `30`.

---

### Line 5

```java
int sum = num1 + num2;
```

Explanation:

* `sum` → Variable used to store the result.
* `+` → Arithmetic addition operator.
* `num1 + num2` → Adds both values.

Calculation:

```text
20 + 30 = 50
```

The result is stored in:

```java
sum
```

---

### Line 6

```java
System.out.println("Sum of Two Integers: " + sum);
```

Explanation:

* `System` → Predefined class.
* `out` → Static object of PrintStream class.
* `println()` → Prints output and moves cursor to next line.
* `+` → Concatenates string with variable value.

Output:

```text
Sum of Two Integers: 50
```

---

## Why Do We Use Variables?

Variables are used to:

* Store values in memory.
* Reuse values multiple times.
* Make programs dynamic.
* Improve readability.

Example:

```java
int num1 = 20;
int num2 = 30;
```

Instead of directly writing:

```java
20 + 30
```

we store them in variables and reuse them.

---

## Why Do We Use the + Operator?

The `+` operator performs:

### Arithmetic Addition

Example:

```java
20 + 30
```

Output:

```text
50
```

---

### String Concatenation

Example:

```java
"Sum = " + sum
```

Output:

```text
Sum = 50
```

In Java, if one operand is a String, `+` becomes a concatenation operator.

---

## Special Method Used

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
System.out.println("Hello");
```

Output:

```text
Hello
```

---

## Special Operator Used

### Arithmetic Addition Operator (+)

Purpose:

* Adds two numeric values.

Syntax:

```java
variable = num1 + num2;
```

Example:

```java
int sum = 20 + 30;
```

Output:

```text
50
```

---

## Summary

This program demonstrates:

* Integer variable declaration.
* Variable initialization.
* Arithmetic addition using `+`.
* Storing result in another variable.
* Console output using `System.out.println()`.
* String concatenation.

This is one of the most fundamental Java programs and is widely used for understanding variables and operators in Core Java.
