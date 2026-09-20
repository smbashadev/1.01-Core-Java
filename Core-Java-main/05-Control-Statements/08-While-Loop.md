# While Loop in Java

## Objective

This program demonstrates the **While Loop** in Java.

The `while` loop is a looping control statement that repeatedly executes a block of code as long as the specified condition remains true.

It is commonly used in:

* User input validation
* Menu driven programs
* Reading files
* Database processing
* Repeating operations until a condition changes

---

# Definition

The **While Loop** executes a block of statements repeatedly as long as the given condition evaluates to `true`.

The condition is checked **before** the loop body executes.

If the condition is false initially, the loop body will not execute even once.

---

# Syntax

```java
while(condition){

    // statements

}
```

---

# Flow Diagram

```text
Initialization

      |

Condition ------ False ------> End

      |

     True

      |

Execute Statements

      |

Update Variable

      |

Back to Condition
```

---

# Program

```java
/*
 * While Loop Example in Java
 */

public class WhileLoopDemo {

    // Main method - JVM starts execution here
    public static void main(String[] args) {

        // Initialize loop variable
        int i = 1;

        // Loop executes while condition is true
        while(i <= 5){

            // Print current value of i
            System.out.println(i);

            // Increment loop variable
            i++;

        }

        // Executes after loop terminates
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

WHILE i <= 5

    Display i

    i = i + 1

END WHILE

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
while(i <= 5)
```

Explanation:

Checks:

```text
i <= 5
```

If:

```text
true
```

Loop executes.

If:

```text
false
```

Loop terminates.

---

### Line 3

```java
System.out.println(i);
```

Prints the current value of:

```text
i
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

This increases:

```text
1 → 2 → 3 → 4 → 5 → 6
```

---

### Line 5

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

# How While Loop Executes Internally

### First Iteration

```text
i = 1

1 <= 5

True

Print 1

i++
```

---

### Second Iteration

```text
i = 2

2 <= 5

True

Print 2

i++
```

---

### Third Iteration

```text
i = 3

Print 3
```

---

### Fourth Iteration

```text
i = 4

Print 4
```

---

### Fifth Iteration

```text
i = 5

Print 5
```

---

### Sixth Iteration

```text
i = 6

6 <= 5

False

Loop Terminates
```

---

# Execution Flow

```text
Initialize i = 1

↓

Check Condition

↓

True

↓

Execute Loop Body

↓

Increment i

↓

Check Condition Again

↓

False

↓

Exit Loop
```

---

# Infinite While Loop

Example:

```java
while(true){

    System.out.println("Hello");

}
```

Output:

```text
Hello
Hello
Hello
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

# Example with False Condition Initially

```java
int i = 10;

while(i <= 5){

    System.out.println(i);

}
```

Condition:

```text
10 <= 5
```

Result:

```text
False
```

Output:

```text
No Output
```

Because:

```text
The loop never executes.
```

---

# Difference Between For Loop and While Loop

| For Loop                       | While Loop                       |
| ------------------------------ | -------------------------------- |
| Used when iterations are known | Used when iterations are unknown |
| Initialization inside loop     | Initialization outside loop      |
| Compact syntax                 | Flexible syntax                  |
| Mostly counting based          | Mostly condition based           |

---

# Real Life Example

ATM Menu:

```text
While User is Logged In

↓

Show Menu

↓

Perform Transaction

↓

Ask Continue?

↓

Repeat Until User Exits
```

---

# Advantages of While Loop

* Simple to understand.
* Suitable for unknown iterations.
* Flexible and easy to maintain.
* Widely used in real-world applications.
* Ideal for condition-based repetition.

---

# Important Points

1. Condition is checked before execution.

2. Loop may execute:

```text
Zero Times
```

or

```text
Multiple Times
```

3. Update statement is important.

4. Failure to update may create:

```text
Infinite Loop
```

---

# Summary

This program demonstrates:

* While Loop
* Initialization
* Condition Checking
* Increment Operation
* Loop Execution Flow
* Infinite Loop
* For vs While Loop
* Real-Time Examples

The While Loop is one of the most important looping constructs in Java and is frequently asked in Core Java interviews.
