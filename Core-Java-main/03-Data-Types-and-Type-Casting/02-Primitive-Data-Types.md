# Primitive Data Types in Java

## Objective

This program demonstrates all **8 Primitive Data Types** available in Java.

The program:

* Declares one variable for each primitive data type.
* Assigns a sample value.
* Displays the values on the console.
* Explains memory size, range and usage of each primitive data type.

Primitive data types are the building blocks of Java programming because they store actual values directly in memory.

---

## Program

```java
/*
 * Java Program Demonstrating All Primitive Data Types
 */

// Define a public class named PrimitiveDataTypes
public class PrimitiveDataTypes {

    // Main method - JVM starts execution from here
    public static void main(String[] args) {

        // byte : 8-bit signed integer
        byte sampleByte = 100;

        // short : 16-bit signed integer
        short sampleShort = 32000;

        // int : 32-bit signed integer
        int sampleInt = 123456789;

        // long : 64-bit signed integer
        // L suffix is mandatory for large values
        long sampleLong = 1234567890123456789L;

        // float : 32-bit floating point number
        // f suffix is mandatory
        float sampleFloat = 3.14f;

        // double : 64-bit floating point number
        double sampleDouble = 9.81;

        // char : stores a single Unicode character
        char sampleChar = 'J';

        // boolean : stores true or false
        boolean sampleBoolean = true;

        // Display heading
        System.out.println("Java Primitive Data Types Example");

        System.out.println("--------------------------------");

        // Print byte value
        System.out.println("byte value    : " + sampleByte);

        // Print short value
        System.out.println("short value   : " + sampleShort);

        // Print int value
        System.out.println("int value     : " + sampleInt);

        // Print long value
        System.out.println("long value    : " + sampleLong);

        // Print float value
        System.out.println("float value   : " + sampleFloat);

        // Print double value
        System.out.println("double value  : " + sampleDouble);

        // Print char value
        System.out.println("char value    : " + sampleChar);

        // Print boolean value
        System.out.println("boolean value : " + sampleBoolean);

    } // End of main method

} // End of PrimitiveDataTypes class
```

---

## Output

```text
Java Primitive Data Types Example
--------------------------------

byte value    : 100

short value   : 32000

int value     : 123456789

long value    : 1234567890123456789

float value   : 3.14

double value  : 9.81

char value    : J

boolean value : true
```

---

## Pseudocode

```text
START

Declare byte variable

Declare short variable

Declare int variable

Declare long variable

Declare float variable

Declare double variable

Declare char variable

Declare boolean variable

Display all values

STOP
```

---

# Primitive Data Types in Java

Java provides **8 Primitive Data Types**.

They are:

| Data Type | Size          | Description              |
| --------- | ------------- | ------------------------ |
| byte      | 1 Byte        | Small integer            |
| short     | 2 Bytes       | Short integer            |
| int       | 4 Bytes       | Integer value            |
| long      | 8 Bytes       | Large integer            |
| float     | 4 Bytes       | Decimal number           |
| double    | 8 Bytes       | High precision decimal   |
| char      | 2 Bytes       | Single Unicode character |
| boolean   | JVM Dependent | true or false            |

---

## 1. byte Data Type

Declaration:

```java
byte sampleByte = 100;
```

Size:

```text
1 Byte = 8 Bits
```

Range:

```text
-128 to 127
```

Purpose:

Used to save memory when storing small integers.

---

## 2. short Data Type

Declaration:

```java
short sampleShort = 32000;
```

Size:

```text
2 Bytes = 16 Bits
```

Range:

```text
-32,768 to 32,767
```

Purpose:

Stores integer values larger than byte.

---

## 3. int Data Type

Declaration:

```java
int sampleInt = 123456789;
```

Size:

```text
4 Bytes = 32 Bits
```

Range:

```text
-2^31 to 2^31 - 1
```

Purpose:

Most commonly used integer type in Java.

---

## 4. long Data Type

Declaration:

```java
long sampleLong = 1234567890123456789L;
```

Size:

```text
8 Bytes = 64 Bits
```

Purpose:

Stores very large integer values.

### Why L suffix is used?

```java
long num = 100000L;
```

Because Java treats integer literals as `int` by default.

`L` explicitly tells Java:

```text
This is a long value
```

---

## 5. float Data Type

Declaration:

```java
float sampleFloat = 3.14f;
```

Size:

```text
4 Bytes = 32 Bits
```

Purpose:

Stores decimal values.

### Why f suffix is used?

Because decimal numbers are treated as:

```java
double
```

by default.

Hence:

```java
3.14f
```

indicates float.

---

## 6. double Data Type

Declaration:

```java
double sampleDouble = 9.81;
```

Size:

```text
8 Bytes = 64 Bits
```

Purpose:

Stores decimal values with high precision.

---

## 7. char Data Type

Declaration:

```java
char sampleChar = 'J';
```

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

Examples:

```java
char grade = 'A';

char symbol = '#';
```

---

## 8. boolean Data Type

Declaration:

```java
boolean sampleBoolean = true;
```

Stores:

```text
true

or

false
```

Purpose:

Used in:

* if statements
* loops
* decision making

Example:

```java
boolean isPassed = true;
```

---

## Line-by-Line Explanation

### Statement

```java
byte sampleByte = 100;
```

Creates a byte variable named:

```text
sampleByte
```

Stores:

```text
100
```

---

### Statement

```java
long sampleLong = 1234567890123456789L;
```

Creates a long variable.

`L` indicates:

```text
Long Literal
```

---

### Statement

```java
float sampleFloat = 3.14f;
```

Creates float variable.

`f` indicates:

```text
Float Literal
```

---

### Statement

```java
char sampleChar = 'J';
```

Stores single character:

```text
J
```

---

### Statement

```java
boolean sampleBoolean = true;
```

Stores:

```text
true
```

---

## Why Primitive Data Types are Called Primitive?

Because:

* They are predefined by Java.
* They store actual values directly.
* They are not objects.
* They provide faster execution.
* They consume less memory.

---

## Summary

This program demonstrates:

* All 8 Primitive Data Types
* Memory size of each data type
* Variable declaration and initialization
* long literals using L suffix
* float literals using f suffix
* Unicode characters using char
* Boolean values
* Console output using println()

Primitive Data Types are one of the most fundamental concepts in Java and are extensively asked in interviews and programming assessments.
