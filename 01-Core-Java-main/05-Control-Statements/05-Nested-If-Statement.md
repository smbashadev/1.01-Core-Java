# Nested If Statement in Java

## Objective

This program demonstrates the **Nested If Statement** in Java.

A Nested If Statement means placing one `if` statement inside another `if` statement.

The inner `if` statement executes only when the outer `if` condition is true.

Nested If is commonly used in:

* Login and Security Systems
* Banking Applications
* Student Eligibility Systems
* Employee Verification
* Admission Systems

---

# Definition

A **Nested If Statement** is an `if` statement placed inside another `if` statement.

It is used when:

```text
One condition depends on another condition.
```

The inner condition is checked only if the outer condition becomes true.

---

# Syntax

```java
if(condition1){

    if(condition2){

        // Statements

    }

}
```

---

# Flow Diagram

```text
           Condition 1

          /          \

      True           False

        |

   Condition 2

    /        \

 True       False

   |

Statements

   |

  End
```

---

# Program

```java
/*
 * Nested If Statement Example in Java
 */

public class NestedIf {

    // Main method - JVM starts execution here
    public static void main(String[] args) {

        // Declare age variable
        int age = 20;

        // Declare weight variable
        int weight = 55;

        // Outer if condition
        if (age >= 18) {

            // Inner if condition
            if (weight > 50) {

                // Executes when both conditions are true
                System.out.println("You are eligible for the gym.");

            }

        }

        // Executes after nested if block
        System.out.println("Program finished.");

    }

}
```

---

## Output

```text
You are eligible for the gym.
Program finished.
```

---

## Pseudocode

```text
START

Declare age = 20

Declare weight = 55

If age >= 18

    If weight > 50

        Display "You are eligible for the gym."

    End If

End If

Display "Program finished."

STOP
```

---

# Line-by-Line Explanation

### Line 1

```java
int age = 20;
```

Explanation:

Creates an integer variable:

```text
age
```

Stores:

```text
20
```

---

### Line 2

```java
int weight = 55;
```

Explanation:

Creates another integer variable:

```text
weight
```

Stores:

```text
55
```

---

### Line 3

```java
if(age >= 18)
```

Explanation:

Checks:

```text
20 >= 18
```

Result:

```text
true
```

Therefore:

```text
Inner if statement will execute.
```

---

### Line 4

```java
if(weight > 50)
```

Explanation:

Checks:

```text
55 > 50
```

Result:

```text
true
```

Therefore:

```text
The message will be printed.
```

---

### Line 5

```java
System.out.println("You are eligible for the gym.");
```

Output:

```text
You are eligible for the gym.
```

This statement executes because:

```text
Outer Condition = true

Inner Condition = true
```

---

### Line 6

```java
System.out.println("Program finished.");
```

This statement executes after the nested if block.

Output:

```text
Program finished.
```

---

# Execution Flow

```text
age = 20

↓

Check:

age >= 18

↓

True

↓

Check:

weight > 50

↓

True

↓

Print:

You are eligible for the gym.

↓

Program finished.
```

---

# Example with False Outer Condition

```java
int age = 15;

if(age >= 18){

    if(weight > 50){

        System.out.println("Eligible");

    }

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

Because:

```text
Inner if is never executed.
```

---

# Example with False Inner Condition

```java
int age = 20;

int weight = 45;
```

Outer Condition:

```text
20 >= 18

True
```

Inner Condition:

```text
45 > 50

False
```

Output:

```text
Program finished.
```

The inner block does not execute.

---

# Why Do We Use Nested If?

Nested If is used when:

```text
Second condition depends on first condition.
```

Example:

```text
If User Logged In

↓

Check Admin Permission

↓

Allow Access
```

The second condition is checked only after the first becomes true.

---

# Real Life Example

Gym Eligibility:

```text
Age >= 18

↓

Weight > 50

↓

Eligible for Gym
```

Both conditions must be satisfied.

---

# Difference Between if and Nested if

| if Statement     | Nested if Statement              |
| ---------------- | -------------------------------- |
| Single Condition | Multiple Conditions              |
| One Decision     | Decision inside another Decision |
| Simpler          | More Complex                     |
| Independent      | Dependent Conditions             |

---

# Important Points

1. Nested If means:

```text
If inside another If
```

2. Inner if executes only when outer if is true.

3. Used for dependent conditions.

4. Supports multiple levels of nesting.

Example:

```java
if(){

    if(){

        if(){

        }

    }

}
```

---

# Advantages of Nested If

* Supports multiple condition checking.
* Useful for hierarchical decisions.
* Improves program logic.
* Used in authentication and validation systems.
* Suitable for real-world applications.

---

# Summary

This program demonstrates:

* Nested If Statement
* Outer and Inner If Conditions
* Multiple Condition Checking
* Dependent Decision Making
* Execution Flow
* Real-Time Eligibility Checking
* Difference Between if and Nested if

Nested If Statements are widely used in Java applications where one condition depends on another condition and are frequently asked in Core Java interviews.
