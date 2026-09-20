# Square of an Integer Using Soft Coding in Java

## Objective

This program demonstrates how to calculate the square of an integer by accepting input from the user at runtime using the `Scanner` class.

This approach is called **Soft Coding**, where values are not fixed in the program but are provided by the user during execution.

---

## Program

```java
// Import Scanner class from java.util package
import java.util.Scanner;

// Define a public class named SquareOfIntegerSC
public class SquareOfIntegerSC {

    // Main method - JVM starts execution from here
    public static void main(String[] args) {

        // Create Scanner object to read input from keyboard
        Scanner sc = new Scanner(System.in);

        // Ask the user to enter a number
        System.out.println("Please enter a Number");

        // Read integer value entered by the user
        int num = sc.nextInt();

        // Calculate square by multiplying number by itself
        int sq = num * num;

        // Display the square of the number
        System.out.println("Square of Integer: " + sq);

        // Close Scanner object and release resources
        sc.close();

    } // End of main method

} // End of SquareOfIntegerSC class
```

---

## Output

```text
Please enter a Number
8
Square of Integer: 64
```

---

## Pseudocode

```text
START

Import Scanner class

Create Scanner object

Display message:
"Please enter a Number"

Read integer value from user

Calculate:
square = number × number

Display square

Close Scanner

STOP
```

---

## Line-by-Line Explanation

### Line 1

```java
import java.util.Scanner;
```

Explanation:

* `import` → Used to include predefined classes.
* `java.util` → Package that contains utility classes.
* `Scanner` → Class used to accept input from the user.

Purpose:

Allows the program to read keyboard input.

---

### Line 2

```java
public class SquareOfIntegerSC
```

Explanation:

* `public` → Accessible from anywhere.
* `class` → Keyword used to create a class.
* `SquareOfIntegerSC` → Name of the class.

---

### Line 3

```java
public static void main(String[] args)
```

Explanation:

* `public` → Accessible from anywhere.
* `static` → JVM can invoke without creating an object.
* `void` → No return value.
* `main` → Entry point of Java program.
* `String[] args` → Stores command-line arguments.

---

### Line 4

```java
Scanner sc = new Scanner(System.in);
```

Explanation:

* `Scanner` → Class used for input operations.
* `sc` → Object reference.
* `new` → Creates object.
* `System.in` → Standard input stream (keyboard).

Purpose:

Creates an object that reads user input.

---

### Line 5

```java
System.out.println("Please enter a Number");
```

Explanation:

Displays a message asking the user to enter a number.

Output:

```text
Please enter a Number
```

---

### Line 6

```java
int num = sc.nextInt();
```

Explanation:

* `int` → Integer variable.
* `num` → Variable name.
* `sc.nextInt()` → Reads integer input from keyboard.

Example:

Input:

```text
8
```

Stored in:

```java
num = 8;
```

---

### Line 7

```java
int sq = num * num;
```

Explanation:

Calculates square using multiplication operator.

Calculation:

```text
8 × 8 = 64
```

Stores result in:

```java
sq
```

---

### Line 8

```java
System.out.println("Square of Integer: " + sq);
```

Explanation:

Displays the square value using string concatenation.

Output:

```text
Square of Integer: 64
```

---

### Line 9

```java
sc.close();
```

Explanation:

Closes Scanner object.

Purpose:

* Releases system resources.
* Prevents memory leaks.
* Considered a good programming practice.

---

## Special Class Used

### Scanner Class

Package:

```java
java.util.Scanner
```

Purpose:

Used to accept user input during runtime.

Example:

```java
Scanner sc = new Scanner(System.in);
```

---

## Important Scanner Methods

### nextInt()

Syntax:

```java
sc.nextInt();
```

Purpose:

Reads integer input from keyboard.

Example:

Input:

```text
25
```

Output:

```java
int num = 25;
```

---

### close()

Syntax:

```java
sc.close();
```

Purpose:

Closes Scanner object and releases resources.

---

## Why Do We Use Soft Coding?

In soft coding:

* Values are entered by the user.
* No need to modify source code.
* Program becomes reusable.
* More flexible and interactive.

Example:

```java
int num = sc.nextInt();
```

The value changes every time the user runs the program.

---

## Difference Between Hard Coding and Soft Coding

| Hard Coding                 | Soft Coding                          |
| --------------------------- | ------------------------------------ |
| Values are fixed in code    | Values are entered by user           |
| Less flexible               | More flexible                        |
| Requires code changes       | No code changes required             |
| Suitable for small examples | Suitable for real-world applications |
| Difficult to maintain       | Easy to maintain                     |

### Hard Coding Example

```java
int num = 8;
```

---

### Soft Coding Example

```java
int num = sc.nextInt();
```

---

## Why Do We Use Scanner in Java?

Scanner is used because:

* Accepts user input at runtime.
* Supports different data types.
* Easy to use.
* Suitable for console applications.

---

## Summary

This program demonstrates:

* Soft Coding in Java.
* Scanner class.
* User input using nextInt().
* Multiplication operator.
* Square calculation.
* String concatenation.
* Resource management using close().
* Difference between Hard Coding and Soft Coding.

This is one of the most important beginner-level programs and is frequently asked in Java interviews.
