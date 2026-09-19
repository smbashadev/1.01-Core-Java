# Data Types in Java

## Objective

This document explains:

* What are Data Types?
* What is a Variable?
* Categories of Data Types in Java
* Primitive Data Types
* Non-Primitive Data Types
* Memory Size of Primitive Data Types

Understanding data types is essential because every variable in Java must have a specific data type that determines the kind of values it can store.

---

# What are Data Types?

**Definition:**

A Data Type can be defined as classification that signifies the type of value a variable can hold.

In simple words:

Data types classify the kind of values a variable can hold.

Examples:

* Integer values → `byte`, `short`, `int`, `long`
* Decimal values → `float`, `double`
* Characters → `char`
* True or False values → `boolean`
* Text → `String`

---

# What is a Variable?

**Definition:**

A variable is a name given to a memory location used to store a value.

It allows a program to:

* Store data
* Access data
* Modify data during execution

---

## Syntax of Variable Declaration

```java
dataType variableName;
```

Example:

```java
int age;

String name;

double salary;
```

---

## Variable Initialization

Assigning a value to a variable is called **Initialization**.

Example:

```java
int age = 25;

String name = "Java";

double salary = 50000.50;
```

---

# Categories of Data Types in Java

Java Data Types are divided into two categories:

```text
Data Types
│
├── Primitive Data Types
│
└── Non Primitive Data Types
```

1. Primitive Data Types

2. Non Primitive Data Types

---

# 1. Primitive Data Types

Primitive data types are predefined by Java.

They store actual values directly in memory.

There are **8 Primitive Data Types**.

---

## Primitive Data Types Table

| Data Type | Size          | Bits            | Description                          |
| --------- | ------------- | --------------- | ------------------------------------ |
| byte      | 1 Byte        | 8 Bits          | Stores small integers                |
| short     | 2 Bytes       | 16 Bits         | Stores short integers                |
| int       | 4 Bytes       | 32 Bits         | Stores integer values                |
| long      | 8 Bytes       | 64 Bits         | Stores large integers                |
| float     | 4 Bytes       | 32 Bits         | Stores decimal values                |
| double    | 8 Bytes       | 64 Bits         | Stores high precision decimal values |
| char      | 2 Bytes       | 16 Bits         | Stores a single Unicode character    |
| boolean   | JVM dependent | 1 Bit (logical) | Stores true or false                 |

---

## byte

Size:

```text
1 Byte = 8 Bits
```

Example:

```java
byte age = 25;
```

---

## short

Size:

```text
2 Bytes = 16 Bits
```

Example:

```java
short marks = 500;
```

---

## int

Size:

```text
4 Bytes = 32 Bits
```

Example:

```java
int salary = 50000;
```

This is the most commonly used integer data type in Java.

---

## long

Size:

```text
8 Bytes = 64 Bits
```

Example:

```java
long population = 1400000000L;
```

Used for storing very large integer values.

---

## float

Size:

```text
4 Bytes = 32 Bits
```

Example:

```java
float price = 99.99f;
```

`f` suffix is mandatory.

---

## double

Size:

```text
8 Bytes = 64 Bits
```

Example:

```java
double pi = 3.14159265359;
```

More precise than float.

---

## char

Size:

```text
2 Bytes = 16 Bits
```

Stores:

```text
Unicode Characters

Range:

\u0000 to \uffff
```

Example:

```java
char grade = 'A';
```

---

## boolean

Stores:

```text
true

or

false
```

Example:

```java
boolean status = true;
```

Used in decision-making statements.

---

# Why Primitive Data Types are Called Primitive?

Because:

* They are predefined by Java.
* They store actual values directly.
* They are not objects.
* They are faster than reference types.

---

# 2. Non Primitive Data Types

Non Primitive Data Types are also called:

```text
Reference Data Types
```

Reason:

They store references (addresses) of objects rather than actual values.

---

## Types of Non Primitive Data Types

* String
* Array
* Class
* Interface
* Enum

---

### String

Used to store text.

Example:

```java
String name = "Java";
```

---

### Array

Used to store multiple values of the same type.

Example:

```java
int[] marks = {90, 80, 70};
```

---

### Class

A blueprint used to create objects.

Example:

```java
class Student {

}
```

---

### Interface

Contains abstract methods and constants.

Example:

```java
interface Vehicle {

}
```

---

### Enum

Represents a fixed set of constants.

Example:

```java
enum Day {

MONDAY,

TUESDAY

}
```

---

# Difference Between Primitive and Non Primitive Data Types

| Primitive Data Types | Non Primitive Data Types            |
| -------------------- | ----------------------------------- |
| Store actual values  | Store object references             |
| Fixed memory size    | Memory size varies                  |
| Faster               | Comparatively slower                |
| Predefined by Java   | Created by programmer or predefined |
| Cannot call methods  | Can call methods                    |

---

## Memory Representation

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

# Why Do We Need Data Types?

Data Types help Java to:

* Allocate memory efficiently.
* Prevent invalid data assignments.
* Improve type safety.
* Increase program performance.
* Improve code readability.

---

# Summary

This document explained:

* Data Types in Java
* Variable and Initialization
* Primitive Data Types
* Memory Size of Primitive Types
* Non Primitive Data Types
* Primitive vs Non Primitive
* Importance of Data Types

Data Types are one of the fundamental concepts in Java because every variable, object and method depends on an appropriate data type.
