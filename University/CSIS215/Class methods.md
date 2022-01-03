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
calling `MyMethod` in the `main` method
```java
public class Main {
  static void myMethod() {
    System.out.println("Hello World!");
  }

  public static void main(String[] args) {
    myMethod();
  }
}

// Outputs "Hello World"
```

### <span style="color: #ff5545;text-transform: capitalize;">Static vs Non-Static methods</span>
You will often see Java programs that have either `static` or `public` attributes and methods.

In the example above, we created a `static` method, which means that it can be accessed without creating an object of the class, unlike `public`, which can only be accessed by objects
```ad-example
```java
public class Main {
  // Static method
  static void myStaticMethod() {
    System.out.println("Static methods can be called without creating objects");
  }

  // Public method
  public void myPublicMethod() {
    System.out.println("Public methods must be called by creating objects");
  }

  // Main method
  public static void main(String[] args) {
    myStaticMethod(); // Call the static method
    // myPublicMethod(); This would compile an error

    Main myObj = new Main(); // Create an object of Main
    myObj.myPublicMethod(); // Call the public method on the object
  }
}
```



## Reference