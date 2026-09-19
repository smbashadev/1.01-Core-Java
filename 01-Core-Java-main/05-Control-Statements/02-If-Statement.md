# If Statement in Java

## Objective

This program demonstrates the **If Statement** in Java.

The `if` statement is the simplest decision-making statement in Java. It executes a block of code only when the specified condition evaluates to `true`.

It is widely used in:

* Age validation
* Login verification
* Eligibility checking
* Marks and grading systems
* Banking and transaction validation

---

# Definition

The **if statement** executes a block of code only if the given condition is true.

If the condition is false, the statements inside the if block are skipped.

---

# Syntax

```java
if(condition){

    // Statements

}
```

---

# Flow Diagram

```text
          Condition

             |

        True | False

             |

     Execute Block

             |

            End
```

---

# Program

```java
/*
 * If Statement Example in Java
 */

public class IfDemo {

    // Main method - JVM starts execution from here
    public static void main(String[] args) {

        // Declare and initialize age variable
        int age = 18;

        // Check whether age is greater than or equal to 18
        if (age >= 18) {

            // Executes only when condition is true
            System.out.println("You are eligible to vote.");

        }

        // Executes after the if block
        System.out.println("Program finished.");

    }

}
```

---

## Output

```text
You are eligible to vote.
Program finished.
```

---

## Pseudocode

```text
START

Declare age = 18

If age >= 18

    Display "You are eligible to vote."

End If

Display "Program finished."

STOP
```

---

# Line-by-Line Explanation

### Line 1

```java
int age = 18;
```

Explanation:

* Declares an integer variable named `age`.
* Assigns the value `18`.

Memory Representation:

```text
age = 18
```

---

### Line 2

```java
if(age >= 18)
```

Explanation:

The condition checks:

```text
18 >= 18
```

Result:

```text
true
```

Since the condition is true:

```text
The statements inside the if block will execute.
```

---

### Line 3

```java
System.out.println("You are eligible to vote.");
```

Explanation:

This statement prints:

```text
You are eligible to vote.
```

because:

```text
Condition = true
```

---

### Line 4

```java
System.out.println("Program finished.");
```

Explanation:

This statement executes after the if block regardless of the condition.

Output:

```text
Program finished.
```

---

# How If Statement Works Internally

Step 1:

Evaluate the condition.

```java
age >= 18
```

↓

Step 2:

If result is:

```text
true
```

Execute:

```java
System.out.println("You are eligible to vote.");
```

↓

Step 3:

Continue with the remaining statements.

---

# Example with False Condition

```java
int age = 15;

if(age >= 18){

System.out.println("Eligible");

}
```

Condition:

```text
15 >= 18
```

Result:

```text
false
```

Output:

```text
No Output
```

Because the if block is skipped.

---

# Relational Operators Used in If Statement

| Operator | Meaning                  |
| -------- | ------------------------ |
| >        | Greater Than             |
| <        | Less Than                |
| >=       | Greater Than or Equal To |
| <=       | Less Than or Equal To    |
| ==       | Equal To                 |
| !=       | Not Equal To             |

---

## Examples

```java
age > 18

marks >= 35

salary == 50000

number != 0
```

---

# Important Points

1. The condition must return:

```text
true

or

false
```

2. Curly braces:

```java
{

}
```

define the if block.

3. If the condition is false:

```text
The block is skipped.
```

4. If the condition is true:

```text
The block executes.
```

---

# Real Life Example

```text
If Account Balance > Withdrawal Amount

↓

Allow Withdrawal

Else

Reject Transaction
```

---

# Advantages of If Statement

* Supports decision making.
* Executes statements conditionally.
* Improves program flexibility.
* Easy to understand and maintain.
* Used extensively in real-world applications.

---

# Summary

This program demonstrates:

* If Statement
* Decision Making in Java
* Relational Operators
* Boolean Conditions
* Conditional Execution
* Flow of If Statement

The `if` statement is the foundation of all decision-making constructs in Java and is one of the most frequently asked topics in Core Java interviews.
