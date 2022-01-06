---
author: aboude
---
# Constructors
___

Created on: 2022-01-03-13:10
Last modified: 2022-01-03-13:10

___
 ### <span style="color: #ff5545;text-transform: capitalize;">What are constructors?</span>
 A constructor in Java is a **special [[Methods|method]]** that is used to initialize [[Classes and Objects|objects]]. The constructor is called when an [[Classes and Objects|object]] of a [[Classes and Objects|class]] is created. It can be used to set initial values for [[Classes and Objects|object]] [[Class attributes|attributes]].
 ```ad-example
 ```java
// Create a Main class
public class Main {
  int x;  // Create a class attribute

  // Create a class constructor for the Main class
  public Main() {
    x = 5;  // Set the initial value for the class attribute x
  }

  public static void main(String[] args) {
    Main myObj = new Main(); // Create an object of class Main (This will call the constructor)
    System.out.println(myObj.x); // Print the value of x
  }
}

// Outputs 5
```
```ad-note
the constructor name must **match the [[Classes and Objects|class]] name**, and it cannot have a **return type** (like `void`).

the constructor is called when the [[Classes and Objects|object]] is created.

All [[Classes and Objects|classes]] have constructors by default: if you do not create a class constructor yourself, Java creates one for you. However, then you are not able to set initial values for [[Classes and Objects|object]] [[Class attributes|attributes]].
```
### <span style="color: #ff5545;text-transform: capitalize;">Constructor Parameters</span>
Constructors can also take parameters, which is used to initialize [[Class attributes|attributes]].

```ad-example
The following example adds an `int y` parameter to the constructor. Inside the constructor we set x to y (x=y). When we call the constructor, we pass a parameter to the constructor (5), which will set the value of x to 5
```java
public class Main {
  int x;

  public Main(int y) {
    x = y;
  }

  public static void main(String[] args) {
    Main myObj = new Main(5);
    System.out.println(myObj.x);
  }
}

// Outputs 5
```
## Reference
[[Methods]] | [[Classes and Objects]] | [[Class attributes]]