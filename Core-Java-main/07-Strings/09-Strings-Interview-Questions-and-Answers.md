# Strings Interview Questions and Answers

## Q1. What is String in Java?

**Answer:**

A String in Java is a sequence of characters used to store text.

Example:

```java
String name = "Java";
```

---

## Q2. Is String a primitive data type in Java?

**Answer:**

No.

String is a non-primitive or reference data type.

---

## Q3. Is String a class in Java?

**Answer:**

Yes.

String is a predefined final class available in the `java.lang` package.

---

## Q4. What are the different ways to create a String?

**Answer:**

There are three ways:

### 1. Using String Literal

```java
String s = "Java";
```

### 2. Using new keyword

```java
String s = new String("Java");
```

### 3. Using Character Array

```java
char[] ch = {'J','a','v','a'};

String s = new String(ch);
```

---

## Q5. What is String Literal?

**Answer:**

A String created using double quotes is called String Literal.

Example:

```java
String s = "Java";
```

It is stored in the String Pool.

---

## Q6. What is String Pool?

**Answer:**

String Pool is a special memory area inside Heap memory where String literals are stored.

It avoids creating duplicate String objects.

---

## Q7. What is the difference between:

```java
String s1 = "Java";

String s2 = new String("Java");
```

**Answer:**

- `s1` is stored in String Pool.
- `s2` creates a new object in Heap memory.

---

## Q8. What is immutable String?

**Answer:**

Immutable means the value cannot be changed after creation.

Example:

```java
String s = "Java";

s = s + " Programming";
```

A new object is created.

---

## Q9. Why is String immutable?

**Answer:**

Because of:

- Security
- Thread Safety
- String Pool optimization
- Caching of hash values

---

## Q10. What is the difference between `==` and `equals()`?

**Answer:**

### `==`

Compares references.

### `equals()`

Compares content.

Example:

```java
String s1 = "Java";

String s2 = new String("Java");

System.out.println(s1 == s2);       // false

System.out.println(s1.equals(s2));  // true
```

---

## Q11. What is `intern()` method?

**Answer:**

`intern()` returns the String object from the String Pool.

Example:

```java
String s1 = new String("Java");

String s2 = s1.intern();
```

---

## Q12. What is the output?

```java
String s1 = "Java";

String s2 = "Java";

System.out.println(s1 == s2);
```

**Answer:**

```text
true
```

Because both refer to the same String Pool object.

---

## Q13. What is the output?

```java
String s1 = new String("Java");

String s2 = new String("Java");

System.out.println(s1 == s2);
```

**Answer:**

```text
false
```

Because both are different Heap objects.

---

## Q14. What does `length()` method do?

**Answer:**

Returns the total number of characters.

Example:

```java
String s = "Java";

System.out.println(s.length());
```

Output:

```text
4
```

---

## Q15. What does `charAt()` method do?

**Answer:**

Returns the character at a specified index.

Example:

```java
String s = "Java";

System.out.println(s.charAt(0));
```

Output:

```text
J
```

---

## Q16. What does `toUpperCase()` method do?

**Answer:**

Converts all characters into uppercase.

Example:

```java
String s = "java";

System.out.println(s.toUpperCase());
```

Output:

```text
JAVA
```

---

## Q17. What does `toLowerCase()` method do?

**Answer:**

Converts all characters into lowercase.

Example:

```java
String s = "JAVA";

System.out.println(s.toLowerCase());
```

Output:

```text
java
```

---

## Q18. What does `trim()` method do?

**Answer:**

Removes spaces from the beginning and end of the String.

Example:

```java
String s = "  Java  ";

System.out.println(s.trim());
```

Output:

```text
Java
```

---

## Q19. What does `substring()` method do?

**Answer:**

Returns a part of the String.

Example:

```java
String s = "Java Programming";

System.out.println(s.substring(0,4));
```

Output:

```text
Java
```

---

## Q20. What does `replace()` method do?

**Answer:**

Replaces characters or words.

Example:

```java
String s = "Java";

System.out.println(s.replace('a','@'));
```

Output:

```text
J@v@
```

---

## Q21. What does `contains()` method do?

**Answer:**

Checks whether the String contains a given sequence.

Example:

```java
String s = "Java Programming";

System.out.println(s.contains("Java"));
```

Output:

```text
true
```

---

## Q22. What does `startsWith()` method do?

**Answer:**

Checks whether a String starts with a specific prefix.

Example:

```java
String s = "Java";

System.out.println(s.startsWith("Ja"));
```

Output:

```text
true
```

---

## Q23. What does `endsWith()` method do?

**Answer:**

Checks whether a String ends with a specific suffix.

Example:

```java
String s = "Java";

System.out.println(s.endsWith("va"));
```

Output:

```text
true
```

---

## Q24. What does `split()` method do?

**Answer:**

Splits a String into multiple parts.

Example:

```java
String s = "Java,Python,C";

String[] arr = s.split(",");
```

Output:

```text
Java
Python
C
```

---

## Q25. What is a Palindrome String?

**Answer:**

A String that reads the same from left to right and right to left.

Examples:

```text
madam
racecar
level
malayalam
```

---

## Q26. How do you check whether a String is palindrome?

**Answer:**

- Reverse the String.
- Compare original and reversed String using `equals()`.

Example:

```java
if(original.equals(reverse))
{
    System.out.println("Palindrome");
}
```

---

## Q27. What is StringBuffer?

**Answer:**

StringBuffer is a mutable class.

Its contents can be modified.

It is:

- Mutable
- Thread Safe
- Synchronized

---

## Q28. What is StringBuilder?

**Answer:**

StringBuilder is also mutable.

It is:

- Mutable
- Not Thread Safe
- Faster than StringBuffer

---

## Q29. Difference between String, StringBuffer and StringBuilder?

| String | StringBuffer | StringBuilder |
|--------|--------------|--------------|
| Immutable | Mutable | Mutable |
| Slow | Faster | Fastest |
| Thread Safe | Yes | No |
| Synchronized | No | Yes |

---

## Q30. Which String topics are frequently asked in interviews?

**Answer:**

- String Literal
- String Pool
- Heap Memory
- Immutable String
- equals() vs ==
- intern() Method
- String Methods
- split() Method
- Palindrome String
- StringBuffer
- StringBuilder
- Difference between String, StringBuffer and StringBuilder
