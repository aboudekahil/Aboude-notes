---
author: aboude
---
# Do-While loops
___

Created on: 2021-12-07-17:32
Last modified: 2021-12-07-17:32

___

### <span style="color: #ff5545;text-transform: capitalize;">what are do while loops?</span>
The `do-while` [[Loops|loop]] is a variant of the [[While loops|while loop]]. This loop will execute the [[Java Syntax|code block]] `once`, before checking if the condition is [[Booleans|true]], then it will repeat the loop as long as the [[Operators#span style color ff5545 Comparison Operators span|condition]] is [[Booleans|true]].

```ad-example
title:Syntax
```java
do {
  // code block to be executed
}
while (condition);
```

___
```ad-example
```java
int i = 0;
do {
  System.out.println(i);
  i++;
}
while (i < 5);
```

The example above uses a `do-while` [[Loops|loop]]. The [[Loops|loop]] will always be executed at least `once`, even if the condition is [[Booleans|false]], because the [[Java Syntax|code block]] is executed before the [[Operators#span style color ff5545 Comparison Operators span|condition]] is tested.

```ad-warning
Do not forget to increase the variable used in the condition, otherwise the loop will never end!
```

## Relevant 
[[Loops]] | [[Do-While loops]] | [[Booleans]] | [[Operators]] | [[Java Syntax]]