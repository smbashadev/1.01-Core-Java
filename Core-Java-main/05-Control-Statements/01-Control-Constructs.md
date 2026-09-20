# Control Constructs in Java

## Objective

Control Constructs are used to control the flow of execution of statements in a Java program.

They determine:

* Which statement should execute.
* How many times a statement should execute.
* Under what condition a statement should execute.

Control Constructs make programs dynamic and intelligent by allowing decision making and repetition of statements.

---

# What are Control Constructs?

Control Constructs are statements that change the normal sequential execution of a Java program.

Without control constructs:

```text
Statement 1

↓

Statement 2

↓

Statement 3

↓

Statement 4
```

Execution happens one after another.

With Control Constructs:

```text
Condition

↓

True → Execute Block 1

False → Execute Block 2
```

or

```text
Repeat

↓

Until condition becomes false
```

---

# Types of Control Constructs

There are two major types:

### 1. Decision Making Statements

Used to make decisions based on conditions.

They include:

* if statement
* if-else statement
* else-if ladder
* Nested if statement
* switch statement

---

### 2. Looping Statements

Used to repeat a block of code multiple times.

They include:

* for loop
* while loop
* do-while loop

---

### 3. Jump Statements

Used to transfer control from one place to another.

They include:

* break statement
* continue statement

---

# 1. if Statement

## Definition

The `if` statement executes a block of code only when the condition is true.

---

## Syntax

```java
if(condition){

    // statements

}
```

---

## Example

```java
int age = 20;

if(age >= 18){

System.out.println("You are eligible to vote.");

}
```

---

## Output

```text
You are eligible to vote.
```

---

## Execution Flow

```text
Condition age>=18

↓

True

↓

Print Eligible to Vote

↓

End
```

---

# 2. if-else Statement

## Definition

The if-else statement executes:

* One block when condition is true.
* Another block when condition is false.

---

## Syntax

```java
if(condition){

// True Block

}

else{

// False Block

}
```

---

## Example

```java
int number = 10;

if(number%2==0){

System.out.println("Even Number");

}

else{

System.out.println("Odd Number");

}
```

---

## Output

```text
Even Number
```

---

## Execution Flow

```text
number%2==0

↓

True

↓

Even Number


False

↓

Odd Number
```

---

# 3. Else If Ladder

## Definition

Else If Ladder is used when multiple conditions need to be checked.

Java evaluates:

* First condition
* Second condition
* Third condition

until one condition becomes true.

---

## Example

```java
int marks = 75;

if(marks>=90){

System.out.println("Grade A");

}

else if(marks>=75){

System.out.println("Grade B");

}

else if(marks>=60){

System.out.println("Grade C");

}

else{

System.out.println("Fail");

}
```

---

## Output

```text
Grade B
```

---

# 4. Nested If Statement

## Definition

A Nested If means:

```text
if inside another if
```

The inner if executes only when the outer if condition is true.

---

## Example

```java
int age = 20;

int weight = 55;

if(age>=18){

if(weight>50){

System.out.println("You are eligible for the gym.");

}

}
```

---

## Output

```text
You are eligible for the gym.
```

---

# 5. Switch Statement

## Definition

The switch statement selects one block from multiple alternatives.

---

## Syntax

```java
switch(expression){

case value1:

// statements

break;


case value2:

// statements

break;


default:

// statements

}
```

---

## Example

```java
int day = 3;

switch(day){

case 1:

System.out.println("Monday");

break;


case 2:

System.out.println("Tuesday");

break;


case 3:

System.out.println("Wednesday");

break;


default:

System.out.println("Invalid Day");

}
```

---

## Output

```text
Wednesday
```

---

# Why is break used in switch?

Without:

```java
break;
```

Java executes all remaining cases.

This is called:

```text
Fall Through
```

Therefore:

```java
break;
```

stops execution.

---

# 6. For Loop

## Definition

The for loop executes a block of code a fixed number of times.

---

## Syntax

```java
for(initialization;

condition;

increment/decrement){

// statements

}
```

---

## Example

```java
for(int i=1;i<=5;i++){

System.out.println(i);

}
```

---

## Output

```text
1

2

3

4

5
```

---

## Execution Flow

```text
Initialization

↓

Condition

↓

Statements

↓

Increment

↓

Condition Again
```

---

# 7. While Loop

## Definition

The while loop executes repeatedly while the condition is true.

---

## Example

```java
int i=1;

while(i<=5){

System.out.println(i);

i++;

}
```

---

## Output

```text
1

2

3

4

5
```

---

## Execution Flow

```text
Condition

↓

True

↓

Statements

↓

Update

↓

Condition Again
```

---

# 8. Do While Loop

## Definition

The do-while loop executes the statements at least once.

Condition is checked after execution.

---

## Syntax

```java
do{

// statements

}

while(condition);
```

---

## Example

```java
int i=1;

do{

System.out.println(i);

i++;

}

while(i<=5);
```

---

## Output

```text
1

2

3

4

5
```

---

# Why Do While Executes at Least Once?

Because:

```text
Statements Execute First

↓

Condition Checks Later
```

Therefore:

Minimum execution:

```text
1 Time
```

---

# 9. Break Statement

## Definition

The break statement terminates:

* Loop
* switch statement

immediately.

---

## Example

```java
for(int i=1;i<=10;i++){

if(i==5){

break;

}

System.out.println(i);

}
```

---

## Output

```text
1

2

3

4
```

---

## Execution

When:

```text
i==5
```

Java executes:

```java
break;
```

and exits the loop.

---

# 10. Continue Statement

## Definition

The continue statement skips the current iteration and moves to the next iteration.

---

## Example

```java
for(int i=1;i<=5;i++){

if(i==3){

continue;

}

System.out.println(i);

}
```

---

## Output

```text
1

2

4

5
```

---

## Execution

When:

```text
i==3
```

Java:

* Skips printing 3
* Continues with next iteration.

---

# Difference Between break and continue

| break                    | continue                 |
| ------------------------ | ------------------------ |
| Terminates loop          | Skips current iteration  |
| Exits loop completely    | Continues next iteration |
| Used in loops and switch | Used only in loops       |

---

# Summary

Control Constructs are used to control the execution flow of Java programs.

This file covers:

* if Statement
* if-else Statement
* Else If Ladder
* Nested If
* Switch Statement
* For Loop
* While Loop
* Do While Loop
* Break Statement
* Continue Statement

These topics are among the most important Core Java concepts and are frequently asked in Java interviews.
