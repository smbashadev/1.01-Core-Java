# Control Statements in Java - Interview Questions and Answers

## Q1. What are control statements in Java?

**Answer:**

Control statements are used to control the flow of execution of a Java program.

They are mainly divided into:

1. Decision Making Statements
2. Looping Statements
3. Jump Statements

---

## Q2. What are decision making statements?

**Answer:**

Decision making statements are used to execute code based on conditions.

Examples:

* if
* if else
* else if ladder
* nested if
* switch

---

## Q3. What are looping statements?

**Answer:**

Looping statements are used to execute a block of code repeatedly.

Examples:

* for loop
* while loop
* do while loop

---

## Q4. What are jump statements?

**Answer:**

Jump statements are used to transfer control from one place to another.

Examples:

* break
* continue

---

# if Statement

## Q5. What is an if statement?

**Answer:**

The `if` statement executes a block of code only when the condition is true.

**Syntax**

```java
if(condition){
   statements;
}
```

---

## Q6. What type of expression is used in if?

**Answer:**

Boolean expression.

Example:

```java
if(age >= 18)
```

---

## Q7. What happens if the condition is false?

**Answer:**

The code inside the if block is skipped.

---

# if else Statement

## Q8. What is if else statement?

**Answer:**

It executes one block if the condition is true and another block if the condition is false.

**Syntax**

```java
if(condition){

}
else{

}
```

---

## Q9. When do we use if else?

**Answer:**

When there are exactly two possible outcomes.

Examples:

* Even or Odd
* Pass or Fail

---

# Else If Ladder

## Q10. What is else if ladder?

**Answer:**

It is used to check multiple conditions one by one.

Example:

```java
if(){

}
else if(){

}
else if(){

}
else{

}
```

---

## Q11. Does Java execute all else if conditions?

**Answer:**

No.

Once a condition becomes true, the remaining conditions are skipped.

---

## Q12. Which programs commonly use else if ladder?

**Answer:**

* Grade Calculation
* Greatest of Three Numbers
* Menu Driven Programs

---

# Nested if

## Q13. What is nested if?

**Answer:**

An if statement inside another if statement is called nested if.

Example:

```java
if(age >= 18){

    if(weight > 50){

    }

}
```

---

## Q14. When is nested if used?

**Answer:**

When one condition depends on another condition.

---

# Switch Statement

## Q15. What is switch statement?

**Answer:**

The switch statement selects one block of code among many options.

**Syntax**

```java
switch(expression){

    case value:
        break;

    default:

}
```

---

## Q16. Which data types are allowed in switch?

**Answer:**

* byte
* short
* int
* char
* String
* enum

---

## Q17. What is default case?

**Answer:**

The default block executes when no case matches.

---

## Q18. Why is break used in switch?

**Answer:**

The break statement stops execution of remaining cases.

---

## Q19. What happens if break is omitted?

**Answer:**

Control falls through to the next case.

This is called:

**Fall Through**

---

# For Loop

## Q20. What is for loop?

**Answer:**

A for loop repeats a block of code a fixed number of times.

**Syntax**

```java
for(initialization;
    condition;
    increment){

}
```

---

## Q21. Which parts are present in for loop?

**Answer:**

1. Initialization
2. Condition
3. Increment or Decrement

---

## Q22. When is for loop preferred?

**Answer:**

When the number of iterations is known in advance.

---

# While Loop

## Q23. What is while loop?

**Answer:**

The while loop executes repeatedly as long as the condition is true.

**Syntax**

```java
while(condition){

}
```

---

## Q24. When is while loop preferred?

**Answer:**

When the number of iterations is not known in advance.

---

## Q25. Is condition checked before execution in while?

**Answer:**

Yes.

The while loop is an **Entry Controlled Loop**.

---

# Do While Loop

## Q26. What is do while loop?

**Answer:**

The do while loop executes the block first and checks the condition later.

**Syntax**

```java
do{

}while(condition);
```

---

## Q27. How many times does do while execute at minimum?

**Answer:**

At least one time.

---

## Q28. Why?

**Answer:**

Because the condition is checked after executing the loop body.

---

## Q29. Which loops are called entry controlled loops?

**Answer:**

* for loop
* while loop

---

## Q30. Which loop is called exit controlled loop?

**Answer:**

The do while loop.

---

# Break Statement

## Q31. What is break statement?

**Answer:**

The break statement immediately terminates the loop or switch statement.

---

## Q32. Where can break be used?

**Answer:**

* for loop
* while loop
* do while loop
* switch statement

---

## Q33. What is the use of break?

**Answer:**

To stop execution when a condition is satisfied.

---

# Continue Statement

## Q34. What is continue statement?

**Answer:**

The continue statement skips the current iteration and moves to the next iteration.

---

## Q35. Does continue stop the loop?

**Answer:**

No.

It only skips the current iteration.

---

## Q36. Difference between break and continue?

**Answer:**

### break

* Terminates the loop completely.
* Control moves outside the loop.

### continue

* Skips only the current iteration.
* Control moves to the next iteration.

---

## Q37. Which control statement is better for menu driven programs?

**Answer:**

The switch statement.

---

## Q38. Which loop is most commonly used?

**Answer:**

The for loop.

---

## Q39. Which loop executes at least once?

**Answer:**

The do while loop.

---

## Q40. Which control statement topics are frequently asked in interviews?

**Answer:**

* if vs switch
* else if ladder
* Nested if
* for loop
* while loop
* do while loop
* break statement
* continue statement
* Entry controlled loop
* Exit controlled loop

---

# Summary

This interview file covers:

* Decision Making Statements
* if, if else, else if, nested if
* Switch Statement
* for Loop
* while Loop
* do while Loop
* Break Statement
* Continue Statement
* Entry Controlled Loop
* Exit Controlled Loop

These are among the most frequently asked Core Java interview topics for freshers and Java Full Stack Developer roles.
