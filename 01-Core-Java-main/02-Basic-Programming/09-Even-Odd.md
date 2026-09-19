# Even Odd Program in Java

## Objective

This program demonstrates how to determine whether a number is **Even** or **Odd** using:

* Scanner class for user input
* Modulus (%) operator
* if-else conditional statement

The program accepts an integer from the user and checks whether it is divisible by 2.

---

## Program

```java
// Import Scanner class for user input
import java.util.Scanner;

// Define a public class named EvenOdd
public class EvenOdd {

    // Main method - JVM starts execution from here
    public static void main(String[] args) {

        // Create Scanner object to read input from keyboard
        Scanner sc = new Scanner(System.in);

        // Ask the user to enter a number
        System.out.println("Please enter a number: ");

        // Read integer value entered by the user
        int num = sc.nextInt();

        // Check whether the number is divisible by 2
        if (num % 2 == 0) {

            // Executes when remainder is zero
            System.out.println("Given number is an Even Number");

        }
        else {

            // Executes when remainder is not zero
            System.out.println("Given number is an Odd Number");

        }

        // Close Scanner object
        sc.close();

    } // End of main method

} // End of EvenOdd class
```

---

## Output 1

```text
Please enter a number:
5

Given number is an Odd Number
```

---

## Output 2

```text
Please enter a number:
4

Given number is an Even Number
```

---

## Pseudocode

```text
START

Import Scanner

Create Scanner object

Display:
"Please enter a number"

Read integer value

If number % 2 == 0

    Display:
    "Given number is an Even Number"

Else

    Display:
    "Given number is an Odd Number"

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

* Imports Scanner class.
* Scanner is used to read input from keyboard.

Package:

```java
java.util
```

---

### Creating Scanner Object

```java
Scanner sc = new Scanner(System.in);
```

Explanation:

* `Scanner` → Predefined class.
* `sc` → Object reference.
* `new` → Creates object.
* `System.in` → Standard input stream.

Purpose:

Reads user input from keyboard.

---

### Reading User Input

```java
int num = sc.nextInt();
```

Explanation:

* `int` → Integer variable.
* `num` → Variable name.
* `nextInt()` → Reads integer input.

Example:

Input:

```text
5
```

Stored as:

```java
num = 5;
```

---

## if Condition

```java
if(num % 2 == 0)
```

Explanation:

The condition checks:

```text
Remainder after dividing the number by 2
```

If remainder equals:

```text
0
```

Then:

```text
The number is Even
```

---

### Example 1

```text
4 % 2 = 0
```

Result:

```text
Even Number
```

---

### Example 2

```text
5 % 2 = 1
```

Result:

```text
Odd Number
```

---

## else Block

```java
else
```

Explanation:

This block executes when:

```java
num % 2 != 0
```

Meaning:

The number is not divisible by 2.

Hence:

```text
Odd Number
```

---

## Modulus Operator (%)

### Syntax

```java
a % b
```

Purpose:

Returns the remainder after division.

---

### Examples

```java
10 % 2
```

Output:

```text
0
```

---

```java
7 % 2
```

Output:

```text
1
```

---

```java
15 % 4
```

Output:

```text
3
```

---

## Why Do We Use Modulus Operator for Even Odd?

A number is:

### Even

If:

```text
number % 2 = 0
```

Examples:

```text
2
4
6
8
10
```

---

### Odd

If:

```text
number % 2 ≠ 0
```

Examples:

```text
1
3
5
7
9
```

---

## Special Class Used

### Scanner Class

Package:

```java
java.util.Scanner
```

Purpose:

Accept user input from keyboard.

---

## Important Scanner Methods

### nextInt()

Syntax:

```java
sc.nextInt();
```

Purpose:

Reads integer input.

---

### close()

Syntax:

```java
sc.close();
```

Purpose:

* Releases resources.
* Closes Scanner object.
* Prevents resource leakage.

---

## Why Do We Use if-else?

The if-else statement is used for:

* Decision Making
* Executing different code blocks based on conditions.

Syntax:

```java
if(condition){

    // True block

}
else{

    // False block

}
```

---

## Summary

This program demonstrates:

* Scanner class
* User input using nextInt()
* Modulus operator (%)
* if-else conditional statement
* Even number checking
* Odd number checking
* Resource management using close()

This is one of the most important beginner-level Java programs and is frequently asked in Core Java interviews because it introduces decision-making and arithmetic operators.
