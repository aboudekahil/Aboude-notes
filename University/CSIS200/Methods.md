---
author: aboude
---
# Methods
___

Created on: 2021-12-09-14:17
Last modified: 2021-12-11-15:08

___

### <span style="color: #ff5545;text-transform: capitalize;">what are methods?</span>
A **method** is a block of code which only runs when it is called.

You can pass data, known as parameters, into a method.

Methods are used to perform certain actions, and they are also known as **functions**.

Why use methods? To reuse code: define the code once, and use it many times.

A method must be declared within a [[Classes and Objects|class]]. It is defined with the name of the method, followed by parentheses **`()`**. Java provides some pre-defined methods, such as [[Java Syntax#span style color ff5545 text-transform capitalize println span|System.out.println()]], but you can also create your own methods to perform certain actions.

```ad-example
title:Syntax
```java
public class Main {
  header returnType Name(type parameter1) {
    // code to be executed
  }
}
```
> -   `header` is like a definition of how we want to use the method.
>
> -  `returnType` defines what we want to get from the method.
> -  `Name` is an [[Identifiers|identifier]] that is used to reference the method and use it.
> - `parameter1` is an optional kind of “input” that is used to enter outside values so they can be used inside the method.
### <span style="color: #ff5545;text-transform: capitalize;">Calling a method</span>
To call a method in Java, write the method's name followed by two parentheses **`()`** and a semicolon **`;`**

```ad-example
Inside `main`, call the `myMethod()` method:
```java
public class Main {
  static void myMethod() {
    System.out.println("I just got executed!");
  }

  public static void main(String[] args) {
    myMethod();
  }
}

// Outputs "I just got executed!"
```
___
```ad-example
A method can also be called multiple times:
```java
public class Main {
  static void myMethod() {
    System.out.println("I just got executed!");
  }

  public static void main(String[] args) {
    myMethod();
    myMethod();
    myMethod();
  }
}

// I just got executed!
// I just got executed!
// I just got executed!
```

### <span style="color: #ff5545;text-transform: capitalize;">method parameters</span>
Information can be passed to methods as parameter. Parameters act as [[Variables|variables]] inside the method.

Parameters are specified after the method name, inside the parentheses. You can add as many parameters as you want, just separate them with a comma.

```ad-example
title:Syntax
```java
public static int doSomething(type name, type another name){

}
```
___
```ad-example
```java
public class Main {
  static void myMethod(String fname) {
    System.out.println(fname + " Refsnes");
  }

  public static void main(String[] args) {
    myMethod("Liam");
    myMethod("Jenny");
    myMethod("Anja");
  }
}
// Liam Refsnes
// Jenny Refsnes
// Anja Refsnes
```

The example has a method that takes a [[Strings|String]] called **fname** as parameter. When the method is called, we pass along a first name, which is used inside the method to print the full name

```ad-note
You can have as many parameters as you like
```ad-example
```java
public class Main {
  static void myMethod(String fname, int age) {
    System.out.println(fname + " is " + age);
  }

  public static void main(String[] args) {
    myMethod("Liam", 5);
    myMethod("Jenny", 8);
    myMethod("Anja", 31);
  }
}

// Liam is 5
// Jenny is 8
// Anja is 31
```

```ad-warning
When you are working with multiple parameters, the method call must have the same number of arguments as there are parameters, and the arguments must be passed in the same order.
```

### <span style="color: #ff5545;text-transform: capitalize;">Return values</span>
The `void` keyword, used in the examples above, indicates that the method should not return a value. If you want the method to return a value, you can use a [[Variable types#span style color ff5545 text-transform capitalize Primitive data types span|primitive data type]] (such as `int`, `char`, etc.) instead of `void`, and use the `return` [[Keywords|keyword]] inside the method.

```ad-example
title: Example 1
```java
public class Main {
  static int myMethod(int x) {
    return 5 + x;
  }

  public static void main(String[] args) {
    System.out.println(myMethod(3));
  }
}
// Outputs 8 (5 + 3)
```

```ad-example
title: Example 2
```java
public class Main {
  static int myMethod(int x, int y) {
    return x + y;
  }

  public static void main(String[] args) {
    int z = myMethod(5, 3);
    System.out.println(z);
  }
}
// Outputs 8 (5 + 3)
```

### <span style="color: #ff5545;text-transform: capitalize;">Method overloading</span>
With **method overloading**, multiple methods can have the same name with different parameters.
```ad-example
title:Example 1
```java
int myMethod(int x)
float myMethod(float x)
double myMethod(double x, double y)
```

```ad-example
title:Example 2
Consider the following example, which has two methods that add [[numbers]] of different type:
```java
static int plusMethodInt(int x, int y) {
  return x + y;
}

static double plusMethodDouble(double x, double y) {
  return x + y;
}

public static void main(String[] args) {
  int myNum1 = plusMethodInt(8, 5);
  double myNum2 = plusMethodDouble(4.3, 6.26);
  System.out.println("int: " + myNum1);
  System.out.println("double: " + myNum2);
}
```

```ad-note
 Multiple methods can have the same name as long as the number and/or type of parameters are different.
```

### <span style="color: #ff5545;text-transform: capitalize;">Scope of variables</span>
In Java, [[variables]] are only accessible inside the region they are created. This is called **scope**.

##### Method scope
[[Variables]] declared directly inside a method are available anywhere in the method following the line of code in which they were declared:
```ad-example
```java
public class Main {
  public static void main(String[] args) {

    // Code here CANNOT use x

    int x = 100;

    // Code here can use x
    System.out.println(x);
```

##### Block scopes
A block of code refers to all of the code between curly braces `{}`. [[Variables|Variables]] declared inside blocks of code are only accessible by the code between the curly braces, which follows the line in which the [[Variables|variable]] was declared.
```ad-example
```java
public class Main {
  public static void main(String[] args) {

    // Code here CANNOT use x

    { // This is a block

      // Code here CANNOT use x

      int x = 100;

      // Code here CAN use x
      System.out.println(x);

   } // The block ends here

  // Code here CANNOT use x

  }
}
```

```ad-note
A block of code may exist on its own or it can belong to an `if`, `while` or `for` statement. In the case of `for` statements, [[variables]] declared in the statement itself are also available inside the block's scope.
```

### <span style="color: #ff5545;text-transform: capitalize;">Recursion</span>
Recursion is the technique of making a function call itself. This technique provides a way to break complicated problems down into simple problems which are easier to solve.

```ad-example
Using recursion to add all [[numbers]] from 1 to 10:
```java
public class Main {
  public static void main(String[] args) {
    int result = sum(10);
    System.out.println(result);
  }
}
```
```ad-note
title:Example Explained
When the `sum()` function is called, it adds parameter `k` to the sum of all [[numbers]] smaller than `k` and returns the result. When k becomes 0, the function just returns 0. When running, the program follows these steps:

10 + sum(9)  
10 + ( 9 + sum(8) )  
10 + ( 9 + ( 8 + sum(7) ) )  
...  
10 + 9 + 8 + 7 + 6 + 5 + 4 + 3 + 2 + 1 + sum(0)  
10 + 9 + 8 + 7 + 6 + 5 + 4 + 3 + 2 + 1 + 0

Since the function does not call itself when `k` is 0, the program stops there and returns the result.
```

##### Halting Condition
Just as [[Loops|loops]] can run into the problem of infinite looping, recursive functions can run into the problem of infinite recursion. Infinite recursion is when the function never stops calling itself. Every recursive function should have a halting condition, which is the condition where the function stops calling itself. In the previous example, the halting condition is when the parameter `k` becomes 0.

## Relevant 
[[Classes and Objects]] | [[Java Syntax]] | [[Identifiers]] | [[Variables]] | [[Strings]] | [[Variable types]] | [[Keywords]] | [[Loops]]