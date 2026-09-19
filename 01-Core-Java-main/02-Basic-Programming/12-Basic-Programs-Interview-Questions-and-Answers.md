# Basic Programs Interview Questions and Answers

This document contains the most frequently asked interview questions from Java Basic Programs including Hello World, Escape Sequences, Sum of Integers, Square of Integer, Even Odd, Greatest of Three Numbers, String Concatenation, Basic Calculator and Scanner Class.

---

## Hello World Program

### Q1. What is the simplest Java program?

**Answer:**

The simplest Java program is the **Hello World** program which prints a message on the console.

---

### Q2. Which method is the entry point of a Java program?

**Answer:**

```java
public static void main(String[] args)
```

JVM always starts execution from the `main()` method.

---

### Q3. What does System.out.println() do?

**Answer:**

`System.out.println()` prints the specified text and moves the cursor to the next line.

Example:

```java
System.out.println("Hello World");
```

Output:

```text
Hello World
```

---

### Q4. Difference between print() and println()?

| print()                            | println()                     |
| ---------------------------------- | ----------------------------- |
| Prints without moving to next line | Prints and moves to next line |
| Cursor remains on same line        | Cursor moves to next line     |

Example:

```java
System.out.print("Java");
System.out.print("Python");
```

Output:

```text
JavaPython
```

---

```java
System.out.println("Java");
System.out.println("Python");
```

Output:

```text
Java
Python
```

---

### Q5. What is System in Java?

**Answer:**

`System` is a predefined final class available in the `java.lang` package.

It provides:

* Standard Input
* Standard Output
* Error Output
* System properties

---

### Q6. What is out?

**Answer:**

`out` is a static object of the `PrintStream` class.

It is used to display output on the console.

Example:

```java
System.out.println("Java");
```

---

### Q7. Why is main() static?

**Answer:**

Because JVM calls `main()` directly without creating an object.

---

### Q8. What does void mean?

**Answer:**

`void` means the method does not return any value.

---

### Q9. Why is String[] args used?

**Answer:**

It stores command-line arguments passed to the Java program.

---

### Q10. Can we write:

```java
public static void main(String args[])
```

**Answer:**

Yes.

Both are valid:

```java
String[] args
```

and

```java
String args[]
```

---

## Sum of Integers

### Q11. How do you add two numbers in Java?

**Answer:**

Using the `+` operator.

Example:

```java
int sum = a + b;
```

---

### Q12. Which operator is used for addition?

**Answer:**

```text
+
```

Arithmetic Addition Operator.

---

### Q13. What is a variable?

**Answer:**

A variable is a named memory location used to store data.

Example:

```java
int age = 25;
```

---

### Q14. What is Initialization?

**Answer:**

Assigning a value to a variable.

Example:

```java
int num = 10;
```

---

### Q15. What is an Integer?

**Answer:**

An integer is a whole number stored using:

```java
int
```

Example:

```java
int marks = 95;
```

---

## Square of Integer

### Q16. How do you find the square of a number?

**Answer:**

```java
number * number
```

Example:

```java
int square = n * n;
```

---

### Q17. Can Math.pow() be used to find square?

**Answer:**

Yes.

Example:

```java
Math.pow(5,2);
```

Output:

```text
25.0
```

---

### Q18. What is the output of:

```java
5 * 5
```

**Answer:**

```text
25
```

---

## Even Odd Program

### Q19. How do you check whether a number is even or odd?

**Answer:**

Using Modulus Operator `%`

Example:

```java
number % 2 == 0
```

If true:

```text
Even Number
```

Else:

```text
Odd Number
```

---

### Q20. What does % operator do?

**Answer:**

Returns the remainder after division.

Example:

```text
10 % 2 = 0

11 % 2 = 1
```

---

## Greatest of Three Numbers

### Q21. Which statement is used to find the greatest among three numbers?

**Answer:**

```text
if - else if - else ladder
```

---

### Q22. Which operators are used for comparison?

**Answer:**

| Operator | Meaning                  |
| -------- | ------------------------ |
| >        | Greater Than             |
| <        | Less Than                |
| >=       | Greater Than or Equal To |
| <=       | Less Than or Equal To    |
| ==       | Equal To                 |
| !=       | Not Equal To             |

---

### Q23. What does && mean?

**Answer:**

Logical AND Operator.

It returns:

```text
true
```

only when both conditions are true.

Example:

```java
num1 > num2 && num1 > num3
```

---

## Escape Sequences

### Q24. What is an escape sequence?

**Answer:**

Escape sequences are special characters beginning with:

```text
\
```

They are used inside Strings.

Examples:

| Escape Sequence | Meaning      |
| --------------- | ------------ |
| \n              | New Line     |
| \t              | Tab          |
| \b              | Backspace    |
| "               | Double Quote |
| \               | Backslash    |

---

### Q25. What does \n do?

**Answer:**

Moves the cursor to the next line.

Example:

```java
System.out.println("Java\nPython");
```

Output:

```text
Java
Python
```

---

### Q26. What does \t do?

**Answer:**

Creates horizontal tab spacing.

Example:

```java
System.out.println("Java\tPython");
```

Output:

```text
Java    Python
```

---

## String Concatenation

### Q27. What is String Concatenation?

**Answer:**

Joining two Strings using:

```text
+
```

Example:

```java
"Java" + "Programming"
```

Output:

```text
JavaProgramming
```

---

### Q28. What is the output?

```java
System.out.println("Result: " + 20 + 30);
```

**Answer:**

```text
Result: 2030
```

Because Java performs String Concatenation from left to right.

---

### Q29. What is the output?

```java
System.out.println("Result: " + (20 + 30));
```

**Answer:**

```text
Result: 50
```

Because parentheses execute first.

---

### Q30. Why are parentheses used?

**Answer:**

To perform arithmetic calculation before concatenation.

Example:

```java
(num1 + num2)
```

---

## Basic Calculator

### Q31. Which operators are used in Calculator programs?

**Answer:**

| Operator | Meaning        |
| -------- | -------------- |
| +        | Addition       |
| -        | Subtraction    |
| *        | Multiplication |
| /        | Division       |
| %        | Modulus        |

---

### Q32. What is Integer Division?

**Answer:**

Division between two integers returns an integer value.

Example:

```text
10 / 3 = 3
```

Decimal part is discarded.

---

### Q33. What is Modulus Operation?

**Answer:**

Returns remainder after division.

Example:

```text
10 % 3 = 1
```

---

## Scanner Questions

### Q34. Which package contains Scanner?

**Answer:**

```java
java.util.Scanner
```

---

### Q35. How do you create Scanner object?

**Answer:**

```java
Scanner sc = new Scanner(System.in);
```

---

### Q36. Which method reads integer input?

**Answer:**

```java
nextInt()
```

Example:

```java
int num = sc.nextInt();
```

---

### Q37. Which method reads String input?

**Answer:**

```java
nextLine()
```

Example:

```java
String name = sc.nextLine();
```

---

### Q38. Why should Scanner be closed?

**Answer:**

To:

* Release system resources.
* Prevent resource leaks.
* Improve application performance.

Example:

```java
sc.close();
```

---

## General Questions

### Q39. What is Hard Coding?

**Answer:**

Values are directly written inside the source code.

Example:

```java
int a = 10;
```

---

### Q40. What is Soft Coding?

**Answer:**

Values are taken from the user during runtime.

Example:

```java
Scanner sc = new Scanner(System.in);

int a = sc.nextInt();
```

---

### Q41. Which Basic Programs are frequently asked in interviews?

**Answer:**

* Hello World
* Escape Sequences
* Sum of Integers
* Square of Integer
* Even Odd
* Greatest of Three Numbers
* Calculator Program
* String Concatenation
* Palindrome
* Arrays
* Strings
* Factorial
* Fibonacci Series

---

## Summary

This document covers the most important interview questions from Java Basic Programs including:

* Hello World
* Escape Sequences
* Sum of Integers
* Square of Integer
* Even Odd
* Greatest of Three Numbers
* String Concatenation
* Basic Calculator
* Scanner Class
* Hard Coding and Soft Coding

These questions are highly recommended for Java beginners and interview preparation.
