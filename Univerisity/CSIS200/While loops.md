---
author: aboude
---
# While loops
___

Created on: 2021-12-07-16:57
Last modified: 2021-12-07-16:57

___

### <span style="color: #ff5545;text-transform: capitalize;">what are while loops</span>
The `while` loop loops through a block of code as long as a specified condition is [[Booleans|true]].

```ad-example
title:Syntax
```java
while (condition) {
  // code block to be executed
}
```

___

```ad-example
```java
int i = 0;
while (i < 5) {
  System.out.println(i);
  i++;
}
```

In the example above, the code in the [[Loops|loop]] will run, over and over again, as long as a [[Variables|variable]] `i` is [[Operators#span style color ff5545 Comparison Operators span|less than]] 5.

```ad-warning
 Do not forget to increase the variable used in the condition, otherwise the loop will never end!
 ```
 
 ## Relevant
 [[Loops]] | [[Operators]] | [[Java Syntax]] | [[Variables]] | [[Booleans]]