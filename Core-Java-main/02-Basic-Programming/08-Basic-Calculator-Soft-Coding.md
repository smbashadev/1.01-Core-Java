# Basic Calculator Using Soft Coding in Java

## Objective

This program demonstrates how to perform basic arithmetic operations by accepting user input at runtime using the **Scanner** class.

The program displays a menu-driven calculator and performs one of the following operations based on the user's choice:

* Addition
* Subtraction
* Multiplication
* Division

This approach is called **Soft Coding**, where values are provided by the user during program execution.

---

## Program

```java
// Import Scanner class for reading user input
import java.util.Scanner;

// Define a public class named CalculatorSC
public class CalculatorSC {

    // Main method - JVM starts execution from here
    public static void main(String[] args) {

        // Create Scanner object to read input from keyboard
        Scanner sc = new Scanner(System.in);

        // Ask user to enter first integer
        System.out.print("Please enter first integer: ");

        // Read first integer
        int num1 = sc.nextInt();

        System.out.println();

        // Ask user to enter second integer
        System.out.print("Please enter second integer: ");

        // Read second integer
        int num2 = sc.nextInt();

        System.out.println();

        // Display calculator menu
        System.out.println("1. Addition");
        System.out.println("2. Subtraction");
        System.out.println("3. Multiplication");
        System.out.println("4. Division");

        // Variables to store results
        int add;
        int sub;
        int mul;
        int div;

        // Ask user to choose an operation
        System.out.println("Please enter your choice: ");

        // Read user choice
        int choose = sc.nextInt();

        // Perform Addition
        if (choose == 1) {

            add = num1 + num2;

            System.out.println("Addition Result: " + add);

        }

        // Perform Subtraction
        else if (choose == 2) {

            sub = num1 - num2;

            System.out.println("Subtraction Result: " + sub);

        }

        // Perform Multiplication
        else if (choose == 3) {

            mul = num1 * num2;

            System.out.println("Multiplication Result: " + mul);

        }

        // Perform Division
        else if (choose == 4) {

            div = num1 / num2;

            System.out.println("Division Result: " + div);

        }

        // Invalid choice
        else {

            System.out.println("Please choose a valid option.");

        }

        // Close Scanner object
        sc.close();

    }

}
```

---

## Sample Output

```text
Please enter first integer: 10

Please enter second integer: 5

1. Addition
2. Subtraction
3. Multiplication
4. Division

Please enter your choice:
1

Addition Result: 15
```

---

## Pseudocode

```text
START

Import Scanner

Create Scanner object

Read first integer

Read second integer

Display menu:

1. Addition

2. Subtraction

3. Multiplication

4. Division

Read user choice

If choice = 1

    Perform Addition

Else if choice = 2

    Perform Subtraction

Else if choice = 3

    Perform Multiplication

Else if choice = 4

    Perform Division

Else

    Display Invalid Choice Message

Close Scanner

STOP
```

---

## Line-by-Line Explanation

### Import Statement

```java
import java.util.Scanner;
```

Explanation:

* Imports the Scanner class.
* Scanner is used to read user input from keyboard.

---

### Creating Scanner Object

```java
Scanner sc = new Scanner(System.in);
```

Explanation:

* `Scanner` → Predefined class.
* `sc` → Object reference.
* `new` → Creates object.
* `System.in` → Standard input stream (keyboard).

Purpose:

Accept input from the user.

---

### Reading First Integer

```java
int num1 = sc.nextInt();
```

Explanation:

Reads an integer entered by the user.

Example:

```text
10
```

Stores:

```java
num1 = 10;
```

---

### Reading Second Integer

```java
int num2 = sc.nextInt();
```

Stores:

```java
num2 = 5;
```

---

### Displaying Menu

```java
System.out.println("1. Addition");
System.out.println("2. Subtraction");
System.out.println("3. Multiplication");
System.out.println("4. Division");
```

Purpose:

Displays calculator operations to the user.

---

### Reading User Choice

```java
int choose = sc.nextInt();
```

Example:

```text
1
```

Stores:

```java
choose = 1;
```

---

### if Condition

```java
if(choose == 1)
```

Meaning:

If the user chooses option 1, perform addition.

---

### else if Condition

```java
else if(choose == 2)
```

Meaning:

If the first condition fails, check for subtraction.

---

### else Block

```java
else
```

Meaning:

Executes when user enters an invalid option.

---

## Arithmetic Operators Used

| Operator | Meaning        |
| -------- | -------------- |
| +        | Addition       |
| -        | Subtraction    |
| *        | Multiplication |
| /        | Division       |

---

## Special Class Used

### Scanner Class

Package:

```java
java.util.Scanner
```

Purpose:

Used to read user input from keyboard.

---

## Important Scanner Methods

### nextInt()

Syntax:

```java
sc.nextInt();
```

Purpose:

Reads integer value from keyboard.

---

### close()

Syntax:

```java
sc.close();
```

Purpose:

* Closes Scanner object.
* Releases system resources.
* Prevents resource leaks.

---

## Why Soft Coding is Better Than Hard Coding

### Hard Coding

```java
int num1 = 100;
```

* Fixed values.
* Cannot change during execution.

---

### Soft Coding

```java
int num1 = sc.nextInt();
```

* User enters values.
* More flexible.
* Suitable for real-world applications.

---

## Summary

This program demonstrates:

* Scanner class.
* User input using nextInt().
* Menu Driven Program.
* if - else if - else statements.
* Arithmetic operators.
* Addition, Subtraction, Multiplication and Division.
* Soft Coding concept.
* Resource management using close().

This is one of the most important beginner-level Java programs and is frequently asked in Core Java interviews.
