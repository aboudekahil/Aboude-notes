---
author: aboude
---
# Constructors
___

Created on: 2022-01-03-13:10
Last modified: 2022-01-03-13:10

___
 ### <span style="color: #ff5545;text-transform: capitalize;">What are constructors?</span>
 A constructor in Java is a **special method** that is used to initialize objects. The constructor is called when an object of a class is created. It can be used to set initial values for object attributes.
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
the constructor name must **match the class name**, and it cannot have a **return type** (like `void`).

the constructor is called when the object is created.

All classes have constructors by default: if you do not create a class constructor yourself, Java creates one for you. However, then you are not able to set initial values for object attributes.
```
### <span style="color: #ff5545;text-transform: capitalize;"></span>
## Reference