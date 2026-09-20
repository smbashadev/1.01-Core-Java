# Break Statement in Java

## Objective

This program demonstrates the **Break Statement** in Java.

The `break` statement is used to terminate a loop or switch statement immediately when a specified condition is satisfied.

It is commonly used in:

* Searching Operations
* Menu Driven Programs
* Switch Statements
* Input Validation
* Loop Termination Conditions

---

# Definition

The **Break Statement** is a jump statement in Java that immediately terminates:

* for loop
* while loop
* do-while loop
* switch statement

After execution of the `break` statement:

```text
Control transfers to the statement immediately after the loop or switch block.
```

---

# Syntax

```java
break;
```

---

# Flow Diagram

```text
Start Loop

     |

Check Condition

     |

Execute Statements

     |

Check break Condition

     |

True ---------> Exit Loop

False

     |

Continue Loop
```

---

# Program

```java
/*
 * Break Statement Example in Java
 */

public class BreakDemo {

    // Main method - JVM starts execution here
    public static void main(String[] args) {

        // Loop starts from 1 and runs up to 10
        for(int i = 1; i <= 10; i++){

            // Check whether i becomes 5
            if(i == 5){

                // Terminate the loop immediately
                break;

            }

            // Print values before break executes
            System.out.println(i);

        }

        // Executes after loop termination
        System.out.println("Loop stopped at 5.");

    }

}
```

---

## Output

```text
1
2
3
4
Loop stopped at 5.
```

---

## Pseudocode

```text
START

For i = 1 to 10

    If i == 5

        Break

    End If

    Display i

End For

Display "Loop stopped at 5"

STOP
```

---

# Line-by-Line Explanation

### Line 1

```java
for(int i = 1; i <= 10; i++)
```

Explanation:

Creates a loop:

* Initial value = 1
* Condition = i <= 10
* Increment = i++

The loop normally prints:

```text
1 2 3 4 5 6 7 8 9 10
```

But break changes this behavior.

---

### Line 2

```java
if(i == 5)
```

Checks:

```text
Is i equal to 5?
```

For:

```text
i = 1 → false

i = 2 → false

i = 3 → false

i = 4 → false

i = 5 → true
```

---

### Line 3

```java
break;
```

Explanation:

When:

```text
i == 5
```

Java immediately:

```text
Terminates the loop.
```

Control jumps to:

```text
The first statement after the loop.
```

---

### Line 4

```java
System.out.println(i);
```

This statement executes only when:

```text
i != 5
```

Output:

```text
1
2
3
4
```

When:

```text
i = 5
```

break executes before printing.

Therefore:

```text
5 is not printed.
```

---

### Line 5

```java
System.out.println("Loop stopped at 5.");
```

Output:

```text
Loop stopped at 5.
```

This statement executes after the loop ends.

---

# Execution Flow

### Iteration 1

```text
i = 1

1 == 5 ?

False

Print 1
```

---

### Iteration 2

```text
i = 2

2 == 5 ?

False

Print 2
```

---

### Iteration 3

```text
i = 3

3 == 5 ?

False

Print 3
```

---

### Iteration 4

```text
i = 4

4 == 5 ?

False

Print 4
```

---

### Iteration 5

```text
i = 5

5 == 5 ?

True

break

Loop Terminates
```

---

# Break Statement with While Loop

Example:

```java
int i = 1;

while(true){

    if(i == 4){

        break;

    }

    System.out.println(i);

    i++;

}
```

Output:

```text
1
2
3
```

---

# Break Statement with Do-While Loop

```java
int i = 1;

do{

    if(i == 3){

        break;

    }

    System.out.println(i);

    i++;

}while(i <= 5);
```

Output:

```text
1
2
```

---

# Break Statement in Switch

```java
int day = 2;

switch(day){

case 1:

System.out.println("Monday");

break;

case 2:

System.out.println("Tuesday");

break;

}
```

Output:

```text
Tuesday
```

Without break:

```text
The next cases may also execute.
```

---

# Why Do We Use Break?

Break is used when:

```text
The required result is found.
```

Example:

Searching an element:

```text
Find number 50

↓

If Found

↓

Break Loop
```

No need to continue unnecessary iterations.

---

# Real Life Example

ATM Application

```text
1 -> Deposit

2 -> Withdraw

3 -> Exit
```

If user selects:

```text
3
```

Then:

```text
break;

Exit Menu
```

---

# Difference Between Break and Continue

| Break                          | Continue                            |
| ------------------------------ | ----------------------------------- |
| Terminates the loop            | Skips current iteration             |
| Exits loop completely          | Continues next iteration            |
| Transfers control outside loop | Transfers control to loop condition |

---

# Advantages of Break Statement

* Stops unnecessary iterations.
* Improves efficiency.
* Reduces execution time.
* Makes code more readable.
* Widely used in searching and menu programs.

---

# Important Points

1. break is a:

```text
Jump Statement
```

2. It immediately exits:

* for loop
* while loop
* do-while loop
* switch statement

3. Statements after break inside the same block are:

```text
Unreachable
```

4. It improves program performance.

---

# Summary

This program demonstrates:

* Break Statement
* Loop Termination
* Break with For Loop
* Break with While Loop
* Break with Do-While Loop
* Break with Switch Statement
* Execution Flow
* Real-Time Examples

The Break Statement is one of the most important jump statements in Java and is frequently asked in Core Java interviews.
