---
author: aboude
---
# Java Exceptions
___

Created on: 2022-01-03-18:36
Last modified: 2022-01-03-18:36

___

### <span style="color: #ff5545;text-transform: capitalize;">what are java exceptions?</span>
When executing Java code, different errors can occur: coding errors made by the programmer, errors due to wrong input, or other unforeseeable things.

When an error occurs, Java will normally stop and generate an error message. The technical term for this is: Java will throw an **exception** (throw an error).

### <span style="color: #ff5545;text-transform: capitalize;">try and catch</span>
The `try` statement allows you to define a block of code to be tested for errors while it is being executed.

The `catch` statement allows you to define a block of code to be executed, if an error occurs in the try block.

The `try` and `catch` keywords come in pairs:

```ad-example
title:Syntax
```java
try {
  //  Block of code to try
}
catch(Exception e) {
  //  Block of code to handle errors
}
```

```ad-error
This will generate an error, because **myNumbers[10]** does not exist.
```java
public class Main {
  public static void main(String[ ] args) {
    int[] myNumbers = {1, 2, 3};
    System.out.println(myNumbers[10]); // error!
  }
}
```
```ad-Do
title: Try and catch
```java
public class Main {
  public static void main(String[ ] args) {
    try {
      int[] myNumbers = {1, 2, 3};
      System.out.println(myNumbers[10]);
    } catch (Exception e) {
      System.out.println("Something went wrong.");
    }
  }
}
// this will output “Something went wrong”
```

### <span style="color: #ff5545;text-transform: capitalize;">Finally keyword</span> 
The `finally` statement lets you execute code, after `try...catch`, regardless of the result
```ad-example
```java
public class Main {
  public static void main(String[] args) {
    try {
      int[] myNumbers = {1, 2, 3};
      System.out.println(myNumbers[10]);
    } catch (Exception e) {
      System.out.println("Something went wrong.");
    } finally {
      System.out.println("The 'try catch' is finished.");
    }
  }
}
/* outputs 
Something went wrong
The 'try catch' is finished.
*/
```

### <span style="color: #ff5545;text-transform: capitalize;">Throw keyword</span>
The `throw` statement allows you to create a custom error.

The `throw` statement is used together with an **exception type**. There are many exception types available in Java: `ArithmeticException`, `FileNotFoundException`, `ArrayIndexOutOfBoundsException`, `SecurityException`.
```ad-example
```java
public class Main {
  static void checkAge(int age) {
    if (age < 18) {
      throw new ArithmeticException("Access denied - You must be at least 18 years old.");
    }
    else {
      System.out.println("Access granted - You are old enough!");
    }
  }

  public static void main(String[] args) {
    checkAge(15); // Set age to 15 (which is below 18...)
  }
}
```
The output will be
```cmd
Exception in thread "main" java.lang.ArithmeticException: Access denied - You must be at least 18 years old.  
	at Main.checkAge(Main.java:4)  
	at Main.main(Main.java:12)
```


## Reference