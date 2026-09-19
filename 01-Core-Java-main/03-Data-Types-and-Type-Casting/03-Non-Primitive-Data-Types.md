# Non-Primitive Data Types in Java

## Objective

This program demonstrates the most commonly used **Non-Primitive Data Types** in Java.

The program explains:

* String
* Array
* Class Object
* Enum
* Reference Types
* Difference between Primitive and Non-Primitive Data Types

Non-Primitive Data Types are also called **Reference Types** because they store references (memory addresses) of objects rather than storing actual values directly.

---

## Program

```java
/*
 * Java Program Demonstrating Non-Primitive Data Types
 */

// Define public class
public class NonPrimitiveDataTypes {

    // Main method - JVM starts execution from here
    public static void main(String[] args) {

        // String example
        String sampleString = "Hello, Java Non-Primitive Types";

        // Array example
        int[] sampleArray = {10, 20, 30};

        // Object example
        Person samplePerson = new Person("Ayesha", 22);

        // Enum example
        Day sampleDay = Day.MONDAY;

        // Display heading
        System.out.println("Java Non-Primitive Data Types Example");

        System.out.println("-----------------------------------");

        // Print String value
        System.out.println("String value      : " + sampleString);

        // Print Array values
        System.out.print("Array values      : ");

        for (int value : sampleArray) {

            System.out.print(value + " ");

        }

        System.out.println();

        // Print object value
        System.out.println("Person object     : " + samplePerson);

        // Print enum value
        System.out.println("Enum value        : " + sampleDay);

        System.out.println();

        System.out.println("Note: String, arrays, classes and enums are reference types.");

        System.out.println("They store references to objects rather than values.");

    }

    // Nested Person class
    static class Person {

        String name;

        int age;

        Person(String name, int age) {

            this.name = name;

            this.age = age;

        }

        @Override

        public String toString() {

            return name + " (" + age + " years old)";

        }

    }

    // Enum example

    enum Day {

        MONDAY,

        TUESDAY,

        WEDNESDAY,

        THURSDAY,

        FRIDAY,

        SATURDAY,

        SUNDAY

    }

}
```

---

## Output

```text
Java Non-Primitive Data Types Example
-----------------------------------

String value      : Hello, Java Non-Primitive Types

Array values      : 10 20 30

Person object     : Ayesha (22 years old)

Enum value        : MONDAY


Note: String, arrays, classes and enums are reference types.

They store references to objects rather than values.
```

---

## Pseudocode

```text
START

Create String variable

Create Integer Array

Create Person object

Create Enum value

Display String

Display Array values

Display Object

Display Enum value

Display reference type information

STOP
```

---

# What are Non-Primitive Data Types?

Non-Primitive Data Types are:

```text
Reference Types
```

Because:

They store:

```text
Reference (Memory Address)
```

of an object rather than storing the actual value directly.

---

## Types of Non-Primitive Data Types

Java provides the following commonly used Non-Primitive Data Types:

1. String

2. Array

3. Class

4. Interface

5. Enum

---

# 1. String

String is used to store:

```text
Text or Sequence of Characters
```

Example:

```java
String name = "Java";
```

---

### Program Statement

```java
String sampleString = "Hello, Java Non-Primitive Types";
```

Explanation:

* `String` is a predefined class.
* It stores character sequences.
* String objects are immutable.

---

### Output

```text
Hello, Java Non-Primitive Types
```

---

# 2. Array

Array stores:

```text
Multiple values of same data type
```

Example:

```java
int[] numbers = {10,20,30};
```

---

### Program Statement

```java
int[] sampleArray = {10,20,30};
```

Explanation:

* `int[]` means integer array.
* Stores multiple integer values.
* Array size becomes fixed after creation.

---

### Array Output

```text
10 20 30
```

---

# Enhanced For Loop Used

Program:

```java
for(int value : sampleArray)
```

This is called:

```text
Enhanced For Loop

or

For Each Loop
```

Purpose:

Iterates through all array elements automatically.

---

# 3. Class Object

A Class is:

```text
Blueprint of an Object
```

Objects are created from classes.

---

### Program Statement

```java
Person samplePerson = new Person("Ayesha",22);
```

Explanation:

* `Person` → Class name.
* `samplePerson` → Object reference.
* `new` → Creates object.
* Constructor initializes values.

---

## Person Class

```java
static class Person
```

Contains:

```text
name

age
```

Fields.

---

## Constructor

```java
Person(String name,int age)
```

Purpose:

Initializes object variables.

---

### this Keyword

```java
this.name = name;

this.age = age;
```

Meaning:

Current object's variables are assigned values.

---

## toString() Method

```java
@Override

public String toString()
```

Purpose:

Returns object information in String format.

Output:

```text
Ayesha (22 years old)
```

Without toString():

```text
Person@1a2b3c
```

would be displayed.

---

# 4. Enum

Enum means:

```text
Enumeration
```

It stores:

```text
Fixed Set of Constants
```

---

### Program Statement

```java
Day sampleDay = Day.MONDAY;
```

Explanation:

* `Day` → Enum name.
* `MONDAY` → Enum constant.

---

## Enum Declaration

```java
enum Day{

MONDAY,

TUESDAY,

WEDNESDAY,

THURSDAY,

FRIDAY,

SATURDAY,

SUNDAY

}
```

---

### Output

```text
MONDAY
```

---

# Primitive vs Non Primitive Data Types

| Primitive            | Non Primitive              |
| -------------------- | -------------------------- |
| Stores actual values | Stores references          |
| Fixed memory size    | Dynamic memory             |
| Faster               | Slightly slower            |
| Cannot call methods  | Can call methods           |
| Predefined           | Predefined or User Defined |

---

### Example

Primitive:

```java
int age = 25;
```

Stores:

```text
25
```

directly.

---

Non Primitive:

```java
String name = "Java";
```

Stores:

```text
Reference

↓

"Java"
```

---

# Memory Representation

```text
Primitive

int age = 25

Memory:

age → 25


Non Primitive

String name = "Java"

Memory:

name → Reference → "Java"
```

---

# Why are Non Primitive Data Types Important?

Because they:

* Store large and complex data.
* Support Object Oriented Programming.
* Allow methods and objects.
* Enable code reusability.
* Provide flexibility.

---

# Summary

This program demonstrates:

* String Data Type
* Array Data Type
* Class Object
* Enum
* Enhanced For Loop
* Constructor
* this keyword
* toString() method
* Reference Types
* Primitive vs Non Primitive

Non-Primitive Data Types are one of the most important concepts in Core Java because Object Oriented Programming is completely based on them.
