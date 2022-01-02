---
author: aboude
---
# For loops
___

Created on: 2021-12-07-17:12
Last modified: 2021-12-07-17:12

___

### <span style="color: #ff5545;text-transform: capitalize;">What are for loops?</span>

When you know exactly how many times you want to loop through a block of code, use the `for` loop instead of a [[While loops|while loop]].

```ad-example
title:Syntax
```java
for (statement 1; statement 2; statement 3) {
  // code block to be executed
}
```

>**<span style="color:#ffcd43">Statement 1</span>** is executed `one time` before the execution of the code block.
>___
> **<span style="color:#18a05e">Statement 2</span>** defines the condition for executing the code block.
> ___
> **<span style="color:#dd5044">Statement 3</span>** is executed `every time` after the code block has been executed.

___

```ad-example
```java
for (int i = 0; i < 5; i++) {
  System.out.println(i);
}
```

##### Example explained:

> **<span style="color:#ffcd43">Statement 1</span>**: sets a [[Variables|variable]] before the loop starts `int i = 0`.
>___
> **<span style="color:#18a05e">Statement 2</span>**: defines the [[Operators#span style color ff5545 Comparison Operators span|condition]] for the [[Loops|loop]] to run `i must be less than 5`. If the condition is [[Booleans|true]], the [[Loops|loop]] will start over again, if it is [[Booleans|false]], the [[Loops|loop]] will end.
>___
> **<span style="color:#dd5044">Statement 3</span>**: [[Operators#span style color ff5545 Arithmetic operators span|increases]] a value `i++` each time the [[Java Syntax|code block]] in the [[Loops|loop]] has been executed.

## Relevant 
[[Loops]] | [[While loops]] | [[Variables]] | [[Booleans]] | [[Operators]] | [[Java Syntax]]