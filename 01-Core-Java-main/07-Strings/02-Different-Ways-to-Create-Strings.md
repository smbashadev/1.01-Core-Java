# Different Ways to Create Strings in Java

## Headline

Different Ways to Create Strings in Java

## Definition

Strings can be created in Java using different methods.

There are three common ways:

1. Using the `new` keyword
2. Using a character array
3. Using a string literal

---

## Java Program

```java
/*
 * Different Ways to Create Strings in Java
 */

public class StringDemo1 {
    public static void main(String[] args) {

        // Step 1: Create a string using new keyword
        String s1 = new String("Java");

        // Step 2: Create a character array
        char[] ch = {'J', 'A', 'v', 'A'};

        // Step 3: Create a string from the character array
        String s2 = new String(ch);

        // Step 4: Create a string using string literal
        String s3 = "Java";

        // Step 5: Print all three strings
        System.out.println(s1);

        System.out.println(s2);

        System.out.println(s3);
    }
}
```

---

## Output

```text
Java
Java
Java
```

---

## Explanation

The first string is created using the `new` keyword.

```java
String s1 = new String("Java");
```

A new String object is created in Heap Memory.

---

The second string is created from a character array.

```java
char[] ch = {'J','A','v','A'};

String s2 = new String(ch);
```

The characters stored in the array are combined to form a String object.

---

The third string is created using a string literal.

```java
String s3 = "Java";
```

This String is stored in the String Constant Pool.

---

Although all three print the same output:

```text
Java
```

their creation process and memory allocation are different.

---

## Pseudocode

```text
START

Create s1 using new String("Java")

Create character array ch = {'J','A','v','A'}

Create s2 using new String(ch)

Create s3 using string literal "Java"

Print s1

Print s2

Print s3

STOP
```

---

## Code Explanation

### 1. Create String using new keyword

```java
String s1 = new String("Java");
```

- Creates a new String object.
- Object is stored in Heap Memory.
- Even if "Java" already exists, a new object is created.

---

### 2. Create Character Array

```java
char[] ch = {'J','A','v','A'};
```

- Stores characters individually.
- Each character occupies one position in the array.

---

### 3. Convert Character Array to String

```java
String s2 = new String(ch);
```

- Converts the character array into a String object.
- The complete text becomes `"JAvA"`.

---

### 4. Create String using Literal

```java
String s3 = "Java";
```

- Uses String Constant Pool.
- Memory efficient because duplicate literals share the same object.

---

### 5. Print Strings

```java
System.out.println(s1);

System.out.println(s2);

System.out.println(s3);
```

Prints all three strings on the console.

---

## Important Points

- String literals are stored in the **String Constant Pool**.
- `new String()` creates a new object in Heap Memory.
- Character arrays can be converted into Strings.
- String literals are memory efficient.
- All three methods create String objects, but memory allocation differs.

---

## Memory Representation

### Using new Keyword

```text
Heap Memory

s1 ----> "Java"
```

---

### Using Character Array

```text
char[] ch

[J] [A] [v] [A]

s2 ----> "JAvA"
```

---

### Using String Literal

```text
String Constant Pool

"Java"

s3 ----> "Java"
```

---

## Summary

- Strings can be created in three different ways in Java.
- Using `new String()` creates objects in Heap Memory.
- Using character arrays converts characters into a String.
- Using string literals stores Strings in the String Constant Pool.
- String literals are the most commonly used and memory efficient way to create Strings.
