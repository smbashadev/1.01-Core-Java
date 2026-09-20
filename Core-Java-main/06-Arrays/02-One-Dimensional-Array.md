# One-Dimensional Array in Java

## Objective

A One-Dimensional Array is used to store multiple values of the same data type in a single row. It helps organize data efficiently and allows accessing elements using index values.

---

## Definition

A One-Dimensional Array is a linear collection of elements of the same data type stored in contiguous memory locations.

**Syntax**

```java
dataType[] arrayName;
```

**Example**

```java
int[] numbers;
String[] names;
```

---

# Java Program

```java
import java.util.Scanner; // Import Scanner class for user input

public class OneDArrayDemo {

    public static void main(String[] args) {

        // Hard Coding without Loop

        String[] names = new String[5]; // Create String array of size 5

        names[0] = "Aman";
        names[1] = "Riya";
        names[2] = "Karan";
        names[3] = "Neha";
        names[4] = "Rahul";

        System.out.println("Names using hard coding without loop:");

        System.out.println(names[0]);
        System.out.println(names[1]);
        System.out.println(names[2]);
        System.out.println(names[3]);
        System.out.println(names[4]);

        int[] ages = new int[5]; // Create integer array

        ages[0] = 18;
        ages[1] = 19;
        ages[2] = 20;
        ages[3] = 21;
        ages[4] = 22;

        System.out.println("Ages using hard coding without loop:");

        System.out.println(ages[0]);
        System.out.println(ages[1]);
        System.out.println(ages[2]);
        System.out.println(ages[3]);
        System.out.println(ages[4]);

        // Soft Coding without Loop

        Scanner sc = new Scanner(System.in);

        String[] softNames = new String[5];

        System.out.println("Enter 5 student names:");

        softNames[0] = sc.nextLine();
        softNames[1] = sc.nextLine();
        softNames[2] = sc.nextLine();
        softNames[3] = sc.nextLine();
        softNames[4] = sc.nextLine();

        System.out.println("Names using soft coding without loop:");

        System.out.println(softNames[0]);
        System.out.println(softNames[1]);
        System.out.println(softNames[2]);
        System.out.println(softNames[3]);
        System.out.println(softNames[4]);

        int[] softAges = new int[5];

        System.out.println("Enter 5 student ages:");

        softAges[0] = sc.nextInt();
        softAges[1] = sc.nextInt();
        softAges[2] = sc.nextInt();
        softAges[3] = sc.nextInt();
        softAges[4] = sc.nextInt();

        System.out.println("Ages using soft coding without loop:");

        System.out.println(softAges[0]);
        System.out.println(softAges[1]);
        System.out.println(softAges[2]);
        System.out.println(softAges[3]);
        System.out.println(softAges[4]);

        sc.nextLine(); // Consume newline

        // Hard Coding with Loop

        String[] loopNames = new String[5];

        String[] hardNameList = {
            "Aman",
            "Riya",
            "Karan",
            "Neha",
            "Rahul"
        };

        for(int i=0;i<hardNameList.length;i++) {
            loopNames[i] = hardNameList[i];
        }

        System.out.println("Names using hard coding with loop:");

        for(int i=0;i<loopNames.length;i++) {
            System.out.println(loopNames[i]);
        }

        int[] loopAges = new int[5];

        int[] hardAgeList = {18,19,20,21,22};

        for(int i=0;i<hardAgeList.length;i++) {
            loopAges[i] = hardAgeList[i];
        }

        System.out.println("Ages using hard coding with loop:");

        for(int i=0;i<loopAges.length;i++) {
            System.out.println(loopAges[i]);
        }

        // Soft Coding with Loop

        System.out.println("Enter 5 student names for loop input:");

        for(int i=0;i<5;i++) {
            loopNames[i] = sc.nextLine();
        }

        System.out.println("Names using soft coding with loop:");

        for(int i=0;i<loopNames.length;i++) {
            System.out.println(loopNames[i]);
        }

        System.out.println("Enter 5 student ages for loop input:");

        for(int i=0;i<5;i++) {
            loopAges[i] = sc.nextInt();
        }

        System.out.println("Ages using soft coding with loop:");

        for(int i=0;i<loopAges.length;i++) {
            System.out.println(loopAges[i]);
        }

        sc.close(); // Close Scanner
    }
}
```

---

## Pseudocode

```text
START

Create String array names
Store names manually
Display names

Create int array ages
Store ages manually
Display ages

Create Scanner object

Take names from user
Display names

Take ages from user
Display ages

Store values using loop
Display values using loop

Take values using loop from user
Display them

Close Scanner

STOP
```

---

## Line-by-Line Explanation

### `String[] names = new String[5];`

Creates a String array capable of storing 5 names.

### `names[0] = "Aman";`

Stores the value `"Aman"` at index 0.

### `int[] ages = new int[5];`

Creates an integer array to store ages.

### `Scanner sc = new Scanner(System.in);`

Creates a Scanner object to read user input from the keyboard.

### `softNames[0] = sc.nextLine();`

Reads one String value from the user.

### `softAges[0] = sc.nextInt();`

Reads one integer value from the user.

### `for(int i=0;i<array.length;i++)`

Traverses the array from first element to last element.

### `array.length`

Returns the size of the array.

### `sc.close();`

Closes the Scanner object and releases system resources.

---

## Important Points

* Arrays store elements of the same data type.
* Array index starts from **0**.
* Arrays have fixed size.
* `array.length` returns total size.
* One-dimensional array stores elements in a single row.
* Arrays are objects in Java.

---

## Special Methods / Properties Used

### length Property

```java
array.length
```

Returns total number of elements in the array.

Example:

```java
int[] arr = {10,20,30};

System.out.println(arr.length);
```

Output:

```text
3
```

---

### nextLine()

Reads a complete String input.

```java
String name = sc.nextLine();
```

---

### nextInt()

Reads integer input.

```java
int age = sc.nextInt();
```

---

### close()

Closes Scanner object.

```java
sc.close();
```

---

## Summary

This program demonstrates:

* One-Dimensional Arrays
* Hard Coding without Loop
* Soft Coding without Loop
* Hard Coding with Loop
* Soft Coding with Loop
* Array Traversal
* Scanner Input
* Array Length Property

One-Dimensional Arrays are widely used to store and process collections of similar data efficiently in Java.
