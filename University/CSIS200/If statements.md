---
author: aboude
---
# If Statments
---

Created on: 2021-12-06-12:44
Last modified: 2021-12-06-12:44

---
### <span style="color: #ff5545;text-transform: capitalize;">What are if statements?</span>

if statements is used to specify a block of code to be executed, if a specified condition is met.
 
 There are 3 key statements you need to know when using an if statement :
 
 -   Use `if` to specify a block of code to be executed, if a specified condition is [[Booleans|true]].

-   Use `else` to specify a block of code to be executed, if the same condition is [[Booleans|false]].
-   Use `else if` to specify a new condition to test, if the first condition is [[Booleans|false]].

### <span style="color: #ff5545;text-transform: capitalize;">if statements</span>

Use the `if` statement to specify a block of Java code to be executed if a condition is [[Booleans|true]].

```ad-example
title: Syntax
```java
if (condition) {
  // block of code to be executed if the condition is true
}
```
___
```ad-example
```java
int x = 20;
int y = 18;
if (x > y) {
  System.out.println("x is greater than y");
}
```

In the example above we use two variables, **x** and **y**, to test whether x is greater than y (using the `>` [[Operators#span style color ff5545 Comparison Operators span|operator]]). As x is 20, and y is 18, and we know that 20 is greater than 18, we print to the screen that "x is greater than y".

### <span style="color: #ff5545;text-transform: capitalize;">else statement</span>

Use the `else` statement to specify a block of code to be executed if the condition is [[Booleans|false]].

```ad-example
title: Syntax
```java
if (condition) {
  // block of code to be executed if the condition is true
} else {
  // block of code to be executed if the condition is false
}
```
___
```ad-example
```java
int time = 20;
if (time < 18) {
  System.out.println("Good day.");
} else {
  System.out.println("Good evening.");
}
// Outputs "Good evening."
```

In the example above, time (20) is greater than 18, so the condition is [[Booleans|false]]. Because of this, we move on to the `else` condition and print to the screen "Good evening". If the time was less than 18, the program would print "Good day".

### <span style="color: #ff5545;text-transform: capitalize;">else if statments</span>
Use the `else if` statement to specify a new condition if the first condition is [[Booleans|false]].

```ad-example
title: Syntax
```java
if (condition1) {
  // block of code to be executed if condition1 is true
} else if (condition2) {
  // block of code to be executed if the condition1 is false and condition2 is true
} else {
  // block of code to be executed if the condition1 is false and condition2 is false
}
```
___
```ad-example
```java
int time = 22;
if (time < 10) {
  System.out.println("Good morning.");
} else if (time < 20) {
  System.out.println("Good day.");
} else {
  System.out.println("Good evening.");
}
// Outputs "Good evening."
```
In the example above, time (22) is greater than 10, so the **first condition** is `false`. The next condition, in the `else if` statement, is also `false`, so we move on to the `else` condition since **condition1** and **condition2** is both `false` - and print to the screen "Good evening".

However, if the time was 14, our program would print "Good day."

### <span style="color: #ff5545;text-transform: capitalize;">Ternary Operator</span>

There is also a short-hand if else, which is known as the **ternary operator** because it consists of three operands. It can be used to replace multiple lines of code with a single line. It is often used to replace simple if else statements.

```ad-example
title:Syntax
```java
variable = (condition) ? expressionTrue :  expressionFalse;
```

##### Example of turning an if statement to ternary:
```ad-Dont
title:Before
```java
int time = 20;
if (time < 18) {
  System.out.println("Good day.");
} else {
  System.out.println("Good evening.");
}
```
```ad-Do
title:After
```java
int time = 20;
String result = (time < 18) ? "Good day." : "Good evening.";
System.out.println(result);
```

## Relevant:
[[Operators#span style color ff5545 Comparison Operators span|Comparison operators]] | [[Booleans]] | [[Java Syntax]] 
