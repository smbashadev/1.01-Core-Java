# Do-While Loop in Java

## Objective

This program demonstrates the **Do-While Loop** in Java.

The `do-while` loop is a looping statement that executes the loop body first and then checks the condition.

This guarantees:

```text
The loop body executes at least one time.
```

It is commonly used in:

* Menu Driven Programs
* ATM Applications
* Login Systems
* User Input Validation
* Game Menus

---

# Definition

The **Do-While Loop** executes a block of code first and then evaluates the condition.

If the condition is:

* True → Loop continues.
* False → Loop terminates.

Unlike the `while` loop:

```text
Condition is checked after execution.
```

Therefore:

```text
Minimum Iterations = 1
```

---

# Syntax

```java
do{

    // statements

}while(condition);
```

---

# Flow Diagram

```text
Initialization

      |

Execute Statements

      |

Update Variable

      |

Check Condition

   True | False

      |      |

Repeat    End
```

---

# Program

```java
/*
 * Do-While Loop Example in Java
 */

public class DoWhileLoopDemo {

    // Main method - JVM starts execution here
    public static void main(String[] args) {

        // Initialize loop variable
        int i = 1;

        // Execute loop body first
        do{

            // Print current value
            System.out.println(i);

            // Increment i
            i++;

        }

        // Check condition after execution
        while(i <= 5);

        // Executes after loop termination
        System.out.println("Loop finished.");

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
5
Loop finished.
```

---

## Pseudocode

```text
START

Set i = 1

DO

    Display i

    i = i + 1

WHILE i <= 5

Display "Loop finished."

STOP
```

---

# Line-by-Line Explanation

### Line 1

```java
int i = 1;
```

Explanation:

Creates an integer variable:

```text
i
```

Stores:

```text
1
```

This is called:

```text
Initialization
```

---

### Line 2

```java
do{
```

Explanation:

The loop body executes immediately.

No condition is checked here.

This is the major difference from:

```text
while loop
```

---

### Line 3

```java
System.out.println(i);
```

Prints:

```text
Current value of i
```

---

### Line 4

```java
i++;
```

Equivalent to:

```java
i = i + 1;
```

Updates:

```text
1 → 2 → 3 → 4 → 5 → 6
```

---

### Line 5

```java
while(i <= 5);
```

Checks:

```text
i <= 5
```

If:

```text
True
```

Loop repeats.

If:

```text
False
```

Loop terminates.

---

### Line 6

```java
System.out.println("Loop finished.");
```

Executes after:

```text
Condition becomes false.
```

Output:

```text
Loop finished.
```

---

# Execution Flow

### First Iteration

```text
i = 1

Execute Body

Print 1

i++

i = 2

Check:

2 <= 5

True
```

---

### Second Iteration

```text
Print 2

i = 3

3 <= 5

True
```

---

### Third Iteration

```text
Print 3
```

---

### Fourth Iteration

```text
Print 4
```

---

### Fifth Iteration

```text
Print 5
```

---

### Sixth Iteration

```text
i = 6

6 <= 5

False

Loop Ends
```

---

# Special Feature of Do-While Loop

Even if the condition is false initially:

```java
int i = 10;

do{

System.out.println(i);

}while(i <= 5);
```

Output:

```text
10
```

Reason:

```text
The loop body executes before checking the condition.
```

---

# Comparison Between While and Do-While

| While Loop              | Do-While Loop          |
| ----------------------- | ---------------------- |
| Condition checked first | Body executed first    |
| May execute zero times  | Executes at least once |
| Entry Controlled Loop   | Exit Controlled Loop   |
| Condition at top        | Condition at bottom    |

---

# Infinite Do-While Loop

Example:

```java
do{

System.out.println("Java");

}while(true);
```

Output:

```text
Java
Java
Java
...
```

Reason:

```text
Condition is always true.
```

This is called:

```text
Infinite Loop
```

---

# Real Life Example

ATM Program

```text
DO

Display Menu

1. Deposit

2. Withdraw

3. Balance

4. Exit

Ask User Choice

WHILE Choice != Exit
```

The menu appears at least once.

---

# Advantages of Do-While Loop

* Executes at least one time.
* Suitable for menu-driven programs.
* Easy to use for input validation.
* Simple and readable syntax.
* Widely used in real-world applications.

---

# Important Points

1. Condition is checked after execution.

2. Minimum iterations:

```text
1
```

3. It is called:

```text
Exit Controlled Loop
```

4. A semicolon is mandatory:

```java
while(condition);
               ^
```

---

# Summary

This program demonstrates:

* Do-While Loop
* Exit Controlled Loop
* Loop Execution Flow
* Condition Checking
* Minimum One Execution
* Infinite Loop
* While vs Do-While
* Real-Time Examples

The Do-While Loop is an important looping construct in Java and is frequently asked in Core Java interviews.
