# Strings in Java

## Objective

The String class is one of the most important classes in Java. It is used to store and manipulate textual data.

This chapter introduces Strings, how they are created, immutability, String methods, String comparison, and the differences between String, StringBuffer, and StringBuilder.

---

## 1. Definition of String

A String in Java is a sequence of characters used to store text.

It is one of the most commonly used data types in Java.

### Example

```java
String name = "Rahul";
```

Here,

- `String` → Data type
- `name` → Variable name
- `"Rahul"` → String literal

---

## 2. How Strings are Created

Strings can be created in three ways.

### Method 1: Using String Literal

```java
String name = "Aman";
```

The object is created inside the **String Constant Pool**.

---

### Method 2: Using new Keyword

```java
String name = new String("Aman");
```

The object is created in Heap Memory.

---

### Method 3: Using Character Array

```java
char[] ch = {'J','a','v','a'};

String s = new String(ch);
```

Output:

```text
Java
```

---

## Example

```java
String name1 = "Aman";

String name2 = new String("Aman");
```

---

## 3. String is Immutable

A String object cannot be modified after it is created.

This property is called **Immutability**.

### Example

```java
String s = "Java";

s = s + " Programming";
```

Initially:

```text
s = Java
```

After concatenation:

```text
s = Java Programming
```

The original object `"Java"` is not modified.

A new object is created.

---

## Why is String Immutable?

Strings are immutable because:

- Security
- Thread Safety
- String Pool optimization
- Better caching
- Improved performance

---

## 4. String Concatenation

String Concatenation means joining two or more Strings.

### Using + Operator

```java
String first = "Hello";

String second = "World";

System.out.println(first + " " + second);
```

### Output

```text
Hello World
```

---

## 5. Important String Methods

Java provides many built-in String methods.

| Method | Description |
|-------|-------------|
| length() | Returns length of string |
| charAt() | Returns character at index |
| concat() | Joins strings |
| equals() | Compares contents |
| equalsIgnoreCase() | Compares ignoring case |
| toUpperCase() | Converts to uppercase |
| toLowerCase() | Converts to lowercase |
| trim() | Removes spaces |
| substring() | Extracts part of string |
| replace() | Replaces characters |
| indexOf() | Finds first occurrence |
| lastIndexOf() | Finds last occurrence |
| contains() | Checks existence |
| startsWith() | Checks starting characters |
| endsWith() | Checks ending characters |

---

## 6. Example of String Methods

```java
String s = "Java Programming";

System.out.println(s.length());

System.out.println(s.charAt(0));

System.out.println(s.toUpperCase());

System.out.println(s.substring(0,4));
```

### Output

```text
16

J

JAVA PROGRAMMING

Java
```

---

## 7. Comparison of Strings

Strings should always be compared using:

```java
equals()
```

instead of:

```java
==
```

### Example

```java
String a = "Java";

String b = "Java";

System.out.println(a.equals(b));
```

### Output

```text
true
```

---

### Difference Between == and equals()

| == | equals() |
|----|----------|
| Compares memory addresses | Compares contents |
| Reference comparison | Value comparison |
| May return false | Returns true if contents are same |

### Example

```java
String a = new String("Java");

String b = new String("Java");

System.out.println(a==b);

System.out.println(a.equals(b));
```

Output:

```text
false

true
```

---

## 8. StringBuffer and StringBuilder

StringBuffer and StringBuilder are mutable classes.

They are used when Strings need frequent modifications.

---

### StringBuffer

- Mutable
- Thread Safe
- Synchronized
- Slower than StringBuilder

Example:

```java
StringBuffer sb = new StringBuffer("Java");

sb.append(" Programming");

System.out.println(sb);
```

Output:

```text
Java Programming
```

---

### StringBuilder

- Mutable
- Not Thread Safe
- Not Synchronized
- Faster than StringBuffer

Example:

```java
StringBuilder sb = new StringBuilder("Java");

sb.append(" Programming");

System.out.println(sb);
```

Output:

```text
Java Programming
```

---

## 9. Difference Between String, StringBuffer and StringBuilder

| Feature | String | StringBuffer | StringBuilder |
|--------|--------|-------------|---------------|
| Mutable | No | Yes | Yes |
| Thread Safe | Yes | Yes | No |
| Synchronized | No | Yes | No |
| Performance | Slow | Medium | Fast |
| Memory | More objects | Less objects | Less objects |

---

## 10. Important Points About Strings

- Strings are objects in Java.
- Strings are immutable.
- Strings are stored in String Constant Pool.
- String methods do not modify the original String.
- A new String object is created after modification.
- String comparison should be done using equals().
- StringBuffer and StringBuilder are mutable alternatives.

---

## 11. Sample Program

```java
String name = "Rahul";

System.out.println("Hello " + name);
```

### Output

```text
Hello Rahul
```

---

## Why Do We Use Strings in Java?

Strings are used because:

- To store names.
- To store addresses.
- To process text data.
- To handle user input.
- To read files.
- To process messages.
- To manipulate characters efficiently.

Almost every Java application uses Strings.

---

## Summary

- String is a sequence of characters.
- Strings are immutable.
- Strings can be created using literals, new keyword, and character arrays.
- String methods help manipulate text.
- equals() is used for String comparison.
- StringBuffer and StringBuilder are mutable alternatives.
- Strings are one of the most frequently used classes in Java.
