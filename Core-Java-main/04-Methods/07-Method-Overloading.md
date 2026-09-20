# Method Overloading in Java

## Objective

This program demonstrates **Method Overloading** in Java.

It explains:

* What is Method Overloading?
* Rules of Method Overloading
* Different ways of Overloading Methods
* Compile Time Polymorphism
* Method Signature
* Advantages of Method Overloading

Method Overloading is one of the most important features of Object-Oriented Programming in Java.

---

# What is Method Overloading?

## Definition

Method Overloading means creating **multiple methods with the same name in the same class but with different parameter lists**.

The methods may differ in:

1. Number of Parameters
2. Data Type of Parameters
3. Order of Parameters

Java identifies and calls the correct method based on the arguments passed during method calling.

---

# Syntax

```java
methodName(int a)

methodName(int a, int b)

methodName(double a, double b)

methodName(String name, int age)
```

All methods:

* Have same name
* Have different parameter lists

This is called:

```text
Method Overloading
```

---

## Program

```java
/*
 * Method Overloading Example
 */

public class MethodOverloading {

    // Main method - JVM starts execution here
    public static void main(String[] args) {

        // Call method with two integers
        add(10, 20);

        // Call method with three integers
        add(10, 20, 30);

        // Call method with two double values
        add(10.5, 20.5);

    }


    // Overloaded Method 1

    public static void add(int a, int b) {

        int sum = a + b;

        System.out.println("Sum of two integers: " + sum);

    }


    // Overloaded Method 2

    public static void add(int a, int b, int c) {

        int sum = a + b + c;

        System.out.println("Sum of three integers: " + sum);

    }


    // Overloaded Method 3

    public static void add(double a, double b) {

        double sum = a + b;

        System.out.println("Sum of two doubles: " + sum);

    }

}
```

---

## Output

```text
Sum of two integers: 30

Sum of three integers: 60

Sum of two doubles: 31.0
```

---

## Pseudocode

```text
START

Call add(10,20)

Call add(10,20,30)

Call add(10.5,20.5)

STOP


add(int a,int b)

sum = a+b

Display sum


add(int a,int b,int c)

sum = a+b+c

Display sum


add(double a,double b)

sum = a+b

Display sum
```

---

# Line-by-Line Explanation

### Line 1

```java
public class MethodOverloading
```

Explanation:

* `public` → Class is accessible from anywhere.
* `class` → Keyword used to create class.
* `MethodOverloading` → Name of the class.

---

### Line 2

```java
public static void main(String[] args)
```

This is:

```text
Entry Point of Java Program
```

JVM starts execution from this method.

---

### Line 3

```java
add(10,20);
```

Java searches:

```java
add(int,int)
```

because:

```text
10

20
```

are integers.

Output:

```text
Sum of two integers: 30
```

---

### Line 4

```java
add(10,20,30);
```

Java searches:

```java
add(int,int,int)
```

because:

```text
Three Integer Arguments
```

are passed.

Output:

```text
Sum of three integers: 60
```

---

### Line 5

```java
add(10.5,20.5);
```

Java searches:

```java
add(double,double)
```

because:

```text
10.5

20.5
```

are double values.

Output:

```text
Sum of two doubles: 31.0
```

---

# Overloaded Method 1

```java
public static void add(int a,int b)
```

Parameters:

```text
int

int
```

Purpose:

Adds two integers.

---

# Overloaded Method 2

```java
public static void add(int a,int b,int c)
```

Parameters:

```text
int

int

int
```

Purpose:

Adds three integers.

---

# Overloaded Method 3

```java
public static void add(double a,double b)
```

Parameters:

```text
double

double
```

Purpose:

Adds two decimal numbers.

---

# Ways to Perform Method Overloading

Method Overloading can be achieved by:

### 1. Changing Number of Parameters

Example:

```java
add(int a)

add(int a,int b)

add(int a,int b,int c)
```

---

### 2. Changing Data Type of Parameters

Example:

```java
add(int a,int b)

add(double a,double b)
```

---

### 3. Changing Order of Parameters

Example:

```java
display(int age,String name)

display(String name,int age)
```

---

# What Cannot Be Used for Overloading?

Changing only:

```java
Return Type
```

is NOT Method Overloading.

Example:

```java
int add(int a,int b)

double add(int a,int b)
```

This is:

```text
Invalid
```

Because parameter list is same.

---

# What is Method Signature?

Method Signature means:

```text
Method Name

+

Parameter List
```

Example:

```java
add(int,int)

add(double,double)
```

Different signatures.

Hence:

```text
Valid Overloading
```

---

# Compile Time Polymorphism

Method Overloading is called:

```text
Compile Time Polymorphism
```

because:

The compiler decides:

```text
Which Method to Call
```

during:

```text
Compilation Time
```

---

# Method Overloading vs Method Overriding

| Method Overloading        | Method Overriding      |
| ------------------------- | ---------------------- |
| Same Class                | Parent and Child Class |
| Same Method Name          | Same Method Name       |
| Different Parameters      | Same Parameters        |
| Compile Time Polymorphism | Runtime Polymorphism   |

---

# Advantages of Method Overloading

Method Overloading provides:

* Code Reusability
* Better Readability
* Easy Maintenance
* Flexibility
* Compile Time Polymorphism
* Same Method Name for Similar Operations

---

# Real Life Example

Example:

```text
Call()

Call(phoneNumber)

Call(phoneNumber,video)

Call(phoneNumber,audio)
```

Same operation:

```text
Call
```

Different parameters.

This is similar to:

```text
Method Overloading
```

---

# Important Rules

1. Method names must be same.

2. Parameter list must be different.

3. Return type alone cannot overload methods.

4. Methods may have different number of parameters.

5. Methods may have different parameter data types.

---

# Summary

This program demonstrates:

* Method Overloading
* Compile Time Polymorphism
* Method Signature
* Overloading by Number of Parameters
* Overloading by Data Type
* Overloading by Order of Parameters
* Advantages of Method Overloading
* Difference Between Overloading and Overriding

Method Overloading is one of the most frequently asked Core Java interview topics and is widely used to increase flexibility and readability of Java applications.
