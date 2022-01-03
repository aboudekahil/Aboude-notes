---
author: aboude
---
# Class methods
___

Created on: 2022-01-03-12:43
Last modified: 2022-01-03-12:43

___
### <span style="color: #ff5545;text-transform: capitalize;">what are class methods</span>
You learned from the [[Methods]] note that methods are declared within a class, and that they are used to perform certain actions
```ad-example
`myMethod()` prints a text (the action), when it is **called**. To call a method, write the method's name followed by two parentheses **()** and a semicolon**;**
```java
public class Main {
  static void myMethod() {
    System.out.println("Hello World!");
  }
}
```

```ad-example
```java
public class Main {
  static void myMethod() {
    System.out.println("Hello World!");
  }

  public static void main(String[] args) {
    myMethod();
  }
}

// Outputs "Hello World!"
```
## Reference