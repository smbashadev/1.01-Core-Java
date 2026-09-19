# Else-If Ladder in Java

## Objective

This program demonstrates the **Else-If Ladder** in Java.

The Else-If Ladder is used when multiple conditions need to be checked one after another.

It allows the program to choose **only one block of code** from many alternatives based on the condition that becomes true first.

This control statement is commonly used in:

* Student Grade Systems
* Employee Salary Slabs
* Tax Calculations
* Menu Driven Programs
* Banking Applications

---

# Definition

The **Else-If Ladder** is a sequence of:

* if statement
* one or more else if statements
* optional else statement

The conditions are checked from top to bottom.

As soon as one condition becomes true:

```text id="8u2s8q"
Remaining conditions are skipped.
```

---

# Syntax

```java id="tkqjvx"
if(condition1){

    // statements

}

else if(condition2){

    // statements

}

else if(condition3){

    // statements

}

else{

    // statements

}
```

---

# Flow Diagram

```text id="tjlwmq"
          Condition 1

          /        \

      True        False

       |             |

   Block 1       Condition 2

                    |

               True | False

                    |

                Block 2

                    |

               Condition 3

                    |

               True | False

                    |

                Block 3

                    |

                 Else Block
```

---

# Program

```java id="lpmryj"
/*
 * Else-If Ladder Example in Java
 */

public class ElseIfDemo {

    // Main method - JVM starts execution here
    public static void main(String[] args) {

        // Declare marks variable
        int marks = 75;

        // Check first condition
        if (marks >= 90) {

            System.out.println("Grade A");

        }

        // Check second condition
        else if (marks >= 75) {

            System.out.println("Grade B");

        }

        // Check third condition
        else if (marks >= 60) {

            System.out.println("Grade C");

        }

        // Executes when all conditions are false
        else {

            System.out.println("Fail");

        }

        // Executes after the ladder
        System.out.println("Program finished.");

    }

}
```

---

## Output

```text id="v2z3cr"
Grade B
Program finished.
```

---

## Pseudocode

```text id="lcr6jt"
START

Declare marks = 75

If marks >= 90

    Display Grade A

Else If marks >= 75

    Display Grade B

Else If marks >= 60

    Display Grade C

Else

    Display Fail

End If

Display Program Finished

STOP
```

---

# Line-by-Line Explanation

### Line 1

```java id="s34gv6"
int marks = 75;
```

Explanation:

Creates an integer variable:

```text id="uyqg5x"
marks
```

and stores:

```text id="rxf2xy"
75
```

---

### Line 2

```java id="0m6k6f"
if(marks >= 90)
```

Condition:

```text id="9op4ij"
75 >= 90
```

Result:

```text id="mh4bx4"
false
```

Therefore:

```text id="umq77i"
This block is skipped.
```

---

### Line 3

```java id="3bnc4x"
else if(marks >= 75)
```

Condition:

```text id="cxgm5f"
75 >= 75
```

Result:

```text id="40btyt"
true
```

Therefore:

```text id="th6r5e"
Grade B is printed.
```

Output:

```text id="v0gm4z"
Grade B
```

---

### Line 4

```java id="r4j88k"
else if(marks >= 60)
```

This condition is:

```text id="5ms7dj"
Not Checked
```

because:

```text id="y7qcx8"
Previous condition is already true.
```

---

### Line 5

```java id="mgn9n6"
else
```

This block executes only when:

```text id="4ylxfr"
All conditions become false.
```

In this example:

```text id="mf3hht"
Skipped
```

---

### Line 6

```java id="u6x4mb"
System.out.println("Program finished.");
```

Executes after the ladder.

Output:

```text id="hhy5gt"
Program finished.
```

---

# How Else-If Ladder Works

Suppose:

```text id="2a3jtl"
marks = 75
```

Java checks:

```text id="4x7f8r"
75 >= 90

False
```

↓

```text id="bjzssz"
75 >= 75

True
```

↓

```text id="r2vdtj"
Print Grade B
```

↓

```text id="5a5zpd"
Stop Checking Remaining Conditions
```

---

# Why Does Java Stop After First True Condition?

Because:

```text id="38v71g"
Else-If Ladder executes only ONE block.
```

This improves:

* Performance
* Readability
* Efficiency

---

# Another Example

```java id="i5sdwq"
int marks = 95;
```

Condition:

```text id="rucd9e"
95 >= 90

True
```

Output:

```text id="oaq4t1"
Grade A
```

Remaining conditions:

```text id="h4i67z"
Skipped
```

---

# Real Life Example

Student Grading System:

```text id="5j5m8o"
Marks >= 90

Grade A


Marks >= 75

Grade B


Marks >= 60

Grade C


Otherwise

Fail
```

---

# Difference Between if-else and else-if Ladder

| if-else                            | else-if Ladder       |
| ---------------------------------- | -------------------- |
| Two choices                        | Multiple choices     |
| One condition                      | Multiple conditions  |
| One true block and one false block | One block among many |
| Simple decisions                   | Complex decisions    |

---

# Important Points

1. Conditions are checked:

```text id="mg6zrq"
Top to Bottom
```

2. Only:

```text id="zwtt2k"
One Block Executes
```

3. Remaining conditions are skipped after first true condition.

4. Final:

```java id="yx3bbv"
else
```

is optional.

5. Frequently used in:

* Grading Systems
* Menu Programs
* Banking Applications
* Salary Calculations

---

# Advantages of Else-If Ladder

* Supports multiple conditions.
* Improves readability.
* Easy to maintain.
* Efficient execution.
* Suitable for real-world applications.

---

# Summary

This program demonstrates:

* Else-If Ladder
* Multiple Condition Checking
* Decision Making
* Flow of Else-If Statements
* Grade Calculation Logic
* Execution Flow
* Real-Time Usage

Else-If Ladder is one of the most important decision-making constructs in Java and is frequently asked in Core Java interviews.
