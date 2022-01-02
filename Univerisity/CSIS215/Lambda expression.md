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
Use a lamba expression in the [[ArrayList|ArrayList]]'s `forEach()` method to [[Java Syntax|print]] every item in the list:
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

Lambda expressions can be stored in [[Variables|variables]] if the [[Variable types|variable's type]] is an [[Interfaces|interface]] which has only one [[Methods|method]]. The lambda expression should have the same number of parameters and the same return type as that method. Java has many of these kinds of interfaces [[Java Packages|built in]], such as the `Consumer` interface (found in the `java.util` package) used by lists.

```ad-example
Use Java's `Consumer` interface to store a lambda expression in a variable:
```java
import java.util.ArrayList;
import java.util.function.Consumer;

public class Main {
  public static void main(String[] args) {
    ArrayList<Integer> numbers = new ArrayList<Integer>();
    numbers.add(5);
    numbers.add(9);
    numbers.add(8);
    numbers.add(1);
    Consumer<Integer> method = (n) -> { System.out.println(n); };
    numbers.forEach( method );
  }
}
```

To use a lambda expression in a method, the method should have a parameter with a single-method interface as its type. Calling the interface's method will run the lambda expression:

```ad-example
Create a method which takes a lambda expression as a parameter:
```java
interface StringFunction {
  String run(String str);
}

public class Main{
	public static void main(String[] args){
		StringFunction exclaim = (s) -> s + "!";
		String function ask = (s) -> s + "?";
		printFormatted("Hello", exclaim);
		printFormatted("Hello", ask);
	}
	public static void printFormatted(String str, StringFunction format) {
    	String result = format.run(str);
    	System.out.println(result);
	}
}
```

## Reference