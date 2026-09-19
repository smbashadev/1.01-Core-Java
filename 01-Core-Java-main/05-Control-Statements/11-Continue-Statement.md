# Continue Statement in Java

## Objective

This program demonstrates the **Continue Statement** in Java.

The `continue` statement is used to skip the current iteration of a loop and immediately move to the next iteration.

Unlike the `break` statement:

```text
break    → Terminates the entire loop

continue → Skips only the current iteration
```

It is commonly used in:

* Filtering data
* Skipping invalid input
* Searching operations
* Processing arrays
* Menu-driven programs

---

# Definition

The **Continue Statement** is a jump statement that skips the remaining statements of the current iteration and transfers control to the next iteration of the loop.

It can be used with:

* for loop
* while loop
* do-while loop

---

# Syntax

```java
continue;
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

Check Continue Condition

     |

True -------------> Next Iteration

False

     |

Execute Remaining Statements

     |

Repeat Loop
```

---

# Program

```java
/*
 * Continue Statement Example in Java
 */

public class ContinueDemo {

    // Main method - JVM starts execution here
    public static void main(String[] args) {

        // Loop from 1 to 5
        for(int i = 1; i <= 5; i++) {

            // Skip the iteration when i becomes 3
            if(i == 3) {

                continue;

            }

            // Print values except 3
            System.out.println(i);

        }

        // Executes after loop completion
        System.out.println("Loop finished.");

    }

}
```

---

## Output

```text
1
2
4
5
Loop finished.
```

---

## Pseudocode

```text
START

For i = 1 to 5

    If i == 3

        Continue

    End If

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

Explanation:

Creates a loop:

* Initial value = 1
* Condition = i <= 5
* Increment = i++

Normally output would be:

```text
1
2
3
4
5
```

But continue changes this behavior.

---

### Line 2

```java
if(i == 3)
```

Checks:

```text
Is i equal to 3 ?
```

If:

```text
True
```

Then:

```java
continue;
```

is executed.

---

### Line 3

```java
continue;
```

Explanation:

Skips:

```text
The remaining statements of the current iteration.
```

Control moves directly to:

```text
Next iteration of the loop.
```

---

### Line 4

```java
System.out.println(i);
```

This statement executes only when:

```text
i != 3
```

Therefore output becomes:

```text
1
2
4
5
```

---

# Execution Flow

### Iteration 1

```text
i = 1

1 == 3 ?

False

Print 1
```

---

### Iteration 2

```text
i = 2

2 == 3 ?

False

Print 2
```

---

### Iteration 3

```text
i = 3

3 == 3 ?

True

continue

Skip printing

Move to next iteration
```

---

### Iteration 4

```text
i = 4

Print 4
```

---

### Iteration 5

```text
i = 5

Print 5
```

---

# Continue with While Loop

Example:

```java
int i = 0;

while(i < 5){

    i++;

    if(i == 3){

        continue;

    }

    System.out.println(i);

}
```

Output:

```text
1
2
4
5
```

---

# Continue with Do-While Loop

```java
int i = 0;

do{

    i++;

    if(i == 3){

        continue;

    }

    System.out.println(i);

}while(i < 5);
```

Output:

```text
1
2
4
5
```

---

# Difference Between Break and Continue

| Break                          | Continue                       |
| ------------------------------ | ------------------------------ |
| Terminates the loop completely | Skips current iteration only   |
| Control goes outside loop      | Control goes to next iteration |
| Used to stop execution         | Used to ignore certain values  |
| Ends loop                      | Continues loop                 |

---

# Real-Time Example

Suppose we want to print numbers from:

```text
1 to 10
```

But skip:

```text
5
```

Program:

```java
for(int i=1;i<=10;i++){

    if(i==5){

        continue;

    }

    System.out.println(i);

}
```

Output:

```text
1 2 3 4 6 7 8 9 10
```

---

# Why Do We Use Continue?

Continue is useful when:

* Some values are not required.
* Invalid inputs should be ignored.
* Particular records should be skipped.
* Processing should continue without stopping the loop.

---

# Advantages of Continue Statement

* Improves readability.
* Avoids unnecessary nested if statements.
* Skips unwanted values easily.
* Makes loops cleaner.
* Improves program logic.

---

# Important Points

1. continue is a:

```text
Jump Statement
```

2. It does not terminate the loop.

3. It skips:

```text
Only the current iteration.
```

4. It can be used with:

* for loop
* while loop
* do-while loop

5. Execution continues with:

```text
Next iteration.
```

---

# Summary

This program demonstrates:

* Continue Statement
* Loop Iteration Skipping
* Continue with For Loop
* Continue with While Loop
* Continue with Do-While Loop
* Break vs Continue
* Execution Flow
* Real-Time Examples

The Continue Statement is an important jump statement in Java and is frequently asked in Core Java interviews.
