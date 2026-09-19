# Interview Questions and Answers

## Methods in Java

### Q1. What is a Method in Java?

**Answer:**

A Method is a block of code written to perform a specific task. It can be called whenever required.

---

### Q2. Why are Methods used?

**Answer:**

Methods are used because:

* Code Reusability
* Reduces Code Duplication
* Improves Readability
* Simplifies Debugging
* Makes Maintenance Easier
* Supports Modular Programming

---

### Q3. What are the two types of Methods in Java?

**Answer:**

There are two types of methods:

1. Predefined Methods
2. User Defined Methods

---

### Q4. What are Predefined Methods?

**Answer:**

Methods already defined by Java are called Predefined Methods.

**Examples:**

```java
System.out.println();

System.out.print();

equals();

toLowerCase();

toUpperCase();

length();
```

---

### Q5. What are User Defined Methods?

**Answer:**

Methods created by the programmer according to application requirements are called User Defined Methods.

---

### Q6. Which method is automatically called by JVM?

**Answer:**

```java
public static void main(String[] args)
```

The JVM automatically calls the `main()` method when the program starts.

---

### Q7. What is the Syntax of a Method?

**Answer:**

```java
returnType methodName(parameters){

    // Statements

}
```

**Example:**

```java
public static void display(){

}
```

---

# Types of Methods

### Q8. How many types of Methods are there based on syntax?

**Answer:**

There are four types:

1. No Return Type No Argument
2. No Return Type With Argument
3. Return Type No Argument
4. Return Type With Argument

---

## No Return Type No Argument

### Q9. What is a No Return Type No Argument Method?

**Answer:**

It does not accept parameters and does not return any value.

**Example:**

```java
void display(){

System.out.println("Hello");

}
```

---

### Q10. Which keyword is used when a method does not return any value?

**Answer:**

```java
void
```

---

## No Return Type With Argument

### Q11. What is a No Return Type With Argument Method?

**Answer:**

The method accepts parameters but does not return any value.

**Example:**

```java
void show(int a){

System.out.println(a);

}
```

---

### Q12. What is a Parameter?

**Answer:**

A Parameter is a variable declared inside the method definition.

**Example:**

```java
void add(int a,int b)
```

Here:

```text
a

b
```

are parameters.

---

### Q13. What is an Argument?

**Answer:**

An Argument is the actual value passed during method calling.

**Example:**

```java
add(10,20);
```

Here:

```text
10

20
```

are arguments.

---

## Return Type No Argument

### Q14. What is a Return Type No Argument Method?

**Answer:**

It returns a value but does not accept parameters.

**Example:**

```java
int getNumber(){

return 100;

}
```

---

### Q15. Which keyword is used to return a value?

**Answer:**

```java
return
```

**Example:**

```java
return sum;
```

---

### Q16. Can a void Method return a value?

**Answer:**

No.

A `void` method cannot return any value.

---

## Return Type With Argument

### Q17. What is a Return Type With Argument Method?

**Answer:**

The method accepts parameters and returns a value.

**Example:**

```java
int add(int a,int b){

return a+b;

}
```

---

### Q18. What is the output?

```java
int result = add(10,20);

System.out.println(result);
```

**Answer:**

```text
30
```

---

### Q19. Is return statement mandatory in non-void methods?

**Answer:**

Yes.

A method having a return type must return a value.

---

# Method Overloading

### Q20. What is Method Overloading?

**Answer:**

Method Overloading means defining multiple methods with the same name but different parameter lists in the same class.

---

### Q21. On what basis does Java differentiate overloaded methods?

**Answer:**

Java differentiates overloaded methods by:

* Number of Parameters
* Data Type of Parameters
* Order of Parameters

---

### Q22. Can methods be overloaded by changing only return type?

**Answer:**

No.

Changing only the return type is **not** Method Overloading.

Incorrect Example:

```java
int add(){

}

double add(){

}
```

This causes a compilation error.

---

### Q23. Give an example of Method Overloading.

**Answer:**

```java
add(int a,int b)

add(int a,int b,int c)

add(double a,double b)
```

---

### Q24. What is Compile Time Polymorphism?

**Answer:**

Method Overloading is called Compile Time Polymorphism because the compiler decides which method to call during compilation.

---

### Q25. Can main() method be overloaded?

**Answer:**

Yes.

The `main()` method can be overloaded.

**Example:**

```java
public static void main(){

}

public static void main(int a){

}
```

However, JVM calls only:

```java
public static void main(String[] args)
```

---

### Q26. Difference between Method Overloading and Method Overriding?

| Method Overloading        | Method Overriding      |
| ------------------------- | ---------------------- |
| Same Class                | Parent and Child Class |
| Same Method Name          | Same Method Name       |
| Different Parameters      | Same Parameters        |
| Compile Time Polymorphism | Runtime Polymorphism   |

---

### Q27. What is Method Signature?

**Answer:**

Method Name + Parameter List is called Method Signature.

**Example:**

```java
add(int,int)
```

---

### Q28. Can methods have multiple parameters?

**Answer:**

Yes.

**Example:**

```java
void display(String name,int age,double salary)
```

---

### Q29. Can one method call another method?

**Answer:**

Yes.

**Example:**

```java
public static void main(String[] args){

display();

}
```

---

### Q30. Why are Methods important in Java?

**Answer:**

Methods are important because they:

* Reuse Code
* Reduce Code Duplication
* Improve Readability
* Simplify Maintenance
* Make Programs Modular
* Improve Code Organization

---

### Q31. Which Method topics are frequently asked in Java Interviews?

**Answer:**

* Types of Methods
* Predefined and User Defined Methods
* Parameters and Arguments
* Return Keyword
* void Keyword
* Method Overloading
* Method Signature
* main() Method
* Compile Time Polymorphism
* Method Overriding
* Difference Between Overloading and Overriding

These are among the most frequently asked Core Java interview questions.
