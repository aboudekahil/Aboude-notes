---
author: aboude
---

# Lambda expression
___

Created on: 2022-01-02-13:48
Last modified: 2022-01-02-13:48

___

### <span style="color: #ff5545;text-transform: capitalize;">what are lambda expressions?</span>
A lambda expression is a short block of code which takes in parameters and returns a value. Lambda expressions are similar to [[Methods|methods]], but they do not need a name and they can be implemented right in the body of a method.

### <span style="color: #ff5545;text-transform: capitalize;">Syntax</span>
The simplest lambda expression contains a single parameter and an expression:
```ad-example
title:Syntax
```java
parameter -> expression
```
To use more than one parameter, wrap them in parentheses:
```ad-example
title:Syntax
```java
(parameter1, parameter2) -> expression
```

Expressions are limited. They have to immediately return a value, and they cannot contain [[Variables|variables]], assignments or statements such as [[If statements|if]] or [[For loops|for]]. In order to do more complex operations, a code block can be used with curly braces. If the lambda expression needs to return a value, then the code block should have a `return` statement.
```ad-example
```java
(parameter1, parameter2) -> {code block}
```

### <span style="color: #ff5545;text-transform: capitalize;">Using lambda expressions</span>
Lambda expressions are usually passed as parameters to a [[Methods|function]]:
```ad-example
Use a lamba expression in the `ArrayList`'s `forEach()` method to print every item in the list:
```java
import java.util.ArrayList;

public class Main {
  public static void main(String[] args) {
    ArrayList<Integer> numbers = new ArrayList<Integer>();
    numbers.add(5);
    numbers.add(9);
    numbers.add(8);
    numbers.add(1);
    numbers.forEach( (n) -> { System.out.println(n); } );
  }
}
```

## Reference