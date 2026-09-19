# Duplicate Strings and String Pool

## Headline

Storing Duplicate String Values Outside String Pool

## Definition

In Java, duplicate string values can be stored in different memory areas.

- String literals are stored in the **String Constant Pool (SCP)**.
- Strings created using the **new** keyword are stored in **Heap Memory**.
- Even if the values are the same, their memory references may be different.

This program demonstrates the difference between **value equality** and **reference equality**.

---

## Java Program

```java
/*
 * Storing Duplicate String Values Outside String Pool
 *
 * This program demonstrates duplicate string values stored
 * in String Pool and Heap Memory.
 */

public class StringDemo2 {
    public static void main(String[] args) {

        // Step 1: Create string literal and store it in String Pool
        String s1 = "Java";

        // Step 2: Create another string literal with same value
        String s2 = "Java";

        // Step 3: Create a new string object in Heap Memory
        String s3 = new String("Java");

        // Step 4: Print values
        System.out.println("Value of s1: " + s1);
        System.out.println("Value of s2: " + s2);
        System.out.println("Value of s3: " + s3);

        // Step 5: Compare values using equals()
        System.out.println("s1 equals s2: " + s1.equals(s2));
        System.out.println("s1 equals s3: " + s1.equals(s3));

        // Step 6: Compare references using ==
        System.out.println("s1 == s2: " + (s1 == s2));
        System.out.println("s1 == s3: " + (s1 == s3));
    }
}
```

---

## Output

```text
Value of s1: Java
Value of s2: Java
Value of s3: Java

s1 equals s2: true
s1 equals s3: true

s1 == s2: true
s1 == s3: false
```

---

## Explanation

- `s1` is created using a String literal.

```java
String s1 = "Java";
```

It is stored in the **String Constant Pool**.

---

- `s2` is also created using the same String literal.

```java
String s2 = "Java";
```

Java does not create another object. Both `s1` and `s2` point to the same memory location.

Therefore:

```java
s1 == s2
```

returns:

```text
true
```

---

- `s3` is created using:

```java
String s3 = new String("Java");
```

This creates a completely new object in Heap Memory.

Therefore:

```java
s1 == s3
```

returns:

```text
false
```

because they refer to different objects.

---

However:

```java
s1.equals(s3)
```

returns:

```text
true
```

because `equals()` compares the values, not the memory references.

---

## Pseudocode

```text
START

Create s1 = "Java"

Create s2 = "Java"

Create s3 = new String("Java")

Print s1, s2 and s3

Compare s1 and s2 using equals()

Compare s1 and s3 using equals()

Compare s1 and s2 using ==

Compare s1 and s3 using ==

STOP
```

---

## Code Explanation

### String Literal

```java
String s1 = "Java";

String s2 = "Java";
```

- Stored in String Constant Pool.
- Duplicate literals share the same object.

---

### String using new Keyword

```java
String s3 = new String("Java");
```

- Creates a new object.
- Stored separately in Heap Memory.

---

### equals() Method

```java
s1.equals(s2);

s1.equals(s3);
```

- Compares String values (contents).
- Returns `true` if values are equal.

---

### == Operator

```java
s1 == s2;

s1 == s3;
```

- Compares memory references.
- Returns `true` only when both references point to the same object.

---

## Memory Representation

### String Constant Pool

```text
        String Pool

          "Java"
         /      \
       s1        s2
```

Both variables point to the same object.

---

### Heap Memory

```text
String Pool

      "Java"
      /   \
    s1     s2


Heap Memory

      "Java"
         ^
         |
         s3
```

`s3` points to a different object created using `new`.

---

## Important Points

- String literals are stored in String Constant Pool.
- Duplicate literals share the same object.
- `new String()` creates a separate object in Heap Memory.
- `equals()` compares values.
- `==` compares references.
- Same String values can have different memory locations.

---

## Summary

This program demonstrates duplicate String values stored in different memory locations.

- `s1` and `s2` share the same object in String Pool.
- `s3` creates a separate object in Heap Memory.
- `equals()` checks values.
- `==` checks memory references.

This is one of the most frequently asked String interview concepts in Java.
