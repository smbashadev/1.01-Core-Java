# Java String intern() Method

## Headline

Java String intern() Method Example

## Definition

The `intern()` method returns the reference of the String object from the **String Constant Pool (SCP)**.

If the same string already exists in the String Pool, the existing reference is returned.

Otherwise, the string is added to the String Pool and its reference is returned.

---

## Java Program

```java
/*
 * Java String intern() Method Example
 */

public class StringDemo7 {
    public static void main(String[] args) {

        // Step 1: Create two separate String objects with same content
        String s1 = new String("Java");

        // Step 2: Create another String object with same content
        String s2 = new String("Java");

        // Step 3: Print whether both references point to the same object
        System.out.println("s1 == s2: " + (s1 == s2));

        // Step 4: Call intern() to get the string from String Pool
        String s3 = s1.intern();

        // Step 5: Call intern() on the second string
        String s4 = s2.intern();

        // Step 6: Compare references
        System.out.println("s1 == s3: " + (s1 == s3));

        // Step 7: Check whether pooled references are same
        System.out.println("s3 == s4: " + (s3 == s4));

        // Step 8: Compare values
        System.out.println("s1.equals(s2): " + s1.equals(s2));

        // Step 9: Compare pooled values
        System.out.println("s3.equals(s4): " + s3.equals(s4));
    }
}
```

---

## Output

```text
s1 == s2: false

s1 == s3: false

s3 == s4: true

s1.equals(s2): true

s3.equals(s4): true
```

---

## Explanation

`s1` and `s2` are created using:

```java
new String("Java")
```

Therefore, Java creates two separate objects in Heap Memory.

So:

```java
s1 == s2
```

returns:

```text
false
```

because both references point to different objects.

---

When we call:

```java
String s3 = s1.intern();

String s4 = s2.intern();
```

Java checks the String Constant Pool.

If `"Java"` already exists, Java returns the pooled object.

Therefore:

```java
s3 == s4
```

returns:

```text
true
```

because both variables point to the same String Pool object.

---

However:

```java
s1 == s3
```

returns:

```text
false
```

because:

- s1 points to Heap Memory
- s3 points to String Pool

They are different objects.

---

## Pseudocode

```text
START

Create s1 = new String("Java")

Create s2 = new String("Java")

Print s1 == s2

s3 = s1.intern()

s4 = s2.intern()

Print s1 == s3

Print s3 == s4

Print s1.equals(s2)

Print s3.equals(s4)

STOP
```

---

## Code Explanation

### Creating Strings using new

```java
String s1 = new String("Java");

String s2 = new String("Java");
```

- Creates two separate String objects.
- Stored in Heap Memory.
- References are different.

---

### Using intern()

```java
String s3 = s1.intern();

String s4 = s2.intern();
```

- Searches the String Pool.
- Returns the pooled String reference.
- Avoids creating duplicate String literals.

---

### == Operator

```java
s1 == s2

s3 == s4
```

- Compares object references.
- Returns true only if both references point to the same object.

---

### equals() Method

```java
s1.equals(s2)

s3.equals(s4)
```

- Compares String contents.
- Returns true when values are equal.

---

## Memory Representation

### Before intern()

```text
Heap Memory

s1 -----> "Java"

s2 -----> "Java"


String Pool

"Java"
```

`s1` and `s2` are different objects.

---

### After intern()

```text
Heap Memory

s1 -----> "Java"

s2 -----> "Java"


String Pool

        "Java"
        /    \
      s3      s4
```

Both `s3` and `s4` point to the same String Pool object.

---

## Important Points

- `intern()` returns the String Pool reference.
- It helps reuse String objects.
- It saves memory by avoiding duplicate strings in the pool.
- `==` compares references.
- `equals()` compares values.
- Strings created using `new` are stored in Heap Memory.
- String literals are stored in the String Constant Pool.

---

## Syntax of intern()

```java
String variable = stringObject.intern();
```

Example:

```java
String s = new String("Java");

String pooled = s.intern();
```

---

## Summary

The `intern()` method is used to obtain the String Pool reference of a String.

- `new String()` creates objects in Heap Memory.
- `intern()` returns the pooled String object.
- It improves memory efficiency.
- It is one of the most frequently asked String interview topics in Java.
