# Explicit Type Casting in Java

## Objective

This program demonstrates **Explicit Type Casting** in Java.

It explains:

* Explicit Type Casting
* Narrowing Conversion
* Cast Operator
* Data Loss During Conversion
* Converting Larger Data Types to Smaller Data Types

Explicit Type Casting is used when the programmer intentionally converts a larger data type into a smaller data type using a cast operator.

---

# What is Explicit Type Casting?

## Definition

Explicit Type Casting is the process of converting a larger data type into a smaller data type manually using a cast operator.

It is also called:

```text
Narrowing Conversion
```

because:

```text
Larger Data Type

↓

Smaller Data Type
```

---

# Why is Explicit Type Casting Required?

Because:

```text
long → int

double → float

double → int

float → short
```

may cause:

* Data Loss
* Precision Loss
* Overflow

Therefore Java does not perform these conversions automatically.

The programmer must explicitly tell the compiler:

```text
I know there may be data loss.

Please perform the conversion.
```

---

# Syntax

```java
targetDataType variable = (targetDataType) sourceVariable;
```

Example:

```java
int num = (int) 100L;
```

---

## Program

```java
/*
 * Java Program Demonstrating Explicit Type Casting
 */

// Define a public class
public class ExplicitTypeCasting {

    // Main method - JVM starts execution here
    public static void main(String[] args) {

        // long to smaller data types

        long longValue = 9876543210L;

        int longToInt = (int) longValue;

        short longToShort = (short) longValue;

        byte longToByte = (byte) longValue;


        // double to smaller data types

        double doubleValue = 12345.6789;

        float doubleToFloat = (float) doubleValue;

        long doubleToLong = (long) doubleValue;

        int doubleToInt = (int) doubleValue;

        short doubleToShort = (short) doubleValue;


        // float to smaller data types

        float floatValue = 98.76f;

        int floatToInt = (int) floatValue;

        short floatToShort = (short) floatValue;


        // int to byte

        int intValue = 260;

        byte intToByte = (byte) intValue;


        // char to numeric types

        char charValue = 'Z';

        byte charToByte = (byte) charValue;

        short charToShort = (short) charValue;

        int charToInt = (int) charValue;


        // Display output

        System.out.println("Java Explicit Type Casting Example");

        System.out.println("----------------------------------");


        System.out.println("long value           : " + longValue);

        System.out.println("long -> int          : " + longToInt);

        System.out.println("long -> short        : " + longToShort);

        System.out.println("long -> byte         : " + longToByte);

        System.out.println();


        System.out.println("double value         : " + doubleValue);

        System.out.println("double -> float      : " + doubleToFloat);

        System.out.println("double -> long       : " + doubleToLong);

        System.out.println("double -> int        : " + doubleToInt);

        System.out.println("double -> short      : " + doubleToShort);

        System.out.println();


        System.out.println("float value          : " + floatValue);

        System.out.println("float -> int         : " + floatToInt);

        System.out.println("float -> short       : " + floatToShort);

        System.out.println();


        System.out.println("int value            : " + intValue);

        System.out.println("int -> byte          : " + intToByte);

        System.out.println();


        System.out.println("char value           : '" + charValue + "'");

        System.out.println("char -> byte         : " + charToByte);

        System.out.println("char -> short        : " + charToShort);

        System.out.println("char -> int          : " + charToInt);

    }

}
```

---

## Output

```text
Java Explicit Type Casting Example
----------------------------------

long value           : 9876543210
long -> int          : 1286608618
long -> short        : 5866
long -> byte         : -22

double value         : 12345.6789
double -> float      : 12345.679
double -> long       : 12345
double -> int        : 12345
double -> short      : 12345

float value          : 98.76
float -> int         : 98
float -> short       : 98

int value            : 260
int -> byte          : 4

char value           : 'Z'
char -> byte         : 90
char -> short        : 90
char -> int          : 90
```

---

## Pseudocode

```text
START

Declare long variable

Convert long to:

int

short

byte


Declare double variable

Convert double to:

float

long

int

short


Declare float variable

Convert float to:

int

short


Declare int variable

Convert int to byte


Declare char variable

Convert char to:

byte

short

int


Display all converted values

STOP
```

---

# Cast Operator

Explicit Type Casting uses:

```java
(targetDataType)
```

This is called:

```text
Cast Operator
```

Example:

```java
double num = 99.99;

int value = (int) num;
```

Output:

```text
99
```

Decimal part is removed.

---

# long to int Conversion

Example:

```java
long num = 1000L;

int value = (int) num;
```

Conversion:

```text
long

↓

int
```

Cast operator is mandatory.

---

# double to int Conversion

Example:

```java
double price = 99.99;

int amount = (int) price;
```

Output:

```text
99
```

Explanation:

```text
Decimal Part

↓

Discarded
```

---

# float to short Conversion

Example:

```java
float num = 25.99f;

short s = (short) num;
```

Output:

```text
25
```

Fractional part is removed.

---

# int to byte Conversion

Example:

```java
int num = 260;

byte b = (byte) num;
```

Output:

```text
4
```

Reason:

Byte Range:

```text
-128 to 127
```

260 exceeds byte range.

Overflow occurs.

---

# char to int Conversion

Example:

```java
char ch = 'Z';

int num = (int) ch;
```

Output:

```text
90
```

Reason:

Unicode value of:

```text
Z = 90
```

---

# Narrowing Conversion Hierarchy

```text
double

↓

float

↓

long

↓

int

↓

short

↓

byte
```

Memory size decreases.

Hence:

```text
Data Loss May Occur
```

---

# Implicit vs Explicit Type Casting

| Implicit Type Casting | Explicit Type Casting  |
| --------------------- | ---------------------- |
| Automatic             | Manual                 |
| Smaller → Larger      | Larger → Smaller       |
| Widening Conversion   | Narrowing Conversion   |
| No Cast Operator      | Cast Operator Required |
| No Data Loss          | Data Loss May Occur    |

---

# Why Do We Use Explicit Type Casting?

Explicit Type Casting is used to:

* Reduce memory usage.
* Convert large values into smaller types.
* Match method parameter types.
* Convert decimal values into integers.
* Perform controlled conversions.

---

# Important Points

1. Explicit Type Casting is manual.

2. Cast operator is mandatory.

3. Data loss may occur.

4. Decimal values lose fractional part.

5. Overflow may occur when converting to smaller types.

---

# Summary

This program demonstrates:

* Explicit Type Casting
* Narrowing Conversion
* Cast Operator
* long to int conversion
* double to float conversion
* double to int conversion
* float to short conversion
* int to byte conversion
* char to numeric conversion
* Overflow and Data Loss

Explicit Type Casting is one of the most important Core Java concepts because it gives programmers control over data conversion while handling memory and precision requirements.
