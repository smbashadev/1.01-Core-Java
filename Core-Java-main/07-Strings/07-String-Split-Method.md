# Java split() Method

## Headline

Java split() Method Example

## Definition

The `split()` method is used to divide a String into multiple parts based on a specified delimiter.

It returns an array of Strings.

The delimiter can be:

- Comma (,)
- Space (" ")
- Hyphen (-)
- Colon (:)
- Any regular expression

---

## Syntax

```java
String[] arrayName = stringName.split("delimiter");
```

### Example

```java
String text = "Java,Python,C,JavaScript";

String[] words = text.split(",");
```

---

## Java Program

```java
/*
 * Java split() Method Example
 */

public class StringDemo5 {
    public static void main(String[] args) {

        // Step 1: Create a string with comma separated values
        String text = "Java,Python,C,JavaScript";

        // Step 2: Split the string using comma delimiter
        String[] words = text.split(",");

        // Step 3: Print the original string
        System.out.println("Original String: " + text);

        // Step 4: Print each element after splitting
        System.out.println("Split parts:");

        for (int i = 0; i < words.length; i++) {

            System.out.println("Part " + i + ": " + words[i]);

        }
    }
}
```

---

## Output

```text
Original String: Java,Python,C,JavaScript

Split parts:

Part 0: Java

Part 1: Python

Part 2: C

Part 3: JavaScript
```

---

## Explanation

The original String is:

```java
Java,Python,C,JavaScript
```

When:

```java
text.split(",")
```

is executed,

Java searches for every comma `,` and breaks the String into smaller parts.

These parts are stored in an array.

```text
words[0] = Java

words[1] = Python

words[2] = C

words[3] = JavaScript
```

---

## Pseudocode

```text
START

Create String text

Assign:

"Java,Python,C,JavaScript"

Split text using comma

Store result in String array

Print original String

FOR each element in array

    Print element

END FOR

STOP
```

---

## Code Explanation

### Step 1

```java
String text = "Java,Python,C,JavaScript";
```

Creates a String containing comma-separated values.

---

### Step 2

```java
String[] words = text.split(",");
```

Breaks the String at every comma.

Returns:

```text
["Java","Python","C","JavaScript"]
```

---

### Step 3

```java
System.out.println("Original String: " + text);
```

Prints the original String.

---

### Step 4

```java
for(int i=0;i<words.length;i++)
```

Traverses the array returned by `split()`.

---

### Step 5

```java
System.out.println(words[i]);
```

Prints each separated word.

---

## Memory Representation

```text
text

"Java,Python,C,JavaScript"



After split(",")

words

+-------+------------+
| Index | Value      |
+-------+------------+
|   0   | Java       |
|   1   | Python     |
|   2   | C          |
|   3   | JavaScript |
+-------+------------+
```

---

## Examples of split()

### Using Space

```java
String s = "Java Programming Language";

String[] arr = s.split(" ");
```

Output:

```text
Java

Programming

Language
```

---

### Using Hyphen

```java
String s = "10-20-30-40";

String[] arr = s.split("-");
```

Output:

```text
10

20

30

40
```

---

### Using Colon

```java
String s = "A:B:C:D";

String[] arr = s.split(":");
```

Output:

```text
A

B

C

D
```

---

## Important Points

- `split()` returns an array of Strings.
- The delimiter is removed from the output.
- Array indexing starts from 0.
- If the delimiter is not found, the entire String becomes a single element.

Example:

```java
String s = "Java";

String[] arr = s.split(",");
```

Output:

```text
arr[0] = Java
```

---

## Common Syntax Examples

```java
split(",")

split(" ")

split("-")

split(":")

split("\\s")
```

---

## Summary

The `split()` method is used to divide a String into multiple parts based on a delimiter.

- Returns a String array.
- Common delimiters are comma, space, hyphen, and colon.
- Very useful for processing CSV data, sentences, and formatted text.
- One of the most frequently asked String methods in Java interviews.
