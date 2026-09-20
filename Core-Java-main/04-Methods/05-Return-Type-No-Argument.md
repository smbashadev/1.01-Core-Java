# Return Type No Argument Method in Java

## Objective

This program demonstrates a **Return Type No Argument Method** in Java.

This type of method:

* Returns a value to the caller.
* Does not accept any arguments (parameters).
* Uses a return statement to send the result back.
* Can return primitive or non-primitive data types.

This method type is widely used when a method needs to calculate a result and provide it to another method.

---

# Definition

A method with:

* **Return Type** → Sends back a value to the calling method.
* **No Arguments** → Does not receive any input values.

Syntax:

```java
returnType methodName(){

    // Statements

    return value;

}
```

---

## Program

```java
/*
 * Return Type No Argument Method Example
 */

public class Method3 {

    // Main method - JVM starts execution here
    public static void main(String[] args) {

        // Call the method and store returned value
        int result = getNumber();

        // Display the returned value
        System.out.println(result);

    }

    // Method with return type and no arguments
    public static int getNumber() {

        // Declare first integer
        int a = 10;

        // Declare second integer
        int b = 20;

        // Calculate sum
        int sum = a + b;

        // Return the result to the caller
        return sum;

    }

}
```

---

## Output

```text
30
```

---

## Pseudocode

```text
START

result = getNumber()

Display result

STOP


getNumber()

a = 10

b = 20

sum = a + b

return sum

END
```

---

# Line-by-Line Explanation

### Line 1

```java
public class Method3
```

Explanation:

* `public` → Class can be accessed from anywhere.
* `class` → Keyword used to create a class.
* `Method3` → Name of the class.

---

### Line 2

```java
public static void main(String[] args)
```

Explanation:

* `public` → Accessible from anywhere.
* `static` → JVM can call the method without creating an object.
* `void` → Does not return anything.
* `main` → Entry point of Java application.
* `String[] args` → Stores command line arguments.

---

### Line 3

```java
int result = getNumber();
```

Explanation:

This statement:

1. Calls:

```java
getNumber();
```

2. Receives the returned value.

3. Stores the returned value into:

```java
result
```

Returned value:

```text
30
```

---

### Line 4

```java
System.out.println(result);
```

Displays:

```text
30
```

on the console.

---

### Line 5

```java
public static int getNumber()
```

Explanation:

This method:

* Returns an integer value.
* Does not take any arguments.
* Uses:

```java
int
```

as return type.

---

### Line 6

```java
int a = 10;
```

Creates:

```text
a = 10
```

---

### Line 7

```java
int b = 20;
```

Creates:

```text
b = 20
```

---

### Line 8

```java
int sum = a + b;
```

Performs:

```text
10 + 20 = 30
```

Stores:

```text
sum = 30
```

---

### Line 9

```java
return sum;
```

Explanation:

The `return` keyword sends:

```text
30
```

back to:

```text
main()
```

Control flow:

```text
main()

↓

getNumber()

↓

Calculate Sum

↓

return 30

↓

main()
```

---

# What is Return Type?

Return Type specifies:

```text
What value the method returns to the caller.
```

Examples:

```java
int

double

String

char

boolean
```

---

## Example

```java
public static int getAge(){

return 25;

}
```

Return Type:

```text
int
```

Because:

```text
25
```

is an integer value.

---

# What is Return Statement?

The `return` statement:

* Ends method execution.
* Sends a value back to the caller.
* Must match the return type.

Syntax:

```java
return value;
```

---

## Example

```java
return sum;
```

Sends:

```text
sum
```

to:

```text
main()
```

---

# Why are there No Arguments?

Because:

```java
int a = 10;

int b = 20;
```

are declared inside the method itself.

No input is received from outside.

Therefore:

```text
No Parameters

No Arguments
```

---

# Method Execution Flow

```text
main()

↓

getNumber()

↓

a = 10

↓

b = 20

↓

sum = 30

↓

return 30

↓

main()

↓

Display Result
```

---

# Advantages of Return Type No Argument Methods

* Returns calculated results.
* Improves code reusability.
* Keeps logic separate from output.
* Easy to test and debug.
* Can be used in expressions.

---

# Real Life Example

Example:

```text
getCurrentYear()

↓

2026
```

The method:

* Does not take input.
* Returns the year.

---

# Important Points

1. Uses a Return Type.

Example:

```java
int

double

String
```

2. Must use:

```java
return;
```

or

```java
return value;
```

3. No parameters.

4. Caller receives the returned value.

---

# Difference Between void and Return Type

| void               | Return Type               |
| ------------------ | ------------------------- |
| Returns nothing    | Returns a value           |
| No return required | return statement required |
| Used for actions   | Used for calculations     |

---

# Summary

This program demonstrates:

* Return Type No Argument Method
* Method Declaration
* Method Calling
* Return Statement
* int Return Type
* Method Execution Flow
* Returning Values to Caller

This method type is very important in Java because it allows methods to perform computations and return results without taking any external input.
