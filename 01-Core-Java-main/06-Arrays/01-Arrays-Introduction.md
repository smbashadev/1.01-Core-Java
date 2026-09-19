# Arrays in Java

## Objective

This file introduces the concept of **Arrays in Java**.

An array is one of the most important data structures in Java used to store multiple values of the same data type using a single variable name.

Arrays are widely used in:

* Storing marks of students
* Employee records
* Matrix operations
* Searching algorithms
* Sorting algorithms
* Collections Framework internally

---

# 1. Definition of Array

An **Array** is a data structure that stores multiple values of the **same data type** in contiguous memory locations.

In Java:

* Arrays are objects.
* Each element is stored at a unique index.
* Index starts from `0`.

### Example

```java
int[] numbers = {10, 20, 30, 40};
```

Memory Representation:

```text
Index :   0    1    2    3

Value :  10   20   30   40
```

---

# 2. Why Arrays are Required

Suppose we want to store marks of 5 students.

Without Arrays:

```java
int mark1 = 80;
int mark2 = 90;
int mark3 = 70;
int mark4 = 85;
int mark5 = 95;
```

Problems:

* Too many variables
* Difficult to manage
* Difficult to process using loops

With Arrays:

```java
int[] marks = {80, 90, 70, 85, 95};
```

Now:

```java
System.out.println(marks[0]);
```

Output:

```text
80
```

Advantages:

* Single variable stores multiple values.
* Easy to process using loops.
* Memory management becomes easier.

---

# 3. Advantages of Arrays

### 1. Store Multiple Values

Stores many values using a single variable.

Example:

```java
int[] numbers = {10,20,30,40,50};
```

---

### 2. Fast Access

Elements are accessed directly using index.

Example:

```java
numbers[2]
```

Output:

```text
30
```

---

### 3. Efficient Memory Usage

Array elements are stored continuously in memory.

This improves:

* Access speed
* Performance

---

### 4. Easy Traversal

Arrays can easily be traversed using loops.

Example:

```java
for(int i=0;i<numbers.length;i++){

    System.out.println(numbers[i]);

}
```

---

### 5. Useful in Algorithms

Arrays are used in:

* Searching
* Sorting
* Matrix Operations
* Dynamic Programming

---

# 4. Disadvantages of Arrays

### 1. Fixed Size

Once created:

```java
int[] arr = new int[5];
```

Size cannot be changed.

---

### 2. Same Data Type Only

Valid:

```java
int[] arr = {10,20,30};
```

Invalid:

```java
int[] arr = {10,"Java",20};
```

Because:

```text
Different data types are not allowed.
```

---

### 3. Insertion is Difficult

If an element is inserted:

```text
Remaining elements need shifting.
```

---

### 4. Memory Wastage

If:

```java
int[] arr = new int[100];
```

And only:

```text
10 elements are used
```

Then:

```text
90 memory locations remain unused.
```

---

# 5. Syntax of Array Declaration

### General Syntax

```java
DataType[] arrayName;
```

Examples:

```java
int[] age;

String[] names;

double[] salary;
```

---

# 6. Array Initialization

Arrays can be initialized in two ways.

---

## Method 1: Declaration + Initialization

```java
int[] numbers = {1,2,3,4};
```

Memory:

```text
Index : 0 1 2 3

Value : 1 2 3 4
```

---

## Method 2: Using new Keyword

```java
int[] numbers = new int[4];

numbers[0] = 10;

numbers[1] = 20;

numbers[2] = 30;

numbers[3] = 40;
```

Output:

```text
10 20 30 40
```

---

# 7. Accessing Array Elements

Each element is accessed using:

```text
Index
```

Index starts from:

```text
0
```

Example:

```java
int[] numbers = {10,20,30};

System.out.println(numbers[0]);

System.out.println(numbers[2]);
```

Output:

```text
10

30
```

---

# Memory Representation

```text
numbers

Index

0    1    2

↓

10   20   30
```

---

# 8. Length Property

The `length` property returns:

```text
Number of elements present in the array
```

Example:

```java
int[] numbers = {5,10,15,20};

System.out.println(numbers.length);
```

Output:

```text
4
```

Explanation:

```text
Array contains four elements.

Hence length = 4.
```

---

# Important Points

1. Arrays are objects in Java.

2. Index starts from:

```text
0
```

3. Arrays store:

```text
Homogeneous Data

(Same Data Type)
```

4. Size is fixed after creation.

5. Array length can be obtained using:

```java
arrayName.length
```

---

# Real Time Examples

### Student Marks

```java
int[] marks = {80,90,70,85,95};
```

---

### Employee IDs

```java
int[] empIds = {101,102,103,104};
```

---

### Names of Students

```java
String[] names = {"Rahul","Anil","John"};
```

---

# Summary

Arrays are used to store multiple values of the same data type.

They provide:

* Fast access using index
* Easy traversal using loops
* Better memory organization
* Efficient data management

Arrays form the foundation for advanced data structures such as:

* ArrayList
* Stack
* Queue
* Matrix
* Collections Framework

Therefore, Arrays are one of the most important topics in Core Java and are frequently asked in interviews.
