# Return Type With Argument Method in Java

## Objective

This program demonstrates a **Return Type With Argument Method** in Java.

This type of method:

* Accepts one or more arguments (parameters).
* Performs operations using the received values.
* Returns a value to the calling method.
* Uses the `return` statement to send the result back.

This is the **most commonly used method type** in real-world Java applications.

---

# Definition

A method with:

* **Return Type** → Sends back a value to the caller.
* **With Arguments** → Receives input values from the caller.

Syntax:

```java
returnType methodName(dataType parameter1, dataType parameter2){

    // Statements

    return value;

}
```

---

## Program

```java
/*
 * Return Type With Argument Method Example
 */

public class Method4 {

    // Main method - JVM starts execution here
    public static void main(String[] args) {

        // Call the method and store returned value
        int result = addNumbers(10, 20);

        // Display the result
        System.out.println(result);

    }

    // Method with return type and arguments
    public static int addNumbers(int a, int b) {

        // Calculate the sum
        int sum = a + b;

        // Return the result
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

result = addNumbers(10,20)

Display result

STOP


addNumbers(a,b)

sum = a + b

return sum

END
```

---

# Line-by-Line Explanation

### Line 1

```java
public class Method4
```

Explanation:

* `public` → Class is accessible from anywhere.
* `class` → Keyword used to create a class.
* `Method4` → Name of the class.

---

### Line 2

```java
public static void main(String[] args)
```

Explanation:

* `public` → Accessible from anywhere.
* `static` → JVM calls it without creating an object.
* `void` → Does not return anything.
* `main` → Entry point of Java program.
* `String[] args` → Stores command line arguments.

---

### Line 3

```java
int result = addNumbers(10,20);
```

Explanation:

This statement:

1. Calls:

```java
addNumbers(10,20)
```

2. Passes:

```text
10

20
```

as arguments.

3. Receives:

```text
30
```

from the method.

4. Stores it in:

```java
result
```

---

### Line 4

```java
public static int addNumbers(int a,int b)
```

Explanation:

This method:

* Returns an integer value.
* Accepts two parameters.
* Adds two numbers.
* Returns the result.

Here:

```text
a

b
```

are called:

```text
Parameters
```

---

### Line 5

```java
int sum = a + b;
```

Performs:

```text
10 + 20
```

Result:

```text
30
```

Stores:

```text
sum = 30
```

---

### Line 6

```java
return sum;
```

Explanation:

The return statement sends:

```text
30
```

back to:

```text
main()
```

Control Flow:

```text
main()

↓

addNumbers(10,20)

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

# What is Return Type?

Return Type specifies:

```text
What value the method sends back to the caller.
```

Examples:

```java
int

double

float

String

boolean
```

---

## Example

```java
public static int square(int n){

return n*n;

}
```

Return Type:

```text
int
```

because:

```text
n*n
```

returns an integer.

---

# What are Parameters?

Parameters are:

```text
Variables declared in method definition.
```

Example:

```java
addNumbers(int a,int b)
```

Parameters:

```text
a

b
```

---

# What are Arguments?

Arguments are:

```text
Actual values passed to the method.
```

Example:

```java
addNumbers(10,20)
```

Arguments:

```text
10

20
```

---

# Parameter vs Argument

| Parameter          | Argument                  |
| ------------------ | ------------------------- |
| Declared in Method | Passed during Method Call |
| Variables          | Actual Values             |
| Receives Data      | Sends Data                |

Example:

```java
addNumbers(int a,int b)

addNumbers(10,20)
```

Parameters:

```text
a

b
```

Arguments:

```text
10

20
```

---

# Why is Return Type int?

Because:

```java
int sum = a+b;
```

returns:

```text
30
```

which is an integer value.

Therefore:

```java
int
```

is used as return type.

---

# Why is This Method Important?

This method:

* Accepts input.
* Processes the input.
* Returns output.

It follows:

```text
Input

↓

Process

↓

Output
```

This is the foundation of:

* Banking Applications
* E-Commerce Applications
* Spring Boot Applications
* REST APIs
* Enterprise Software

---

# Method Execution Flow

```text
main()

↓

addNumbers(10,20)

↓

a=10

b=20

↓

sum=30

↓

return 30

↓

main()

↓

Display 30
```

---

# Advantages of Return Type With Argument Method

* Reusable
* Dynamic
* Accepts different inputs
* Returns results
* Reduces code duplication
* Most suitable for real-world applications

---

# Real Life Example

```text
calculateSalary(employeeId)

↓

Calculate Salary

↓

Return Salary
```

Input:

```text
employeeId
```

Output:

```text
salary
```

---

# Important Points

1. Uses Return Type.

2. Accepts Parameters.

3. Uses return statement.

4. Can accept multiple arguments.

5. Most frequently used method type in Java.

---

# Comparison of Four Types of Methods

| Method Type                  | Return Value | Arguments |
| ---------------------------- | ------------ | --------- |
| No Return Type No Argument   | No           | No        |
| No Return Type With Argument | No           | Yes       |
| Return Type No Argument      | Yes          | No        |
| Return Type With Argument    | Yes          | Yes       |

---

# Summary

This program demonstrates:

* Return Type With Argument Method
* Method Declaration
* Method Calling
* Parameters
* Arguments
* Return Statement
* int Return Type
* Method Execution Flow
* Input → Process → Output Concept

Return Type With Argument Method is the most powerful and widely used method type in Java because it accepts input values, performs operations and returns the result to the caller.
