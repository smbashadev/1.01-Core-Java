# Implicit Type Casting in Java

## Objective

This program demonstrates **Implicit Type Casting** in Java.

It explains:

* Automatic Type Conversion
* Widening Conversion
* Conversion Hierarchy
* Primitive Data Type Promotion
* Conversion from Smaller Data Types to Larger Data Types

Implicit Type Casting is performed automatically by the Java compiler when converting a smaller data type into a larger compatible data type.

---

# What is Implicit Type Casting?

## Definition

Implicit Type Casting is the automatic conversion of a smaller primitive data type into a larger primitive data type.

The programmer does not need to write any cast operator.

It is also called:

```text
Widening Conversion
```

because:

```text
Smaller Data Type

↓

Larger Data Type
```

---

# Implicit Conversion Hierarchy

```text
byte
  ↓
short
  ↓
int
  ↓
long
  ↓
float
  ↓
double
```

Java automatically performs these conversions.

---

## Program

```java
/*
 * Java Program Demonstrating Implicit Type Casting
 */

// Define a public class
public class ImplicitTypeCasting {

    // Main method - JVM starts execution here
    public static void main(String[] args) {

        // byte to larger data types

        byte byteValue = 42;

        short byteToShort = byteValue;

        int byteToInt = byteValue;

        long byteToLong = byteValue;

        float byteToFloat = byteValue;

        double byteToDouble = byteValue;


        // short to larger data types

        short shortValue = 32000;

        int shortToInt = shortValue;

        long shortToLong = shortValue;

        float shortToFloat = shortValue;

        double shortToDouble = shortValue;


        // char to larger data types

        char charValue = 'A';

        int charToInt = charValue;

        long charToLong = charValue;

        float charToFloat = charValue;

        double charToDouble = charValue;


        // int to larger data types

        int intValue = 123456;

        long intToLong = intValue;

        float intToFloat = intValue;

        double intToDouble = intValue;


        // long to larger data types

        long longValue = 123456789L;

        float longToFloat = longValue;

        double longToDouble = longValue;


        // float to double

        float floatValue = 3.14f;

        double floatToDouble = floatValue;


        // Display Output

        System.out.println("Java Implicit Type Casting Example");

        System.out.println("----------------------------------");

        System.out.println("byte value         : " + byteValue);

        System.out.println("byte -> short      : " + byteToShort);

        System.out.println("byte -> int        : " + byteToInt);

        System.out.println("byte -> long       : " + byteToLong);

        System.out.println("byte -> float      : " + byteToFloat);

        System.out.println("byte -> double     : " + byteToDouble);

        System.out.println();


        System.out.println("short value        : " + shortValue);

        System.out.println("short -> int       : " + shortToInt);

        System.out.println("short -> long      : " + shortToLong);

        System.out.println("short -> float     : " + shortToFloat);

        System.out.println("short -> double    : " + shortToDouble);

        System.out.println();


        System.out.println("char value         : '" + charValue + "'");

        System.out.println("char -> int        : " + charToInt);

        System.out.println("char -> long       : " + charToLong);

        System.out.println("char -> float      : " + charToFloat);

        System.out.println("char -> double     : " + charToDouble);

        System.out.println();


        System.out.println("int value          : " + intValue);

        System.out.println("int -> long        : " + intToLong);

        System.out.println("int -> float       : " + intToFloat);

        System.out.println("int -> double      : " + intToDouble);

        System.out.println();


        System.out.println("long value         : " + longValue);

        System.out.println("long -> float      : " + longToFloat);

        System.out.println("long -> double     : " + longToDouble);

        System.out.println();


        System.out.println("float value        : " + floatValue);

        System.out.println("float -> double    : " + floatToDouble);

    }

}
```

---

## Output

```text
Java Implicit Type Casting Example
----------------------------------

byte value         : 42
byte -> short      : 42
byte -> int        : 42
byte -> long       : 42
byte -> float      : 42.0
byte -> double     : 42.0

short value        : 32000
short -> int       : 32000
short -> long      : 32000
short -> float     : 32000.0
short -> double    : 32000.0

char value         : 'A'
char -> int        : 65
char -> long       : 65
char -> float      : 65.0
char -> double     : 65.0

int value          : 123456
int -> long        : 123456
int -> float       : 123456.0
int -> double      : 123456.0

long value         : 123456789
long -> float      : 1.23456792E8
long -> double     : 1.23456789E8

float value        : 3.14
float -> double    : 3.14
```

---

## Pseudocode

```text
START

Declare byte variable

Convert byte to:

short

int

long

float

double


Declare short variable

Convert short to:

int

long

float

double


Declare char variable

Convert char to:

int

long

float

double


Declare int variable

Convert int to:

long

float

double


Declare long variable

Convert long to:

float

double


Declare float variable

Convert float to:

double


Display all converted values

STOP
```

---

# Why is it Called Widening Conversion?

Because:

```text
byte (1 Byte)

↓

short (2 Bytes)

↓

int (4 Bytes)

↓

long (8 Bytes)

↓

float

↓

double
```

Memory capacity increases.

Therefore:

```text
No Data Loss Occurs
```

---

# byte to Larger Types

Example:

```java
byte b = 42;

int num = b;
```

Conversion:

```text
byte

↓

int
```

Automatic conversion.

---

# short to Larger Types

Example:

```java
short s = 32000;

long num = s;
```

Conversion:

```text
short

↓

long
```

No cast operator required.

---

# char to int Conversion

Example:

```java
char ch = 'A';

int num = ch;
```

Output:

```text
65
```

Reason:

```text
Unicode Value of A = 65
```

---

# int to long Conversion

Example:

```java
int num = 100;

long value = num;
```

Conversion:

```text
int

↓

long
```

Automatic conversion.

---

# long to float Conversion

Example:

```java
long num = 1000L;

float value = num;
```

Conversion:

```text
long

↓

float
```

Performed automatically.

---

# float to double Conversion

Example:

```java
float price = 99.99f;

double value = price;
```

Conversion:

```text
float

↓

double
```

---

# Why No Cast Operator is Required?

Because:

```text
Smaller Type

↓

Larger Type
```

Java guarantees:

* Safe conversion.
* No information loss.
* Automatic conversion.

Hence:

```java
int num = 10;

double d = num;
```

is valid.

---

# Difference Between Implicit and Explicit Type Casting

| Implicit Type Casting | Explicit Type Casting  |
| --------------------- | ---------------------- |
| Automatic             | Manual                 |
| Smaller → Larger      | Larger → Smaller       |
| Widening Conversion   | Narrowing Conversion   |
| No Cast Operator      | Cast Operator Required |
| No Data Loss          | Data Loss May Occur    |

---

# Summary

This program demonstrates:

* Implicit Type Casting
* Widening Conversion
* byte to short/int/long/float/double
* short to int/long/float/double
* char to numeric conversions
* int to long/float/double
* long to float/double
* float to double
* Automatic conversions without cast operator

Implicit Type Casting is one of the most important Core Java concepts because it allows safe conversion between compatible primitive data types automatically.
