---
author: aboude
---
# Break/Continue
___

Created on: 2021-12-07-18:01
Last modified: 2021-12-07-18:01

___

### <span style="color: #ff5545;text-transform: capitalize;">Break keyword</span>
You have already seen the `break` statement used in an earlier chapter of this tutorial. It was used to "jump out" of a [[Switch statements|switch statement]].

The `break` statement can also be used to jump out of a **[[Loops|loop]]**.

```ad-example
```java
for (int i = 0; i < 10; i++) {
  if (i == 4) {
    break;
  }
  System.out.println(i);
}
```

This example stops the [[Loops|loop]] when i is [[Operators#span style color ff5545 Comparison Operators span|equal]] to 4.

### <span style="color: #ff5545;text-transform: capitalize;">Continue keyword</span>
The `continue` statement breaks one iteration (in the loop), if a specified [[Operators#span style color ff5545 Comparison Operators span|condition]] occurs, and continues with the next iteration in the [[Loops|loop]].

```ad-example
```java
for (int i = 0; i < 10; i++) {
  if (i == 4) {
    continue;
  }
  System.out.println(i);
}
```

This example skips the value of 4.

## Relevant 
[[Loops]] | [[While loops]] | [[Do-While loops]] | [[For loops]] | [[For-each loops]] | [[Operators]] | [[Switch statements]] | [[Java Syntax]]