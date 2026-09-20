# Palindrome String in Java

## Headline

Palindrome String Program

## Definition

A palindrome string is a string that reads the same from left to right and from right to left.

### Examples

```text
madam    → Palindrome

level    → Palindrome

radar    → Palindrome

java     → Not a Palindrome
```

---

## Java Program

```java
/*
 * Palindrome String Program
 */

public class StringDemo6 {
    public static void main(String[] args) {

        // Step 1: Store the string to check
        String text = "madam";

        // Step 2: Convert the string to lowercase
        String lowerText = text.toLowerCase();

        // Step 3: Reverse the string
        String reverseText = "";

        for (int i = lowerText.length() - 1; i >= 0; i--) {

            reverseText = reverseText + lowerText.charAt(i);

        }

        // Step 4: Compare original and reversed strings

        if (lowerText.equals(reverseText)) {

            System.out.println(text + " is a palindrome");

        } else {

            System.out.println(text + " is not a palindrome");

        }
    }
}
```

---

## Output

```text
madam is a palindrome
```

---

## Explanation

The program stores the word:

```text
madam
```

Then it reverses the word character by character:

```text
madam → madam
```

Since the original string and reversed string are equal,

the output is:

```text
madam is a palindrome
```

---

## Pseudocode

```text
START

Store string "madam"

Convert to lowercase

Create empty string reverseText

FOR i = length-1 TO 0

    reverseText = reverseText + current character

END FOR

IF original equals reverseText

    Print "Palindrome"

ELSE

    Print "Not Palindrome"

END IF

STOP
```

---

## Code Explanation

### Step 1

```java
String text = "madam";
```

Stores the input string.

---

### Step 2

```java
String lowerText = text.toLowerCase();
```

Converts the string to lowercase.

This makes the comparison case-insensitive.

Example:

```text
Madam → madam
```

---

### Step 3

```java
String reverseText = "";
```

Creates an empty string to store the reversed text.

---

### Step 4

```java
for(int i=lowerText.length()-1;i>=0;i--)
```

The loop starts from the last character and moves backward.

For:

```text
madam
```

Indexes are:

```text
m a d a m

0 1 2 3 4
```

The loop reads:

```text
4 → 3 → 2 → 1 → 0
```

---

### Step 5

```java
reverseText = reverseText + lowerText.charAt(i);
```

Adds one character at a time into the reversed string.

Process:

```text
m

ma

mad

mada

madam
```

---

### Step 6

```java
lowerText.equals(reverseText)
```

Compares the original string and reversed string.

If both are same:

```text
Palindrome
```

Otherwise:

```text
Not Palindrome
```

---

## Memory Representation

```text
text

"madam"



lowerText

"madam"



reverseText

"madam"
```

Comparison:

```text
lowerText.equals(reverseText)

madam == madam

true
```

---

## Example 1

```java
String text = "level";
```

Output:

```text
level is a palindrome
```

---

## Example 2

```java
String text = "radar";
```

Output:

```text
radar is a palindrome
```

---

## Example 3

```java
String text = "java";
```

Reverse:

```text
avaj
```

Output:

```text
java is not a palindrome
```

---

## Important Points

- A palindrome reads the same from both directions.
- `equals()` is used to compare strings.
- `charAt()` returns a character at a specific index.
- `toLowerCase()` ignores uppercase/lowercase differences.
- This example checks simple words without spaces.

---

## Frequently Asked Interview Question

### Q: Why do we use equals() instead of == ?

Answer:

```text
equals() → compares values

== → compares memory references
```

For palindrome checking, we compare values, so we use:

```java
equals()
```

---

## Summary

- A palindrome string reads the same forward and backward.
- Reverse the string and compare it with the original.
- If both are equal, the string is a palindrome.
- Common interview examples: madam, level, radar, civic, racecar.
