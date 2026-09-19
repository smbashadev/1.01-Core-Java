# Methods in Java


Methods:
A method is a set of instructions written to perform a specific task.

General example of a method in daily life:

Example 1: Method to prepare Maggi

Step 1: Boil the water

Step 2: Add Maggi and other ingredients

Step 3: Stir for a while

Step 4: Serve and eat

Example 2: Method for getting a job
1. Get skilled
2. Apply for the interview
3. Give the interview
4. Crack the interview
5. Accept the offer letter

Methods are of two types:
1. Predefined methods
2. User-defined methods

1. Predefined methods: These methods are already coded by the Java team. Whenever we want to use their functionality, we can simply call them.
Example: println(); print(); equals(); toLowerCase(); etc.

2. User-defined methods: These methods are defined by the programmer according to their requirements. Whenever we want to use a user-defined method, we must call it.

Note:
Every method in Java must be explicitly called in the program except for the main() method, whose signature is:
public static void main(String[] args)
The main() method is automatically called by the JVM when the program starts.

Syntax of a method:
return_type method_name(arguments/parameters) {
    set of statements
}
# Methods in Java

## Objective

This document explains:

* What is a Method?
* Real Life Examples of Methods
* Types of Methods in Java
* Predefined Methods
* User Defined Methods
* Importance of main() Method
* Syntax of a Method
* Advantages of Methods

Methods are one of the most important features of Java because they help organize code into reusable and manageable blocks.

---

# What is a Method?

## Definition

A Method is a set of instructions written to perform a specific task.

A method contains a group of statements that are executed whenever the method is called.

In simple words:

```text
Method = A reusable block of code that performs a specific task.
```

---

# Real Life Examples of Methods

Methods are not only used in programming.

We perform methods in our daily life as well.

---

## Example 1: Method to Prepare Maggi

```text
Step 1 : Boil the water

Step 2 : Add Maggi and other ingredients

Step 3 : Stir for a while

Step 4 : Serve and eat
```

Here,

Preparing Maggi is a method.

Each step is an instruction inside the method.

---

## Example 2: Method for Getting a Job

```text
Step 1 : Get skilled

Step 2 : Apply for interviews

Step 3 : Attend interviews

Step 4 : Crack the interview

Step 5 : Accept the offer letter
```

This is also a sequence of instructions.

Hence it can be considered as a method.

---

# Why Do We Use Methods?

Methods help to:

* Reuse code.
* Reduce code duplication.
* Improve readability.
* Simplify debugging.
* Improve maintainability.
* Divide large programs into smaller modules.

---

# Types of Methods in Java

Java provides two types of methods:

```text
Methods
│
├── Predefined Methods
│
└── User Defined Methods
```

---

# 1. Predefined Methods

## Definition

Predefined Methods are methods already written by the Java Development Team.

Programmers can directly use them by calling the methods.

No need to write their implementation.

---

## Examples

```java
System.out.println();

System.out.print();

equals();

toLowerCase();

toUpperCase();

length();
```

---

### Example

```java
System.out.println("Hello World");
```

Explanation:

* `System` → Predefined class.
* `out` → Static object.
* `println()` → Predefined method used to display output.

---

# 2. User Defined Methods

## Definition

User Defined Methods are methods created by the programmer according to the application requirements.

The programmer:

* Defines the method.
* Writes the logic.
* Calls the method whenever needed.

---

## Example

```java
public static void greet(){

System.out.println("Welcome to Java");

}
```

Calling the method:

```java
greet();
```

Output:

```text
Welcome to Java
```

---

# Important Note

Every method in Java must be called explicitly.

Example:

```java
calculate();

display();

showData();
```

These methods execute only when called.

---

# Exception: main() Method

There is one exception.

```java
public static void main(String[] args)
```

This method is:

```text
Automatically called by JVM.
```

---

## Why main() Method is Special?

Because:

* JVM searches for the main() method.
* Execution begins from main().
* Without main(), a Java application cannot start.

Hence:

```text
main() is the Entry Point of Java Program.
```

---

# Syntax of a Method

```java
return_type method_name(arguments){

    // Statements

}
```

---

## Example

```java
public static void display(){

System.out.println("Java Methods");

}
```

---

# Components of a Method

```java
public static int add(int a,int b){

return a+b;

}
```

This method contains:

| Component   | Meaning          |
| ----------- | ---------------- |
| public      | Access Modifier  |
| static      | Belongs to class |
| int         | Return Type      |
| add         | Method Name      |
| int a,int b | Parameters       |
| return a+b  | Return Statement |

---

# Return Type

The Return Type specifies:

```text
What value the method returns.
```

Examples:

```java
int

double

String

boolean

void
```

---

### void Return Type

```java
void display(){

}
```

Means:

```text
This method does not return anything.
```

---

# Method Name

The Method Name:

* Identifies the method.
* Used to call the method.

Example:

```java
display();

calculate();

showResult();
```

---

# Parameters / Arguments

Parameters are variables used to receive values.

Example:

```java
int add(int a,int b)
```

Here:

```text
a

b
```

are parameters.

---

# Return Statement

The return statement sends a value back to the calling method.

Example:

```java
return a+b;
```

---

# Method Calling

A method is executed only when it is called.

Example:

```java
display();
```

If not called:

```text
Method will not execute.
```

---

# Predefined vs User Defined Methods

| Predefined Methods            | User Defined Methods       |
| ----------------------------- | -------------------------- |
| Already written by Java       | Written by Programmer      |
| Directly used                 | Must be created            |
| No implementation required    | Programmer writes logic    |
| Examples: println(), equals() | Examples: add(), display() |

---

# Advantages of Methods

Methods provide:

* Code Reusability
* Better Readability
* Easier Testing
* Reduced Code Duplication
* Easier Maintenance
* Modular Programming

---

# Summary

This document explained:

* What is a Method
* Real Life Examples
* Predefined Methods
* User Defined Methods
* main() Method
* Method Syntax
* Components of a Method
* Return Type
* Parameters
* Return Statement
* Advantages of Methods

Methods are one of the most important concepts in Java because they allow programmers to write reusable, modular and maintainable code.
