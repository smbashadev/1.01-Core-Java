# For Loop in Java

## Objective

This program demonstrates the **For Loop** in Java.

The `for` loop is a looping statement used to execute a block of code repeatedly for a fixed number of times.

It is commonly used in:

* Printing numbers
* Generating multiplication tables
* Array traversal
* Pattern programs
* Mathematical calculations
* Iterative processing

---

# Definition

The **For Loop** is used when the number of iterations is known in advance.

It consists of three parts:

1. Initialization
2. Condition
3. Increment/Decrement

The loop executes until the condition becomes false.

---

# Syntax

```java
for(initialization; condition; increment/decrement){

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

Increment / Decrement

      |

Back to Condition
```

---

# Program

```java
/*
 * For Loop Example in Java
 */

public class ForLoopDemo {

    // Main method - JVM starts execution here
    public static void main(String[] args) {

        // For loop from 1 to 5
        for(int i = 1; i <= 5; i++){

            // Print current value of i
            System.out.println(i);

        }

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

For i = 1 to 5

    Display i

End For

Display "Loop finished."

STOP
```

---

# Line-by-Line Explanation

### Line 1

```java
for(int i = 1; i <= 5; i++)
```

This statement contains three parts:

**Initialization**

```java
int i = 1
```

* Declares variable `i`
* Assigns initial value `1`
* Executes only once.

---

**Condition**

```java
i <= 5
```

* Checks whether `i` is less than or equal to 5.
* If true, loop executes.
* If false, loop terminates.

---

**Increment**

```java
i++
```

Equivalent to:

```java
i = i + 1;
```

After each iteration:

```text
1 → 2 → 3 → 4 → 5 → 6
```

---

### Line 2

```java
System.out.println(i);
```

Prints the current value of:

```text
i
```

Output:

```text
1
2
3
4
5
```

---

### Line 3

```java
System.out.println("Loop finished.");
```

Executes after the loop condition becomes false.

Output:

```text
Loop finished.
```

---

# How For Loop Executes Internally

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

# Components of For Loop

| Component      | Purpose                       |
| -------------- | ----------------------------- |
| Initialization | Starting value                |
| Condition      | Checks whether loop continues |
| Increment      | Updates loop variable         |
| Body           | Statements inside loop        |

---

# Reverse For Loop

```java
for(int i = 5; i >= 1; i--){

System.out.println(i);

}
```

Output:

```text
5
4
3
2
1
```

---

# Nested For Loop

```java
for(int i=1;i<=3;i++){

    for(int j=1;j<=2;j++){

        System.out.println(i + " " + j);

    }

}
```

Output:

```text
1 1
1 2
2 1
2 2
3 1
3 2
```

---

# Real Life Example

Printing Multiplication Table:

```java
for(int i=1;i<=10;i++){

System.out.println(5 * i);

}
```

Output:

```text
5
10
15
20
25
30
35
40
45
50
```

---

# Difference Between For and While Loop

| For Loop                       | While Loop                       |
| ------------------------------ | -------------------------------- |
| Used when iterations are known | Used when iterations are unknown |
| Initialization inside loop     | Initialization outside loop      |
| Compact syntax                 | More flexible                    |
| Mostly used for counting       | Mostly used for conditions       |

---

# Advantages of For Loop

* Easy to write.
* Suitable for fixed iterations.
* Compact syntax.
* Improves readability.
* Widely used in arrays and collections.

---

# Summary

This program demonstrates:

* For Loop
* Initialization
* Condition Checking
* Increment Operator
* Loop Execution Flow
* Reverse Loop
* Nested Loop
* Real-Time Examples

The For Loop is one of the most fundamental looping constructs in Java and is frequently asked in Core Java interviews.
