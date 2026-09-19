# Search an Element in a Two-Dimensional Array in Java

## Objective

This program searches for a specific integer element in a Two-Dimensional Array (Matrix). The program accepts matrix elements from the user, searches for the required element, and displays whether the element is present or not.

---

## Definition

Searching in a Two-Dimensional Array means checking whether a particular value exists inside the matrix.

The program scans each element row by row and column by column until the element is found.

---

## Java Program

```java
import java.util.Scanner; // Import Scanner class for user input

public class SearchElement {

    public static void main(String[] args) {

        // Step 1: Create Scanner object for keyboard input
        Scanner sc = new Scanner(System.in);

        // Step 2: Ask user for number of rows
        System.out.println("Enter number of rows:");
        int rows = sc.nextInt();

        // Step 3: Ask user for number of columns
        System.out.println("Enter number of columns:");
        int cols = sc.nextInt();

        // Step 4: Declare a Two-Dimensional Array
        int[][] arr = new int[rows][cols];

        // Step 5: Accept array elements from the user

        System.out.println("Enter array elements:");

        for(int i = 0; i < rows; i++) {

            for(int j = 0; j < cols; j++) {

                arr[i][j] = sc.nextInt();

            }

        }

        // Step 6: Read the element to search

        System.out.println("Enter the element to search:");

        int key = sc.nextInt();

        // Step 7: Search the element using nested loops

        boolean found = false;

        for(int i = 0; i < rows; i++) {

            for(int j = 0; j < cols; j++) {

                if(arr[i][j] == key) {

                    found = true;

                    break;

                }

            }

            if(found) {

                break;

            }

        }

        // Step 8: Display the result

        if(found) {

            System.out.println("Element found in the 2D array.");

        }
        else {

            System.out.println("Element not found in the 2D array.");

        }

        // Step 9: Close Scanner object

        sc.close();

    }

}
```

---

## Sample Output

### Case 1 : Element Found

```text
Enter number of rows:
2

Enter number of columns:
3

Enter array elements:

1 2 3
4 5 6

Enter the element to search:

5

Element found in the 2D array.
```

### Case 2 : Element Not Found

```text
Enter number of rows:
2

Enter number of columns:
3

Enter array elements:

1 2 3
4 5 6

Enter the element to search:

10

Element not found in the 2D array.
```

---

## Pseudocode

```text
START

Create Scanner object

Read rows

Read columns

Create Two-Dimensional Array

Read matrix elements using nested loops

Read element to search

Set found = false

FOR each row

    FOR each column

        IF current element equals key

            found = true

            Exit inner loop

        END IF

    END FOR

    IF found

        Exit outer loop

    END IF

END FOR

IF found

    Display "Element found"

ELSE

    Display "Element not found"

END IF

Close Scanner

STOP
```

---

## Line-by-Line Explanation

### `Scanner sc = new Scanner(System.in);`

Creates a Scanner object to accept user input from the keyboard.

---

### `int rows = sc.nextInt();`

Reads the number of rows from the user.

---

### `int cols = sc.nextInt();`

Reads the number of columns from the user.

---

### `int[][] arr = new int[rows][cols];`

Creates a Two-Dimensional Array with user-defined rows and columns.

Example:

```java
int[][] arr = new int[2][3];
```

Creates:

```text
[0][0] [0][1] [0][2]

[1][0] [1][1] [1][2]
```

---

### Nested For Loop

```java
for(int i=0;i<rows;i++)
{
    for(int j=0;j<cols;j++)
    {
        arr[i][j]=sc.nextInt();
    }
}
```

Purpose:

* Outer loop traverses rows.
* Inner loop traverses columns.
* Reads all matrix elements.

---

### `boolean found = false;`

A flag variable used to determine whether the element is found.

Initially:

```java
boolean found = false;
```

Meaning:

Element is not found yet.

---

### Search Condition

```java
if(arr[i][j] == key)
```

Checks whether the current matrix element matches the search element.

If true:

```java
found = true;
```

The element is present in the matrix.

---

### `break;`

```java
break;
```

Terminates the loop immediately after the element is found.

This avoids unnecessary comparisons.

---

### Result Display

```java
if(found)
```

If found is true:

```text
Element found in the 2D array.
```

Otherwise:

```text
Element not found in the 2D array.
```

---

## Why Boolean Variable is Used?

The boolean variable:

```java
boolean found;
```

is used because:

* It stores only two values: true or false.
* It indicates whether the element is found.
* It helps terminate the search early.

---

## Time Complexity

```text
Best Case  : O(1)

Worst Case : O(rows × columns)

Average    : O(rows × columns)
```

---

## Important Points

* Uses nested loops for searching.
* Two-Dimensional Array stores data in rows and columns.
* Boolean variable is used as a search flag.
* break statement terminates loops early.
* Searching continues until the element is found or all elements are checked.

---

## Special Methods Used

### nextInt()

```java
sc.nextInt();
```

Reads integer input from the keyboard.

---

### close()

```java
sc.close();
```

Closes the Scanner object and releases system resources.

---

## Summary

This program demonstrates:

* Searching an element in a Two-Dimensional Array
* Matrix input using Scanner
* Nested loops
* Boolean flag technique
* break statement
* Search operation in matrices

Searching is one of the most important operations performed on arrays and is frequently asked in Java interviews and programming assessments.
