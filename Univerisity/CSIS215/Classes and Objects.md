---
author: aboude
---
# Classes and Objects
___

Created on: 2022-01-02-12:57
Last modified: 2022-01-02-12:57

___

### <span style="color: #ff5545;text-transform: capitalize;">What are classes and objects</span>
Everything in Java is associated with classes and objects, along with its attributes and [[Methods|methods]]. For example: in real life, a car is an object. The car has attributes, such as weight and color, and [[Methods|methods]], such as drive and brake.

A Class is like an object constructor, or a "blueprint" for creating objects.

### <span style="color: #ff5545;text-transform: capitalize;">Creating a class</span>
To create a class in Java we use the `class` [[Keywords|keyword]]

```ad-example
```java
public class Main {
	int x = 5;
}
```
```ad-warning
a class should always start with an uppercase first letter, and that the name of the java file should match the class name.
```

### <span style="color: #ff5545;text-transform: capitalize;">Creating an object</span>
In Java, an object is created from a class. We have already created the class named `Main`, so now we can use this to create objects.

To create an object of `Main`, specify the class name, followed by the object name, and use the [[Keywords|keyword]] `new`:
```ad-example
Create an object called `myObj` and [[Java Syntax|print]] the value of x:
```java
public class Main {
  int x = 5;

  public static void main(String[] args) {
    Main myObj = new Main();
    System.out.println(myObj.x);
  }
}
```

### <span style="color: #ff5545;text-transform: capitalize;">Multiple objects</span>
You can create multiple objects of one class:

```ad-example
```java
public class Main {
  int x = 5;

  public static void main(String[] args) {
    Main myObj1 = new Main();  // Object 1
    Main myObj2 = new Main();  // Object 2
    System.out.println(myObj1.x);
    System.out.println(myObj2.x);
  }
}
```

## Reference
[[Methods]] | [[Keywords]] | [[Java Syntax]]