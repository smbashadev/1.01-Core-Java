# Jagged Array in Java

## Objective

A Jagged Array is an array of arrays where each row can have a different number of elements.

This program demonstrates how to store student ages for different schools and classes where each class contains a different number of students.

---

## Definition

A Jagged Array is a multidimensional array in which each row can have a different size.

Unlike a regular multidimensional array, the number of columns is not fixed.

### Example

```java
int[][] jagged = {
    {10, 20},
    {30, 40, 50},
    {60}
};
```

Here,

- Row 1 contains 2 elements
- Row 2 contains 3 elements
- Row 3 contains 1 element

This is called a Jagged Array.

---

## Why Jagged Arrays are Required

Jagged Arrays are useful when:

- Different rows have different sizes.
- Memory should not be wasted by allocating unnecessary elements.
- Real-world data contains varying lengths.

Examples:

- Schools having different numbers of classes.
- Classes having different numbers of students.
- Departments having different numbers of employees.

---

## Program

```java
public class JaggedArray {

    public static void main(String[] args) {

        // Step 1: Declare a jagged array
        int[][][] ages = new int[2][][];

        // Step 2: Number of classes in each school
        ages[0] = new int[2][];
        ages[1] = new int[3][];

        // Step 3: Number of students in each class

        ages[0][0] = new int[2];
        ages[0][1] = new int[3];

        ages[1][0] = new int[2];
        ages[1][1] = new int[3];
        ages[1][2] = new int[4];

        // School 1 Class 1
        ages[0][0][0] = 14;
        ages[0][0][1] = 15;

        // School 1 Class 2
        ages[0][1][0] = 16;
        ages[0][1][1] = 17;
        ages[0][1][2] = 18;

        // School 2 Class 1
        ages[1][0][0] = 13;
        ages[1][0][1] = 14;

        // School 2 Class 2
        ages[1][1][0] = 15;
        ages[1][1][1] = 16;
        ages[1][1][2] = 17;

        // School 2 Class 3
        ages[1][2][0] = 18;
        ages[1][2][1] = 19;
        ages[1][2][2] = 20;
        ages[1][2][3] = 21;

        // Display School 1 Class 1
        System.out.println("School 1, Class 1 ages:");
        System.out.println(ages[0][0][0]);
        System.out.println(ages[0][0][1]);

        // Display School 1 Class 2
        System.out.println("School 1, Class 2 ages:");
        System.out.println(ages[0][1][0]);
        System.out.println(ages[0][1][1]);
        System.out.println(ages[0][1][2]);

        // Display School 2 Class 1
        System.out.println("School 2, Class 1 ages:");
        System.out.println(ages[1][0][0]);
        System.out.println(ages[1][0][1]);

        // Display School 2 Class 2
        System.out.println("School 2, Class 2 ages:");
        System.out.println(ages[1][1][0]);
        System.out.println(ages[1][1][1]);
        System.out.println(ages[1][1][2]);

        // Display School 2 Class 3
        System.out.println("School 2, Class 3 ages:");
        System.out.println(ages[1][2][0]);
        System.out.println(ages[1][2][1]);
        System.out.println(ages[1][2][2]);
        System.out.println(ages[1][2][3]);

    }
}
```

---

## Output

```text
School 1, Class 1 ages:
14
15

School 1, Class 2 ages:
16
17
18

School 2, Class 1 ages:
13
14

School 2, Class 2 ages:
15
16
17

School 2, Class 3 ages:
18
19
20
21
```

---

## Memory Representation

```text
ages[2][][]

School 1

    Class 1 -> [14, 15]

    Class 2 -> [16, 17, 18]


School 2

    Class 1 -> [13, 14]

    Class 2 -> [15, 16, 17]

    Class 3 -> [18, 19, 20, 21]
```

---

## Pseudocode

```text
START

Create jagged array ages[2][][]

School 1 has 2 classes
School 2 has 3 classes

Allocate students for each class

Store ages manually

Display all ages

STOP
```

---

## Line-by-Line Explanation

### 1.

```java
int[][][] ages = new int[2][][];
```

Creates a jagged array for 2 schools.

---

### 2.

```java
ages[0] = new int[2][];
ages[1] = new int[3][];
```

- School 1 contains 2 classes.
- School 2 contains 3 classes.

---

### 3.

```java
ages[0][0] = new int[2];
```

Class 1 of School 1 contains 2 students.

---

### 4.

```java
ages[0][1] = new int[3];
```

Class 2 of School 1 contains 3 students.

---

### 5.

```java
ages[1][2] = new int[4];
```

Class 3 of School 2 contains 4 students.

---

### 6.

```java
ages[0][0][0] = 14;
```

Stores age 14 in:

- School 1
- Class 1
- Student 1

---

### 7.

```java
System.out.println(ages[1][2][3]);
```

Displays:

```text
21
```

which means:

- School 2
- Class 3
- Student 4

---

## Why Do We Use Jagged Arrays in Java?

We use Jagged Arrays because:

- Every row can have different sizes.
- Memory is allocated only when required.
- Reduces memory wastage.
- Represents real-world hierarchical data efficiently.

Examples:

- Schools and Classes
- Employees and Departments
- Countries and States
- Students and Subjects

---

## Advantages

1. Saves memory.
2. Flexible row sizes.
3. Efficient memory allocation.
4. Suitable for irregular data.
5. Easy representation of hierarchical information.

---

## Disadvantages

1. More difficult than normal arrays.
2. Allocation is slightly complex.
3. Traversing requires careful handling.
4. Beginners may find it difficult initially.

---

## Important Points

- Jagged Array is an array of arrays.
- Each row may contain a different number of elements.
- Java treats jagged arrays as objects.
- Memory is allocated separately for each row.
- Jagged Arrays save memory compared to fixed multidimensional arrays.

---

## Summary

A Jagged Array is a multidimensional array in which rows can have different sizes.

In this example:

- School 1 has 2 classes.
- School 2 has 3 classes.
- Each class contains a different number of students.

Jagged Arrays are widely used when data size varies from one row to another and memory efficiency is important.
