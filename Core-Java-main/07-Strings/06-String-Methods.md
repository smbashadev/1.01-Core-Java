# Java String Methods

## Headline

Java String Methods with Simple Example

## Definition

A String in Java is a sequence of characters used to store text.

Java provides many built-in methods to perform operations such as:

- Finding length
- Accessing characters
- Concatenating strings
- Comparing strings
- Converting case
- Removing spaces
- Extracting substrings
- Replacing characters
- Searching characters or words
- Checking prefixes and suffixes

---

## Java Program

```java
/*
 * Java String Methods with Simple Example
 */

public class StringDemo4 {
    public static void main(String[] args) {

        // Step 1: Create a string value
        String text = "  Java Programming  ";

        // Step 2: Use length() to get the number of characters
        int len = text.length();
        System.out.println("Length: " + len);

        // Step 3: Use charAt(index)
        System.out.println("Character at index 0: " + text.charAt(0));

        // Step 4: Use concat()
        String result = text.concat(" Language");
        System.out.println("After concat: " + result);

        // Step 5: Use equals()
        System.out.println("Equals with '  Java Programming  ': "
                + text.equals("  Java Programming  "));

        // Step 6: Use equalsIgnoreCase()
        System.out.println("EqualsIgnoreCase with '  java programming  ': "
                + text.equalsIgnoreCase("  java programming  "));

        // Step 7: Use toUpperCase() and toLowerCase()
        System.out.println("Uppercase: " + text.toUpperCase());

        System.out.println("Lowercase: " + text.toLowerCase());

        // Step 8: Use trim()
        System.out.println("Trimmed: " + text.trim());

        // Step 9: Use substring()
        String sub = text.trim().substring(0, 4);

        System.out.println("Substring: " + sub);

        // Step 10: Use replace()
        System.out.println("Replace 'a' with '@': "
                + text.replace('a', '@'));

        // Step 11: Use indexOf() and lastIndexOf()
        System.out.println("Index of 'a': " + text.indexOf('a'));

        System.out.println("Last index of 'a': "
                + text.lastIndexOf('a'));

        // Step 12: Use contains()
        System.out.println("Contains 'Programming': "
                + text.contains("Programming"));

        // Step 13: Use startsWith() and endsWith()
        System.out.println("Starts with space: "
                + text.startsWith(" "));

        System.out.println("Ends with space: "
                + text.endsWith(" "));
    }
}
```

---

## Output

```text
Length: 20

Character at index 0:

(space)

After concat:
  Java Programming   Language

Equals with '  Java Programming  ': true

EqualsIgnoreCase with '  java programming  ': true

Uppercase:
  JAVA PROGRAMMING  

Lowercase:
  java programming  

Trimmed:
Java Programming

Substring:
Java

Replace 'a' with '@':
  J@v@ Progr@mming  

Index of 'a': 3

Last index of 'a': 11

Contains 'Programming': true

Starts with space: true

Ends with space: true
```

---

## Explanation

The program creates the following string:

```java
String text = "  Java Programming  ";
```

This string contains:

- Leading spaces
- Text: Java Programming
- Trailing spaces

Different String methods are then used to manipulate and analyze the string.

---

## Pseudocode

```text
START

Create text = "  Java Programming  "

Find length

Find character at index 0

Concatenate another string

Compare strings using equals()

Compare ignoring case

Convert to uppercase

Convert to lowercase

Remove spaces using trim()

Extract substring

Replace characters

Find first occurrence

Find last occurrence

Check contains()

Check startsWith()

Check endsWith()

STOP
```

---

## Code Explanation

### 1. length()

```java
text.length()
```

Returns the total number of characters.

Output:

```text
20
```

---

### 2. charAt()

```java
text.charAt(0)
```

Returns the character at the specified index.

Output:

```text
(space)
```

---

### 3. concat()

```java
text.concat(" Language")
```

Combines two strings.

Output:

```text
Java Programming Language
```

---

### 4. equals()

```java
text.equals("  Java Programming  ")
```

Compares exact contents.

Output:

```text
true
```

---

### 5. equalsIgnoreCase()

```java
text.equalsIgnoreCase("  java programming  ")
```

Ignores uppercase and lowercase differences.

Output:

```text
true
```

---

### 6. toUpperCase()

```java
text.toUpperCase()
```

Converts all letters to uppercase.

Output:

```text
JAVA PROGRAMMING
```

---

### 7. toLowerCase()

```java
text.toLowerCase()
```

Converts all letters to lowercase.

Output:

```text
java programming
```

---

### 8. trim()

```java
text.trim()
```

Removes spaces from beginning and end.

Output:

```text
Java Programming
```

---

### 9. substring()

```java
text.trim().substring(0,4)
```

Extracts a part of the string.

Output:

```text
Java
```

---

### 10. replace()

```java
text.replace('a','@')
```

Replaces all occurrences of a character.

Output:

```text
J@v@ Progr@mming
```

---

### 11. indexOf()

```java
text.indexOf('a')
```

Returns the first occurrence index.

Output:

```text
3
```

---

### 12. lastIndexOf()

```java
text.lastIndexOf('a')
```

Returns the last occurrence index.

Output:

```text
11
```

---

### 13. contains()

```java
text.contains("Programming")
```

Checks whether a word exists.

Output:

```text
true
```

---

### 14. startsWith()

```java
text.startsWith(" ")
```

Checks the beginning of the string.

Output:

```text
true
```

---

### 15. endsWith()

```java
text.endsWith(" ")
```

Checks the ending of the string.

Output:

```text
true
```

---

## Commonly Used String Methods

| Method | Description |
|-------|-------------|
| length() | Returns string length |
| charAt() | Returns character at index |
| concat() | Concatenates strings |
| equals() | Compares values |
| equalsIgnoreCase() | Compares ignoring case |
| toUpperCase() | Converts to uppercase |
| toLowerCase() | Converts to lowercase |
| trim() | Removes spaces |
| substring() | Extracts part of string |
| replace() | Replaces characters |
| indexOf() | Finds first occurrence |
| lastIndexOf() | Finds last occurrence |
| contains() | Checks existence |
| startsWith() | Checks prefix |
| endsWith() | Checks suffix |

---

## Important Points

- String objects are immutable.
- String methods do not change the original string.
- Most String methods return a new String.
- Index values start from 0.
- `equals()` compares values.
- `==` compares memory references.

---

## Summary

This program demonstrates the most commonly used String methods in Java.

It covers:

- Length
- Character access
- Concatenation
- Comparison
- Case conversion
- Trimming
- Substring
- Replace
- Searching
- Prefix and suffix checking

These methods are frequently used in Java applications and interviews.
