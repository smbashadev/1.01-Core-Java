# Types of Methods in Java

## Objective

This document explains:

* Types of Methods in Java
* No Return Type No Argument Method
* No Return Type With Argument Method
* Return Type No Argument Method
* Return Type With Argument Method
* Difference between Return Type and Void
* Difference between Arguments and Parameters

Methods in Java are classified based on two factors:

1. Return Type
2. Arguments (Parameters)

---

# Types of Methods in Java

Based on syntax, a method in Java can be classified into the following four types:

```text
Methods
│
├── 1. No Return Type No Argument
│
├── 2. No Return Type With Argument
│
├── 3. Return Type No Argument
│
└── 4. Return Type With Argument
```

---

# 1. No Return Type No Argument

## Definition

This type of method:

* Does not return any value.
* Does not take any parameters.
* Uses `void` as return type.

---

## Syntax

```java
void display(){

    // Statements

}
```

---

## Example

```java
void greet(){

System.out.println("Welcome to Java");

}
```

---

## Method Call

```java
greet();
```

---

## Characteristics

* No return statement required.
* No parameters.
* Executes only when called.
* Used for displaying output or performing simple operations.

---

# 2. No Return Type With Argument

## Definition

This type of method:

* Does not return any value.
* Accepts one or more parameters.
* Uses `void` as return type.

---

## Syntax

```java
void show(int a){

    // Statements

}
```

---

## Example

```java
void displayName(String name){

System.out.println(name);

}
```

---

## Method Call

```java
displayName("Java");
```

---

## Characteristics

* No return value.
* Accepts parameters.
* Used to process input values.

---

# 3. Return Type No Argument

## Definition

This type of method:

* Returns a value.
* Does not take any parameters.
* Uses a return statement.

---

## Syntax

```java
int getNumber(){

return value;

}
```

---

## Example

```java
int getAge(){

return 25;

}
```

---

## Method Call

```java
int age = getAge();
```

---

## Characteristics

* Returns a value.
* No parameters.
* Return statement is mandatory.

---

# 4. Return Type With Argument

## Definition

This type of method:

* Returns a value.
* Accepts one or more parameters.
* Uses return statement.

---

## Syntax

```java
int add(int a,int b){

return a+b;

}
```

---

## Example

```java
int multiply(int x,int y){

return x*y;

}
```

---

## Method Call

```java
int result = multiply(10,20);
```

---

## Characteristics

* Accepts parameters.
* Returns a value.
* Most frequently used method type in Java applications.

---

# What is Return Type?

Return Type specifies:

```text
What value the method sends back to the calling method.
```

Examples:

```java
int

double

String

boolean
```

---

## Example

```java
int square(){

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

is an integer.

---

# What is void?

`void` means:

```text
The method does not return any value.
```

Example:

```java
void display(){

System.out.println("Java");

}
```

This method:

* Displays output.
* Does not return anything.

---

# What are Arguments?

Arguments are:

```text
Values passed to a method.
```

Example:

```java
add(10,20);
```

Here:

```text
10

20
```

are arguments.

---

# What are Parameters?

Parameters are:

```text
Variables declared inside method definition.
```

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

# Difference Between Arguments and Parameters

| Parameters         | Arguments                 |
| ------------------ | ------------------------- |
| Declared in Method | Passed during Method Call |
| Variables          | Actual Values             |
| Receive Data       | Send Data                 |

Example:

```java
int add(int a,int b){

return a+b;

}


add(10,20);
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

# Difference Between Return Type and void

| Return Type               | void                         |
| ------------------------- | ---------------------------- |
| Returns value             | Returns nothing              |
| Requires return statement | No return statement required |
| Examples: int, double     | Example: void                |

---

# Comparison of All Four Types

| Method Type                  | Return Value | Arguments |
| ---------------------------- | ------------ | --------- |
| No Return Type No Argument   | No           | No        |
| No Return Type With Argument | No           | Yes       |
| Return Type No Argument      | Yes          | No        |
| Return Type With Argument    | Yes          | Yes       |

---

# Which Method Type is Most Commonly Used?

```text
Return Type With Argument
```

Reason:

* Accepts input.
* Processes data.
* Returns result.
* Used extensively in real-world Java applications.

---

# Summary

This document explained:

* Types of Methods in Java
* No Return Type No Argument
* No Return Type With Argument
* Return Type No Argument
* Return Type With Argument
* Return Type
* void Keyword
* Parameters
* Arguments
* Comparison of All Method Types

Understanding these four method types is essential because almost every Java application uses them extensively.
