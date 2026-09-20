# If-Else Statement in Java

## Objective

This program demonstrates the **If-Else Statement** in Java.

The `if-else` statement is a decision-making statement that allows a program to choose between two different execution paths based on a condition.

It is commonly used for:

* Even or Odd Number Checking
* Voting Eligibility
* Pass or Fail Results
* Login Authentication
* Age Verification
* Banking Applications

---

# Definition

The **if-else statement** executes:

* One block of code if the condition is **true**.
* Another block of code if the condition is **false**.

Only one block executes at a time.

---

# Syntax

```java
if(condition){

    // True Block

}

else{

    // False Block

}
```

---

# Flow Diagram

```text
             Condition

            /        \

         True        False

          |             |

   Execute if      Execute else
      Block           Block

           \         /

              End
```

---

# Program

```java
/*
 * If-Else Statement Example in Java
 */

public class IfElseDemo {

    // Main method - JVM starts execution here
    public static void main(String[] args) {

        // Declare an integer variable
        int number = 10;

        // Check whether the number is even
        if (number % 2 == 0) {

            // Executes when condition is true
            System.out.println("The number is even.");

        }

        else {

            // Executes when condition is false
            System.out.println("The number is odd.");

        }

        // Executes after if-else block
        System.out.println("Program finished.");

    }

}
```

---

## Output

```text
The number is even.
Program finished.
```

---

## Pseudocode

```text
START

Declare number = 10

If number % 2 == 0

    Display "The number is even."

Else

    Display "The number is odd."

End If

Display "Program finished."

STOP
```

---

# Line-by-Line Explanation

### Line 1

```java
int number = 10;
```

Explanation:

Declares an integer variable named:

```text
number
```

and assigns:

```text
10
```

---

### Line 2

```java
if(number % 2 == 0)
```

Explanation:

The `%` operator is called:

```text
Modulus Operator
```

It returns the remainder.

Calculation:

```text
10 % 2 = 0
```

Condition:

```text
0 == 0
```

Result:

```text
true
```

---

### Line 3

```java
System.out.println("The number is even.");
```

Since:

```text
Condition = true
```

This statement executes.

Output:

```text
The number is even.
```

---

### Line 4

```java
else
```

The else block executes only when:

```text
Condition = false
```

In this example:

```text
Condition = true
```

Therefore:

```text
Else block is skipped.
```

---

### Line 5

```java
System.out.println("Program finished.");
```

This statement executes after the if-else block.

Output:

```text
Program finished.
```

---

# How Even-Odd Logic Works

Condition:

```java
number % 2 == 0
```

Meaning:

If remainder is:

```text
0
```

Then:

```text
Even Number
```

Otherwise:

```text
Odd Number
```

---

## Example

```text
8 % 2 = 0

Even
```

```text
11 % 2 = 1

Odd
```

---

# What is Modulus (%) Operator?

The modulus operator:

```java
%
```

returns:

```text
Remainder after division
```

Examples:

```text
10 % 2 = 0

15 % 2 = 1

20 % 3 = 2
```

---

# Execution Flow

```text
number = 10

↓

10 % 2 == 0

↓

True

↓

Print:

"The number is even."

↓

Print:

"Program finished."

↓

End
```

---

# Example with False Condition

```java
int number = 7;

if(number % 2 == 0){

System.out.println("Even");

}

else{

System.out.println("Odd");

}
```

Condition:

```text
7 % 2 = 1
```

Result:

```text
false
```

Output:

```text
Odd
```

---

# Difference Between if and if-else

| if                                   | if-else                    |
| ------------------------------------ | -------------------------- |
| Executes only when condition is true | Executes one of two blocks |
| No false block                       | Has false block            |
| Single path                          | Two execution paths        |

---

# Important Points

1. Condition must return:

```text
true

or

false
```

2. Only one block executes.

3. The else block is optional.

4. Curly braces define blocks:

```java
{

}
```

5. Widely used in decision-making programs.

---

# Real Life Example

```text
If Username and Password are Correct

↓

Login Success

Else

Login Failed
```

---

# Advantages of If-Else Statement

* Supports two-way decision making.
* Easy to understand.
* Improves program flexibility.
* Reduces unnecessary code.
* Useful in real-world applications.

---

# Summary

This program demonstrates:

* If-Else Statement
* Decision Making
* Modulus Operator
* Even-Odd Logic
* Boolean Conditions
* Execution Flow
* Difference Between if and if-else

The If-Else Statement is one of the most important decision-making constructs in Java and is frequently asked in Core Java interviews.
