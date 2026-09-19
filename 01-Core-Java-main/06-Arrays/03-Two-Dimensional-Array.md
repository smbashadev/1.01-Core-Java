# Two-Dimensional Array in Java

## Objective

A Two-Dimensional Array is used to store data in the form of rows and columns. It is mainly used to represent matrices, tables, spreadsheets, and tabular data.

---

## Definition

A Two-Dimensional Array is an array of arrays in Java. It stores data in row and column format.

### Syntax

```java
dataType[][] arrayName;
```

### Example

```java
int[][] matrix;

String[][] names;
```

---

## Java Program to Store Matrix Values using Scanner

```java
import java.util.Scanner; // Import Scanner class for user input

public class TwoDArrayDemo {

    public static void main(String[] args) {

        // Step 1: Create Scanner object to accept input
        Scanner sc = new Scanner(System.in);

        // Step 2: Ask user for number of rows
        System.out.println("Enter number of rows:");
        int rows = sc.nextInt();

        // Step 3: Ask user for number of columns
        System.out.println("Enter number of columns:");
        int cols = sc.nextInt();

        // Step 4: Declare a two-dimensional array
        int[][] matrix = new int[rows][cols];

        // Step 5: Read matrix elements using nested loops
        System.out.println("Enter elements of the matrix:");

        for(int i = 0; i < rows; i++) {

            for(int j = 0; j < cols; j++) {

                matrix[i][j] = sc.nextInt();

            }

        }

        // Step 6: Display matrix elements

        System.out.println("Matrix elements are:");

        for(int i = 0; i < rows; i++) {

            for(int j = 0; j < cols; j++) {

                System.out.print(matrix[i][j] + " ");

            }

            System.out.println();

        }

        // Step 7: Close Scanner object

        sc.close();

    }

}
```

---

## Sample Output

```text
Enter number of rows:
2

Enter number of columns:
3

Enter elements of the matrix:

1 2 3
4 5 6

Matrix elements are:

1 2 3
4 5 6
```

---

## Pseudocode

```text
START

Create Scanner object

Read rows

Read columns

Create matrix with rows and columns

FOR each row

    FOR each column

        Read matrix element

    END FOR

END FOR

Display matrix

FOR each row

    FOR each column

        Print matrix element

    END FOR

    Move to next line

END FOR

Close Scanner

STOP
```

---

## Line-by-Line Explanation

### `Scanner sc = new Scanner(System.in);`

Creates a Scanner object to read user input from the keyboard.

---

### `int rows = sc.nextInt();`

Reads the number of rows from the user.

---

### `int cols = sc.nextInt();`

Reads the number of columns from the user.

---

### `int[][] matrix = new int[rows][cols];`

Creates a Two-Dimensional Array with specified rows and columns.

Example:

```java
int[][] matrix = new int[2][3];
```

This creates:

```text
1st Row → [0][0] [0][1] [0][2]

2nd Row → [1][0] [1][1] [1][2]
```

---

### Nested For Loop

```java
for(int i=0;i<rows;i++)
{
    for(int j=0;j<cols;j++)
    {
        matrix[i][j]=sc.nextInt();
    }
}
```

Purpose:

* Outer loop controls rows.
* Inner loop controls columns.
* Reads every element of the matrix.

---

### Printing Matrix

```java
System.out.print(matrix[i][j] + " ");
```

Prints one matrix element.

```java
System.out.println();
```

Moves cursor to next line after printing one row.

---

## Why Nested Loops are Used?

A Two-Dimensional Array has:

* Rows
* Columns

Therefore:

* Outer loop → Traverses rows.
* Inner loop → Traverses columns.

Without nested loops, accessing every element becomes difficult.

---

## Array Memory Representation

For:

```java
int[][] matrix = new int[2][3];
```

Memory structure:

```text
Row 0 → [0][0] [0][1] [0][2]

Row 1 → [1][0] [1][1] [1][2]
```

Index Representation:

```text
matrix[0][0]

matrix[0][1]

matrix[0][2]

matrix[1][0]

matrix[1][1]

matrix[1][2]
```

---

## Special Methods Used

### nextInt()

```java
sc.nextInt();
```

Purpose:

Reads an integer value from the keyboard.

Example:

```java
int num = sc.nextInt();
```

---

### close()

```java
sc.close();
```

Purpose:

Closes Scanner object and releases system resources.

---

## Important Points

* Two-Dimensional Array is also called Matrix.
* Stores data in rows and columns.
* Index starts from 0.
* Uses nested loops for traversal.
* Arrays are fixed in size after creation.
* Can store only same data type elements.

---

## Real World Applications

Two-Dimensional Arrays are used in:

* Matrices
* Marks Table
* Excel Sheets
* Chess Board
* Image Processing
* Game Development
* Seating Arrangement Systems

---

## Summary

This program demonstrates:

* Two-Dimensional Arrays
* Matrix Creation
* Dynamic Array Size
* Nested Loops
* Scanner Input
* Matrix Traversal
* Row and Column Representation

Two-Dimensional Arrays are one of the most important concepts in Java because they are widely used to represent tabular and matrix-based data efficiently.
