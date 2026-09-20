# Three-Dimensional Array in Java

## Objective

The Three-Dimensional Array is used to store data in three dimensions. In this example, the array stores information about:

* Schools
* Classes
* Students

The program stores and displays student names using hard-coded values without loops.

---

## Definition

A Three-Dimensional Array is an array of Two-Dimensional Arrays.

It stores data in three levels:

1. First Dimension → School
2. Second Dimension → Class
3. Third Dimension → Student

### Syntax

```java
datatype[][][] arrayName = new datatype[size1][size2][size3];
```

### Example

```java
String[][][] schoolData = new String[2][2][3];
```

This means:

* 2 Schools
* 2 Classes in each School
* 3 Students in each Class

---

## Java Program

```java
public class ThreeDArrayDemo {

    public static void main(String[] args) {

        // Step 1: Declare a 3D array
        String[][][] schoolData = new String[2][2][3];

        // School 1 - Class 1
        schoolData[0][0][0] = "Aman";
        schoolData[0][0][1] = "Riya";
        schoolData[0][0][2] = "Karan";

        // School 1 - Class 2
        schoolData[0][1][0] = "Neha";
        schoolData[0][1][1] = "Rahul";
        schoolData[0][1][2] = "Meera";

        // School 2 - Class 1
        schoolData[1][0][0] = "Arjun";
        schoolData[1][0][1] = "Sita";
        schoolData[1][0][2] = "Vikram";

        // School 2 - Class 2
        schoolData[1][1][0] = "Pooja";
        schoolData[1][1][1] = "Ankit";
        schoolData[1][1][2] = "Deepa";

        // Display values

        System.out.println("School 1, Class 1 students:");
        System.out.println(schoolData[0][0][0]);
        System.out.println(schoolData[0][0][1]);
        System.out.println(schoolData[0][0][2]);

        System.out.println("School 1, Class 2 students:");
        System.out.println(schoolData[0][1][0]);
        System.out.println(schoolData[0][1][1]);
        System.out.println(schoolData[0][1][2]);

        System.out.println("School 2, Class 1 students:");
        System.out.println(schoolData[1][0][0]);
        System.out.println(schoolData[1][0][1]);
        System.out.println(schoolData[1][0][2]);

        System.out.println("School 2, Class 2 students:");
        System.out.println(schoolData[1][1][0]);
        System.out.println(schoolData[1][1][1]);
        System.out.println(schoolData[1][1][2]);

    }

}
```

---

## Output

```text
School 1, Class 1 students:
Aman
Riya
Karan

School 1, Class 2 students:
Neha
Rahul
Meera

School 2, Class 1 students:
Arjun
Sita
Vikram

School 2, Class 2 students:
Pooja
Ankit
Deepa
```

---

## Memory Representation

```text
schoolData[2][2][3]

School 0

    Class 0
        Aman
        Riya
        Karan

    Class 1
        Neha
        Rahul
        Meera


School 1

    Class 0
        Arjun
        Sita
        Vikram

    Class 1
        Pooja
        Ankit
        Deepa
```

---

## Pseudocode

```text
START

Create a 3D array schoolData[2][2][3]

Store student names for:

School 1
    Class 1
    Class 2

School 2
    Class 1
    Class 2

Display all stored names

STOP
```

---

## Line-by-Line Explanation

### Declaration

```java
String[][][] schoolData = new String[2][2][3];
```

Creates a Three-Dimensional Array.

* First Dimension → 2 Schools
* Second Dimension → 2 Classes
* Third Dimension → 3 Students

---

### Storing Values

```java
schoolData[0][0][0] = "Aman";
```

Meaning:

```text
School 1
Class 1
Student 1 = Aman
```

---

```java
schoolData[0][0][1] = "Riya";
```

Meaning:

```text
School 1
Class 1
Student 2 = Riya
```

---

```java
schoolData[1][1][2] = "Deepa";
```

Meaning:

```text
School 2
Class 2
Student 3 = Deepa
```

---

## Understanding Indices

```text
schoolData[school][class][student]
```

Example:

```java
schoolData[0][1][2]
```

Means:

```text
School 1
Class 2
Student 3
```

Value:

```text
Meera
```

---

## Advantages of Three-Dimensional Arrays

* Stores data in multiple dimensions.
* Organizes hierarchical information.
* Useful for School → Class → Student data.
* Faster access using indexes.
* Supports structured storage.

---

## Disadvantages

* Difficult to understand for beginners.
* Memory usage increases with dimensions.
* Manual handling becomes complex.
* Nested loops are usually required for larger datasets.

---

## Important Points

* Three-Dimensional Array is an array of Two-Dimensional Arrays.
* Indexing starts from 0.
* The first index represents School.
* The second index represents Class.
* The third index represents Student.
* Java stores arrays as objects.

---

## Summary

A Three-Dimensional Array stores data in three levels.

In this example:

* First Dimension → School
* Second Dimension → Class
* Third Dimension → Student

The program demonstrates storing and displaying student names using hard-coded values without loops. Three-Dimensional Arrays are useful when working with hierarchical or layered data structures.
