# Escape Sequences in Java

## Objective

This program demonstrates the use of Java escape sequences inside string literals. Escape sequences are special characters that begin with a backslash (`\`) and are used to represent characters such as newline, tab, backspace and quotation marks.

---

## Program

```java
// Escape Sequences Program in Java

// Define a public class named EscapeSequences
public class EscapeSequences {

    // Main method - JVM starts execution from here
    public static void main(String[] args) {

        // Print "Java", move cursor to next line, then print "Python"
        System.out.println("Java\nPython");

        // Print "Java", insert a tab space, then print "Python"
        System.out.println("Java\tPython");

        // Print "Java", perform backspace, then print "Python"
        System.out.println("Java\bPython");

        // Print Java enclosed within double quotation marks
        System.out.println("\"Java\" is a Programming Language");

        // Print Java without moving the cursor to the next line
        System.out.print("Java");

        // Print Python on the same line
        System.out.print("Python");

    } // End of main method

} // End of EscapeSequences class
```

---

## Output

```text
Java
Python

Java    Python

JavPython

"Java" is a Programming Language

JavaPython
```

---

## Pseudocode

```text
START

Print Java and move to next line

Print Java and insert tab space

Print Java and perform backspace

Print Java enclosed in quotation marks

Print Java without newline

Print Python on the same line

STOP
```

---

## Line-by-Line Explanation

### Line 1

```java
public class EscapeSequences
```

Explanation:

* `public` → Class is accessible from anywhere.
* `class` → Keyword used to create a class.
* `EscapeSequences` → Name of the class.

---

### Line 2

```java
public static void main(String[] args)
```

Explanation:

* `public` → Accessible from anywhere.
* `static` → JVM can invoke the method without creating an object.
* `void` → Method does not return any value.
* `main` → Entry point of Java application.
* `String[] args` → Stores command line arguments.

---

### Statement 1

```java
System.out.println("Java\nPython");
```

Explanation:

* `\n` → New Line escape sequence.
* Moves the cursor to the next line.

Output:

```text
Java
Python
```

---

### Statement 2

```java
System.out.println("Java\tPython");
```

Explanation:

* `\t` → Horizontal Tab escape sequence.
* Inserts tab spacing between words.

Output:

```text
Java    Python
```

---

### Statement 3

```java
System.out.println("Java\bPython");
```

Explanation:

* `\b` → Backspace escape sequence.
* Removes the character immediately before it while displaying output.

Output:

```text
JavPython
```

---

### Statement 4

```java
System.out.println("\"Java\" is a Programming Language");
```

Explanation:

* `\"` → Double Quote escape sequence.
* Allows double quotation marks inside a string.

Output:

```text
"Java" is a Programming Language
```

---

### Statement 5

```java
System.out.print("Java");
```

Explanation:

* `print()` prints output without moving to the next line.

---

### Statement 6

```java
System.out.print("Python");
```

Explanation:

* Prints Python immediately after Java.

Output:

```text
JavaPython
```

---

## Escape Sequences Used in This Program

| Escape Sequence | Description           |
| --------------- | --------------------- |
| `\n`            | New Line              |
| `\t`            | Horizontal Tab        |
| `\b`            | Backspace             |
| `\"`            | Double Quotation Mark |

---

## Difference Between print() and println()

### print()

```java
System.out.print("Java");
System.out.print("Python");
```

Output:

```text
JavaPython
```

The cursor remains on the same line.

---

### println()

```java
System.out.println("Java");
System.out.println("Python");
```

Output:

```text
Java
Python
```

The cursor moves to the next line after printing.

---

## Special Methods Used

### println()

**Syntax**

```java
System.out.println(data);
```

**Purpose**

* Prints output.
* Moves the cursor to the next line.

---

### print()

**Syntax**

```java
System.out.print(data);
```

**Purpose**

* Prints output.
* Does not move the cursor to the next line.

---

## Why Are Escape Sequences Used in Java?

Escape sequences are used to:

* Format console output.
* Insert new lines and tabs.
* Display quotation marks inside strings.
* Improve output readability.
* Control text formatting without writing additional code.

---

## Summary

This program demonstrates:

* New Line (`\n`)
* Tab Space (`\t`)
* Backspace (`\b`)
* Double Quotes (`\"`)
* Difference between `print()` and `println()`
* Formatted output in Java

Escape sequences are an important part of Java string handling and are frequently used in console applications and interview questions.
