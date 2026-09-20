# Type Casting in Java

## Objective

This document explains:

* What is Type Casting?
* Why Type Casting is required.
* Types of Type Casting in Java.
* Implicit Type Casting (Widening Conversion).
* Explicit Type Casting (Narrowing Conversion).
* Examples of each type.

Type Casting is one of the fundamental concepts in Java that allows conversion of data from one data type to another.

---

# What is Type Casting?

## Definition

Type Casting is the process of converting a value from one data type to another data type.

In Java, type casting helps programmers convert:

* Smaller data type to larger data type.
* Larger data type to smaller data type.

---

## Syntax of Type Casting

### Implicit Type Casting

```java
smallerDataTypeVariable = largerDataTypeVariable;
```

The conversion is performed automatically by Java Compiler.

---

### Explicit Type Casting

```java
targetDataType variable = (targetDataType) sourceVariable;
```

The conversion is performed manually by the programmer.

---

# Types of Type Casting in Java

There are two types of Type Casting:

```text
Type Casting
│
├── 1. Implicit Type Casting
│      (Widening Conversion)
│
└── 2. Explicit Type Casting
       (Narrowing Conversion)
```

---

# 1. Implicit Type Casting

## Definition

Implicit Type Casting is performed automatically by the Java Compiler when:

```text
Smaller Data Type

↓

Larger Data Type
```

The programmer does not need to perform any manual conversion.

It is also called:

```text
Widening Conversion
```

because the smaller data type is converted into a larger data type.

---

## Implicit Conversion Order

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

## Example

```java
int num = 100;

float value = num;
```

Explanation:

```text
int → float
```

The compiler automatically converts:

```text
100

↓

100.0
```

No cast operator is required.

---

## Why is it called Widening Conversion?

Because:

```text
int

4 Bytes

↓

float

4 Bytes with decimal representation
```

The destination type can store all values of the source type safely.

Hence:

```text
No Data Loss
```

---

# 2. Explicit Type Casting

## Definition

Explicit Type Casting is required when:

```text
Larger Data Type

↓

Smaller Data Type
```

The programmer must explicitly tell the compiler to perform the conversion.

This is done using:

```text
Cast Operator
```

It is also called:

```text
Narrowing Conversion
```

---

## Syntax

```java
targetType variable = (targetType) sourceVariable;
```

Example:

```java
int num = (int) 100L;
```

---

## Example

```java
long num = 1000L;

int value = (int) num;
```

Explanation:

```text
long → int
```

The compiler does not perform this conversion automatically.

Programmer must write:

```java
(int)
```

before the variable.

---

## Why is it called Narrowing Conversion?

Because:

```text
long

8 Bytes

↓

int

4 Bytes
```

Memory size decreases.

There is a possibility of:

```text
Data Loss
```

Hence Java requires explicit conversion.

---

# Cast Operator

The cast operator tells the compiler:

```text
I know this conversion may lose data,

but I want to perform it intentionally.
```

Syntax:

```java
(targetDataType)
```

Example:

```java
int num = (int) 25.50;
```

Output:

```text
25
```

Decimal part is removed.

---

# Difference Between Implicit and Explicit Type Casting

| Implicit Type Casting     | Explicit Type Casting  |
| ------------------------- | ---------------------- |
| Automatic conversion      | Manual conversion      |
| Smaller → Larger          | Larger → Smaller       |
| Widening Conversion       | Narrowing Conversion   |
| No cast operator required | Cast operator required |
| No data loss              | Data loss may occur    |

---

## Examples

### Implicit Type Casting

```java
byte b = 10;

int num = b;
```

Conversion:

```text
byte → int
```

Automatic conversion.

---

### Explicit Type Casting

```java
double num = 25.99;

int value = (int) num;
```

Conversion:

```text
double → int
```

Manual conversion.

Output:

```text
25
```

---

# Why Do We Need Type Casting?

Type Casting is used to:

* Convert one data type into another.
* Reduce memory usage.
* Perform arithmetic operations involving different data types.
* Work with methods requiring specific data types.
* Improve flexibility in programming.

---

# Important Point

Java performs:

```text
Smaller → Larger

Automatically
```

But:

```text
Larger → Smaller

Requires Explicit Casting
```

because:

```text
Data Loss may occur.
```

---

# Summary

This document explained:

* Type Casting in Java.
* Implicit Type Casting.
* Explicit Type Casting.
* Widening Conversion.
* Narrowing Conversion.
* Cast Operator.
* Difference between Implicit and Explicit Type Casting.

Type Casting is an important Core Java concept because it allows conversion between different data types while ensuring type safety and memory efficiency.
