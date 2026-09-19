# Find Output Using String Concatenation and Addition in Java

## Objective

This program demonstrates the difference between:

* String Concatenation using `+`
* Arithmetic Addition using `+`
* Effect of Parentheses `()`
* Left-to-Right Evaluation in Java

This is one of the most frequently asked Java interview questions because many beginners confuse string concatenation with numeric addition.

---

## Program

```java
// FindOutput program showing the difference between
// string concatenation and numeric addition in Java

// Define a public class named FindOutput
public class FindOutput {

    // Main method - JVM starts execution from here
    public static void main(String[] args) {

        // Declare integer variable num1 and assign value 20
        int num1 = 20;

        // Declare integer variable num2 and assign value 30

        int num2 = 30;

        // Add num1 and num2 and store the result in sum
        int sum = num1 + num2;

        // String concatenation occurs from left to right
        System.out.println("Result1: " + num1 + num2);

        // Parentheses force addition first
        System.out.println("Result2: " + (num1 + num2));

        // Print previously calculated sum
        System.out.println("Result3: " + sum);

    } // End of main method

} // End of FindOutput class
```

---

## Output

```text
Result1: 2030

Result2: 50

Result3: 50
```

---

## Pseudocode

```text
START

Declare num1 = 20

Declare num2 = 30

Calculate:

sum = num1 + num2

Display:

"Result1: " + num1 + num2

Display:

"Result2: " + (num1 + num2)

Display:

"Result3: " + sum

STOP
```

---

## Line-by-Line Explanation

### Line 1

```java
public class FindOutput
```

Explanation:

* `public` → Class is accessible from anywhere.
* `class` → Keyword used to define a class.
* `FindOutput` → Name of the class.

---

### Line 2

```java
public static void main(String[] args)
```

Explanation:

* `public` → Accessible from anywhere.
* `static` → JVM can call without object creation.
* `void` → No return value.
* `main` → Entry point of Java application.
* `String[] args` → Stores command line arguments.

---

### Line 3

```java
int num1 = 20;
```

Explanation:

Creates integer variable:

```text
num1 = 20
```

---

### Line 4

```java
int num2 = 30;
```

Explanation:

Creates integer variable:

```text
num2 = 30
```

---

### Line 5

```java
int sum = num1 + num2;
```

Explanation:

Performs arithmetic addition.

Calculation:

```text
20 + 30 = 50
```

Stores:

```text
sum = 50
```

---

## Important Statement 1

```java
System.out.println("Result1: " + num1 + num2);
```

### Step-by-Step Evaluation

Java evaluates expressions from **Left to Right**.

Step 1:

```java
"Result1: " + num1
```

Result:

```text
Result1: 20
```

Step 2:

```java
"Result1: 20" + num2
```

Result:

```text
Result1: 2030
```

Final Output:

```text
Result1: 2030
```

---

### Why Did This Happen?

Because:

```text
If one operand is String,

the + operator performs String Concatenation.
```

---

## Important Statement 2

```java
System.out.println("Result2: " + (num1 + num2));
```

### Step-by-Step Evaluation

Parentheses execute first.

Step 1:

```java
num1 + num2
```

Calculation:

```text
20 + 30 = 50
```

Step 2:

```java
"Result2: " + 50
```

Output:

```text
Result2: 50
```

---

### Why Did This Happen?

Because:

```text
Parentheses have higher precedence.

(num1 + num2)

is evaluated before concatenation.
```

---

## Important Statement 3

```java
System.out.println("Result3: " + sum);
```

Explanation:

The variable:

```java
sum
```

already stores:

```text
50
```

Hence:

```text
Result3: 50
```

---

## String Concatenation in Java

Syntax:

```java
String + Variable
```

Example:

```java
"Java " + "Programming"
```

Output:

```text
Java Programming
```

---

### Another Example

```java
"Age: " + 25
```

Output:

```text
Age: 25
```

---

## Arithmetic Addition in Java

Syntax:

```java
number1 + number2
```

Example:

```java
20 + 30
```

Output:

```text
50
```

---

## Difference Between Concatenation and Addition

| String Concatenation | Arithmetic Addition |
| -------------------- | ------------------- |
| Combines values      | Adds values         |
| Result is String     | Result is Numeric   |
| Uses + with String   | Uses + with numbers |

Example:

```java
"20" + "30"
```

Output:

```text
2030
```

---

Example:

```java
20 + 30
```

Output:

```text
50
```

---

## Why Are Parentheses Important?

Parentheses:

```java
(num1 + num2)
```

force Java to:

1. Perform addition first.
2. Then perform concatenation.

Without parentheses:

```java
"Result: " + num1 + num2
```

Output:

```text
Result: 2030
```

With parentheses:

```java
"Result: " + (num1 + num2)
```

Output:

```text
Result: 50
```

---

## Special Method Used

### println()

Syntax:

```java
System.out.println(data);
```

Purpose:

* Prints output.
* Moves cursor to next line.

---

## Special Operator Used

### + Operator

Purpose:

The `+` operator performs:

1. Arithmetic Addition
2. String Concatenation

Examples:

```java
20 + 30
```

Output:

```text
50
```

---

```java
"20" + "30"
```

Output:

```text
2030
```

---

## Summary

This program demonstrates:

* String Concatenation.
* Arithmetic Addition.
* Left-to-Right evaluation.
* Parentheses precedence.
* * operator behavior.
* Variable usage.
* Console output using println().

This is one of the most important Core Java interview programs because it explains how Java evaluates expressions involving Strings and integers.
