# Interview Questions and Answers

## Data Types

### Q1. What is a Data Type in Java?

**Answer:**

A Data Type specifies the type of value that a variable can store, such as integer, decimal, character, or boolean.

---

### Q2. How many categories of Data Types are there in Java?

**Answer:**

There are two categories:

1. Primitive Data Types
2. Non-Primitive Data Types

---

### Q3. What is a Variable?

**Answer:**

A Variable is a name given to a memory location used to store data.

**Example:**

```java
int age = 25;
```

---

### Q4. Why are Data Types important?

**Answer:**

* They specify the type of data.
* They determine memory allocation.
* They help perform valid operations on data.
* They improve type safety.

---

# Primitive Data Types

### Q5. How many Primitive Data Types are there in Java?

**Answer:**

There are **8 Primitive Data Types**:

* byte
* short
* int
* long
* float
* double
* char
* boolean

---

### Q6. What is byte?

**Answer:**

`byte` is an 8-bit signed integer.

**Memory Size:**

```text
1 Byte
```

**Range:**

```text
-128 to 127
```

---

### Q7. What is short?

**Answer:**

`short` is a 16-bit signed integer.

**Memory Size:**

```text
2 Bytes
```

---

### Q8. What is int?

**Answer:**

`int` is a 32-bit signed integer.

**Memory Size:**

```text
4 Bytes
```

**Example:**

```java
int age = 25;
```

---

### Q9. What is long?

**Answer:**

`long` is a 64-bit signed integer.

**Memory Size:**

```text
8 Bytes
```

**Example:**

```java
long number = 123456789L;
```

---

### Q10. What is float?

**Answer:**

`float` stores decimal values.

**Memory Size:**

```text
4 Bytes
```

**Example:**

```java
float price = 25.5f;
```

---

### Q11. What is double?

**Answer:**

`double` stores decimal values with higher precision.

**Memory Size:**

```text
8 Bytes
```

**Example:**

```java
double salary = 25000.75;
```

---

### Q12. What is char?

**Answer:**

`char` stores a single Unicode character.

**Memory Size:**

```text
2 Bytes
```

**Example:**

```java
char grade = 'A';
```

---

### Q13. What is boolean?

**Answer:**

`boolean` stores only two values:

* true
* false

**Example:**

```java
boolean status = true;
```

---

# Non Primitive Data Types

### Q14. What are Non Primitive Data Types?

**Answer:**

Non Primitive Data Types are reference types that store references to objects.

**Examples:**

* String
* Array
* Class
* Interface
* Enum

---

### Q15. What is String?

**Answer:**

String is a sequence of characters.

**Example:**

```java
String name = "Java";
```

---

### Q16. What is an Array?

**Answer:**

An Array is a collection of elements of the same data type.

**Example:**

```java
int[] numbers = {10,20,30};
```

---

### Q17. What is an Enum?

**Answer:**

Enum is a special class used to define fixed constants.

**Example:**

```java
enum Day {

MONDAY,

TUESDAY

}
```

---

# Primitive vs Non Primitive Data Types

### Q18. Difference between Primitive and Non Primitive Data Types?

| Primitive Data Types | Non Primitive Data Types     |
| -------------------- | ---------------------------- |
| Stores actual values | Stores references to objects |
| Fixed memory size    | Memory size varies           |
| Faster access        | Slightly slower              |
| Cannot call methods  | Can call methods             |

---

### Q19. Which is faster, Primitive or Non Primitive?

**Answer:**

Primitive Data Types are faster because values are stored directly in memory.

---

### Q20. Can Primitive Types call methods?

**Answer:**

No.

Primitive Types cannot call methods directly.

---

# Type Casting

### Q21. What is Type Casting?

**Answer:**

Type Casting is the process of converting one data type into another.

---

### Q22. How many Types of Type Casting are there?

**Answer:**

There are two types:

1. Implicit Type Casting
2. Explicit Type Casting

---

# Implicit Type Casting

### Q23. What is Implicit Type Casting?

**Answer:**

Implicit Type Casting is automatic conversion from a smaller data type to a larger data type.

It is also called:

```text
Widening Conversion
```

---

### Q24. Give examples of Implicit Type Casting.

**Answer:**

```text
byte → short

short → int

int → long

long → float

float → double
```

---

### Q25. Is Explicit Cast required in Implicit Type Casting?

**Answer:**

No.

Java automatically performs the conversion.

---

### Q26. Is Data Loss possible in Implicit Type Casting?

**Answer:**

Generally No.

Because a smaller data type is converted into a larger data type.

---

### Q27. Example of Implicit Type Casting?

**Answer:**

```java
int num = 100;

float value = num;
```

---

# Explicit Type Casting

### Q28. What is Explicit Type Casting?

**Answer:**

Explicit Type Casting converts a larger data type into a smaller data type manually.

It is also called:

```text
Narrowing Conversion
```

---

### Q29. Why is Explicit Casting required?

**Answer:**

Because data may be lost during conversion.

Java requires the programmer to cast explicitly.

---

### Q30. Example of Explicit Casting?

**Answer:**

```java
long num = 1000;

int value = (int) num;
```

---

### Q31. What is the Syntax of Explicit Casting?

**Answer:**

```java
(TargetType) variable
```

**Example:**

```java
int x = (int) longValue;
```

---

### Q32. Can Data Loss occur in Explicit Casting?

**Answer:**

Yes.

Information may be lost when converting a larger data type into a smaller data type.

---

### Q33. What is the Output?

```java
int x = (int) 10.75;

System.out.println(x);
```

**Answer:**

```text
10
```

The decimal part is removed.

---

### Q34. Difference between Implicit and Explicit Casting?

| Implicit Casting    | Explicit Casting     |
| ------------------- | -------------------- |
| Automatic           | Manual               |
| Smaller to Larger   | Larger to Smaller    |
| Safe Conversion     | Data Loss Possible   |
| Widening Conversion | Narrowing Conversion |

---

### Q35. Which Type Casting is safer?

**Answer:**

Implicit Type Casting is safer because there is no loss of data in normal widening conversions.

---

### Q36. Is char involved in Type Casting?

**Answer:**

Yes.

`char` can be converted to:

* int
* long
* float
* double

**Example:**

```java
char ch = 'A';

int x = ch;
```

**Output:**

```text
65
```

---

### Q37. What is Widening Conversion?

**Answer:**

Conversion from a smaller data type to a larger data type.

**Example:**

```text
int → double
```

---

### Q38. What is Narrowing Conversion?

**Answer:**

Conversion from a larger data type to a smaller data type.

**Example:**

```text
double → int
```

---

### Q39. Which operator is used in Explicit Type Casting?

**Answer:**

Cast Operator.

Examples:

```java
(int)

(double)

(float)
```

---

### Q40. Which topics are frequently asked in Java Interviews?

**Answer:**

* Primitive Data Types
* Non Primitive Data Types
* Memory Size of Data Types
* Implicit Type Casting
* Explicit Type Casting
* Widening Conversion
* Narrowing Conversion
* Primitive vs Non Primitive Data Types
* Type Casting Rules
* Cast Operator
