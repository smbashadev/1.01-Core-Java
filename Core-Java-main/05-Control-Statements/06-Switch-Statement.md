# Switch Statement in Java

## Objective

This program demonstrates the **Switch Statement** in Java.

The `switch` statement is a multi-way decision-making statement used to select one block of code from several alternatives based on the value of an expression.

It is commonly used in:

* Menu Driven Programs
* Calculator Applications
* ATM Systems
* Day and Month Selection
* Employee Role Management
* Banking Applications

---

# Definition

The **Switch Statement** allows a program to execute one block of code from multiple choices.

The value of the expression is compared with different `case` values.

If a matching case is found:

* The corresponding block executes.
* The `break` statement terminates the switch block.

If no case matches:

* The `default` block executes.

---

# Syntax

```java
switch(expression){

    case value1:
        // statements
        break;

    case value2:
        // statements
        break;

    case value3:
        // statements
        break;

    default:
        // statements

}
```

---

# Flow Diagram

```text
              Expression

                    |

          -----------------

          |       |       |

        Case1   Case2   Case3

          |       |       |

        Match   Match   Match

          |       |       |

        Execute Matching Block

                    |

                 break

                    |

                   End


If no case matches

↓

default block executes
```

---

# Program

```java
/*
 * Switch Statement Example in Java
 */

public class SwitchDemo {

    // Main method - JVM starts execution here
    public static void main(String[] args) {

        // Declare a variable for day
        int day = 3;

        // Switch statement
        switch(day){

            case 1:

                // Executes when day is 1
                System.out.println("Monday");
                break;

            case 2:

                // Executes when day is 2
                System.out.println("Tuesday");
                break;

            case 3:

                // Executes when day is 3
                System.out.println("Wednesday");
                break;

            default:

                // Executes when no case matches
                System.out.println("Invalid day");

        }

        // Executes after switch block
        System.out.println("Program finished.");

    }

}
```

---

## Output

```text
Wednesday
Program finished.
```

---

## Pseudocode

```text
START

Declare day = 3

Switch(day)

Case 1

    Display Monday

    Break

Case 2

    Display Tuesday

    Break

Case 3

    Display Wednesday

    Break

Default

    Display Invalid day

End Switch

Display Program finished

STOP
```

---

# Line-by-Line Explanation

### Line 1

```java
int day = 3;
```

Explanation:

Creates an integer variable:

```text
day
```

Stores:

```text
3
```

---

### Line 2

```java
switch(day)
```

Explanation:

The switch statement evaluates:

```text
day = 3
```

and compares it with:

```text
case 1

case 2

case 3
```

---

### Line 3

```java
case 1:
```

Checks:

```text
3 == 1
```

Result:

```text
false
```

This block is skipped.

---

### Line 4

```java
case 2:
```

Checks:

```text
3 == 2
```

Result:

```text
false
```

This block is skipped.

---

### Line 5

```java
case 3:
```

Checks:

```text
3 == 3
```

Result:

```text
true
```

Therefore:

```text
Print Wednesday
```

Output:

```text
Wednesday
```

---

### Line 6

```java
break;
```

Explanation:

The `break` statement:

* Terminates the switch block.
* Prevents execution of remaining cases.

Control transfers outside the switch statement.

---

### Line 7

```java
default:
```

The default block executes only when:

```text
No case matches.
```

Example:

```java
int day = 8;
```

Output:

```text
Invalid day
```

---

### Line 8

```java
System.out.println("Program finished.");
```

Output:

```text
Program finished.
```

This statement executes after the switch block.

---

# How Switch Statement Works

Suppose:

```text
day = 3
```

Java checks:

```text
Case 1

3 == 1

False
```

↓

```text
Case 2

3 == 2

False
```

↓

```text
Case 3

3 == 3

True
```

↓

```text
Print Wednesday
```

↓

```text
break
```

↓

```text
Exit Switch
```

---

# What Happens Without break?

Example:

```java
int day = 2;

switch(day){

case 1:
System.out.println("Monday");

case 2:
System.out.println("Tuesday");

case 3:
System.out.println("Wednesday");

}
```

Output:

```text
Tuesday
Wednesday
```

Reason:

Without `break`, Java executes all remaining cases.

This behavior is called:

```text
Fall Through
```

---

# Data Types Supported by Switch

Java Switch supports:

```text
byte

short

int

char

String

enum
```

Example:

```java
String day = "Monday";

switch(day){

case "Monday":

System.out.println("Working Day");

break;

}
```

---

# Real Life Example

ATM Menu:

```text
1 -> Balance Enquiry

2 -> Deposit

3 -> Withdraw

4 -> Exit
```

The user selects one option:

```text
Switch executes the matching case.
```

---

# Difference Between Else-If Ladder and Switch

| Else-If Ladder                 | Switch Statement        |
| ------------------------------ | ----------------------- |
| Used for ranges and conditions | Used for fixed values   |
| Multiple boolean expressions   | Single expression       |
| Slower for many options        | Faster for many options |
| More flexible                  | More readable           |

---

# Important Points

1. Switch evaluates only one expression.

2. Case values must be:

```text
Constant Values
```

3. The `break` statement is used to:

```text
Terminate the switch block.
```

4. The `default` block is optional.

5. Multiple cases can share the same block.

---

# Advantages of Switch Statement

* Improves readability.
* Faster than long else-if ladders.
* Suitable for menu-driven programs.
* Easy to maintain.
* Supports multiple fixed choices.

---

# Summary

This program demonstrates:

* Switch Statement
* Case Labels
* break Statement
* default Block
* Fall Through Concept
* Execution Flow
* Supported Data Types
* Difference Between Switch and Else-If Ladder

The Switch Statement is one of the most important decision-making constructs in Java and is frequently asked in Core Java interviews.
