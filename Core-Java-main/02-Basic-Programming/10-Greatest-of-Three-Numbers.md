# Greatest of Three Numbers in Java

## Objective

This program demonstrates how to find the greatest number among three user-entered integers using:

* Scanner class for user input
* Relational operators (`>`)
* Logical AND operator (`&&`)
* if - else if - else conditional statements

The program compares three numbers and determines which number is the largest.

---

## Program

```java
// Import Scanner class for reading user input
import java.util.Scanner;

// Define a public class named GreaterOf3Num
public class GreaterOf3Num {

    // Main method - JVM starts execution from here
    public static void main(String[] args) {

        // Create Scanner object to read keyboard input
        Scanner sc = new Scanner(System.in);

        // Ask user to enter first number
        System.out.print("Please enter first number: ");

        // Read first integer
        int num1 = sc.nextInt();

        System.out.println();

        // Ask user to enter second number
        System.out.print("Please enter second number: ");

        // Read second integer
        int num2 = sc.nextInt();

        System.out.println();

        // Ask user to enter third number
        System.out.print("Please enter third number: ");

        // Read third integer
        int num3 = sc.nextInt();

        System.out.println();

        // Check whether first number is greater than second and third
        if (num1 > num2 && num1 > num3) {

            System.out.println("First number is greater among three numbers");

        }

        // Check whether second number is greater than first and third
        else if (num2 > num1 && num2 > num3) {

            System.out.println("Second number is greater among three numbers");

        }

        // Otherwise third number is greater
        else {

            System.out.println("Third number is greater among three numbers");

        }

        // Close Scanner object
        sc.close();

    } // End of main method

} // End of GreaterOf3Num class
```

---

## Output - Example 1

```text
Please enter first number: 100

Please enter second number: 50

Please enter third number: 25

First number is greater among three numbers
```

---

## Output - Example 2

```text
Please enter first number: 20

Please enter second number: 90

Please enter third number: 50

Second number is greater among three numbers
```

---

## Output - Example 3

```text
Please enter first number: 20

Please enter second number: 65

Please enter third number: 120

Third number is greater among three numbers
```

---

## Pseudocode

```text
START

Import Scanner

Create Scanner object

Read first number

Read second number

Read third number

If first number is greater than second and third

    Display first number is greater

Else if second number is greater than first and third

    Display second number is greater

Else

    Display third number is greater

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

### Reading First Number

```java
int num1 = sc.nextInt();
```

Explanation:

Reads the first integer entered by the user.

Example:

```text
100
```

Stores:

```java
num1 = 100;
```

---

### Reading Second Number

```java
int num2 = sc.nextInt();
```

Stores:

```java
num2 = 50;
```

---

### Reading Third Number

```java
int num3 = sc.nextInt();
```

Stores:

```java
num3 = 25;
```

---

## First if Condition

```java
if(num1 > num2 && num1 > num3)
```

Explanation:

Checks:

* Is num1 greater than num2?
* Is num1 greater than num3?

If both are true:

```text
First number is greater among three numbers
```

---

## else if Condition

```java
else if(num2 > num1 && num2 > num3)
```

Explanation:

Checks:

* Is num2 greater than num1?
* Is num2 greater than num3?

If both are true:

```text
Second number is greater among three numbers
```

---

## else Block

```java
else
```

Explanation:

If first and second conditions are false:

The third number is considered the greatest.

Output:

```text
Third number is greater among three numbers
```

---

## Relational Operator Used

### Greater Than (>)

Syntax:

```java
a > b
```

Purpose:

Checks whether left operand is greater than right operand.

Example:

```java
100 > 50
```

Output:

```text
true
```

---

## Logical AND Operator (&&)

Syntax:

```java
condition1 && condition2
```

Purpose:

Returns:

```text
true
```

only if both conditions are true.

Example:

```java
100 > 50 && 100 > 25
```

Output:

```text
true
```

---

## Why Do We Use if - else if - else?

This statement is used when:

* Multiple conditions need to be checked.
* Only one block should execute.

Syntax:

```java
if(condition1){

}

else if(condition2){

}

else{

}
```

---

## Special Class Used

### Scanner Class

Package:

```java
java.util.Scanner
```

Purpose:

Accepts user input from keyboard.

---

## Important Scanner Methods

### nextInt()

Syntax:

```java
sc.nextInt();
```

Purpose:

Reads integer input from keyboard.

---

### close()

Syntax:

```java
sc.close();
```

Purpose:

* Releases resources.
* Closes Scanner object.
* Prevents resource leaks.

---

## Summary

This program demonstrates:

* Scanner class
* User input using nextInt()
* Relational operator (>)
* Logical AND operator (&&)
* if - else if - else statement
* Comparing three integers
* Finding the greatest number
* Resource management using close()

This is one of the most important beginner-level Java programs and is frequently asked in Core Java interviews because it introduces multiple conditions and logical operators.
