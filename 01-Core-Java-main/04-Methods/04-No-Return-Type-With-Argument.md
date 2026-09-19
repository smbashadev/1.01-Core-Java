# No Return Type With Argument Method in Java

## Objective

This program demonstrates a **No Return Type With Argument Method** in Java.

This type of method:

* Does not return any value.
* Accepts one or more arguments (parameters).
* Uses `void` as the return type.
* Processes the values passed during method calling.

This is one of the most commonly used User Defined Method types in Java.

---

# Definition

A method with:

* **No Return Type** → Does not send back any value.
* **With Argument** → Receives one or more input values from the caller.

Syntax:

```java
void methodName(dataType parameter){

    // Statements

}
```

---

## Program

```java
/*
 * No Return Type With Argument Method Example
 */

public class Method2 {

    // Main method - JVM starts execution here
    public static void main(String[] args) {

        // Calling the method and passing an argument
        displayMessage("Java");

    }

    // Method with no return type and one argument
    public static void displayMessage(String name) {

        // Display message using argument
        System.out.println("Hello " + name);

    }

}
```

---

## Output

```text
Hello Java
```

---

## Pseudocode

```text
START

Call displayMessage("Java")

STOP


displayMessage(name)

Display "Hello " + name

END
```

---

# Line-by-Line Explanation

### Line 1

```java
public class Method2
```

Explanation:

* `public` → Class can be accessed from anywhere.
* `class` → Keyword used to create a class.
* `Method2` → Name of the class.

---

### Line 2

```java
public static void main(String[] args)
```

Explanation:

* `public` → Accessible from anywhere.
* `static` → JVM can call the method without creating an object.
* `void` → No return value.
* `main` → Entry point of Java program.
* `String[] args` → Stores command line arguments.

---

### Line 3

```java
displayMessage("Java");
```

Explanation:

This statement:

* Calls the method.
* Passes `"Java"` as an argument.

Here:

```text
Argument = "Java"
```

Control transfers from:

```text
main()

↓

displayMessage("Java")

↓

Execute statements

↓

Return to main()
```

---

### Line 4

```java
public static void displayMessage(String name)
```

Explanation:

This is a:

* User Defined Method
* No Return Type Method
* With Argument Method

Here:

```text
String name
```

is called:

```text
Parameter
```

The parameter receives:

```text
"Java"
```

which is passed from the method call.

---

### Line 5

```java
System.out.println("Hello " + name);
```

Explanation:

This statement joins:

```text
"Hello "

+

"Java"
```

Result:

```text
Hello Java
```

This is called:

```text
String Concatenation
```

---

# What is an Argument?

An Argument is:

```text
The actual value passed to a method during method calling.
```

Example:

```java
displayMessage("Java");
```

Here:

```text
"Java"
```

is the Argument.

---

# What is a Parameter?

A Parameter is:

```text
A variable declared inside the method definition to receive values.
```

Example:

```java
displayMessage(String name)
```

Here:

```text
name
```

is the Parameter.

---

# Parameter vs Argument

| Parameter          | Argument                  |
| ------------------ | ------------------------- |
| Declared in method | Passed during method call |
| Receives data      | Sends data                |
| Variable           | Actual Value              |

Example:

```java
displayMessage(String name)

displayMessage("Java")
```

Parameter:

```text
name
```

Argument:

```text
Java
```

---

# Why is Return Type void?

The method:

```java
displayMessage()
```

only displays output.

It does not return anything.

Therefore:

```java
void
```

is used.

---

# Why Do We Pass Arguments?

Arguments make methods:

* Flexible
* Reusable
* Dynamic

Without arguments:

```java
displayJava();
```

Only prints:

```text
Java
```

With arguments:

```java
displayMessage("Java");

displayMessage("Python");

displayMessage("Oracle SQL");
```

The same method works for different values.

---

# Method Execution Flow

```text
main()

↓

displayMessage("Java")

↓

name = "Java"

↓

Print Hello Java

↓

Return to main()
```

---

# Advantages of No Return Type With Argument Method

* Accepts different input values.
* Reduces code duplication.
* Reusable for multiple values.
* Improves flexibility.
* Easier to maintain.

---

# Real Life Example

Example:

```text
sendMessage("Welcome")

sendMessage("Congratulations")

sendMessage("Good Morning")
```

Same method:

```text
sendMessage()
```

Different arguments.

---

# Important Points

1. Uses:

```java
void
```

2. Accepts parameters.

3. Does not return any value.

4. Executes only when called.

5. Parameters receive values from arguments.

---

# Summary

This program demonstrates:

* No Return Type With Argument Method
* Method Declaration
* Method Calling
* Parameters
* Arguments
* String Concatenation
* void Return Type
* Execution Flow of Methods
* Reusability of Methods

This method type is widely used in Java applications because it accepts input from users or other methods while performing operations without returning any value.
