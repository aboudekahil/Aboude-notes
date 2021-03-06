---
author: aboude
---

# Modifiers
___

Created on: 2022-01-02-21:55
Last modified: 2022-01-02-21:55

___

### <span style="color: #ff5545;text-transform: capitalize;">what are modifiers?</span>
Modifiers are [[keywords|Keywords]] you add to [[Classes and Objects|Classes]], [[Methods|methods]], [[Variables|variables]] and other java members to change their meaning.

Modifiers are split into two groups:
* **Access Modifiers** - controls the access level

* **Non-Access Modifiers** - do not control access level, but provides other functionality

### <span style="color: #ff5545;text-transform: capitalize;">Access modifiers</span>
For [[Classes and Objects|classes]] you can use

| Modifier  |                                                            Description                                                            |
|:---------:|:---------------------------------------------------------------------------------------------------------------------------------:|
| `public`  |                                            The class is accessible by any other class                                             |
| *default* | The class is only accessible by classes in the same [[Java Packages\|package]]. `This is used when you don't specify a modifier.` |

For  **[[Classes and Objects|attributes]], [[Methods|methods]] and [[Constructors|constructors]]**, you can use the one of the following:

|  Modifier   |                                            Description                                             |
|:-----------:|:--------------------------------------------------------------------------------------------------:|
|  `public`   |                               The code is accessible for all classes                               |
|  `private`  |                       The code is only accessible within the declared class                        |
| `protected` |   The code is accessible in the same [[Java Packages\|package]] and [[Inheritance\|subclasses]].   |
|  *default*  | The code is only accessible in the same package. `This is used when you don't specify a modifier.` | 

### <span style="color: #ff5545;text-transform: capitalize;">Non-Access Modifiers</span>
For [[Classes and Objects|classes]] you can use

|  Modifier  |                                                                 Description                                                                 |
|:----------:|:-------------------------------------------------------------------------------------------------------------------------------------------:|
|  `final`   |                                       The class cannot be [[Inheritance\|inherited]] by other classes                                       |
| `abstract` | The class cannot be used to create [[Classes and Objects\|objects]] (To access an abstract class, it must be inherited from another class.) | 

For attributes and [[Methods|methods]]:

| Modifier       | Description                                                                                                                                                                                           |
| -------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `final`        | Attributes and [[methods]] cannot be overridden/modified                                                                                                                                                  |
| `static`       | Attributes and [[methods]] belongs to the class, rather than an object                                                                                                                                    |
| `abstract`     | Can only be used in an abstract class, and can only be used on [[methods]]. The method does not have a body, for example **abstract void run();**. The body is provided by the subclass (inherited from). |
| `transient`    | Attributes and [[methods]] are skipped when serializing the object containing them                                                                                                                        |
| `synchronized` | [[Methods]] can only be accessed by one thread at a time                                                                                                                                                  |
| `volatile`     | The value of an attribute is not cached thread-locally, and is always read from the "main memory"                                                                                                     | 

### <span style="color: #ff5545;text-transform: capitalize;">Final</span>
If you don't want the ability to override existing attribute values, declare attributes as `final`:
```ad-example
```java
public class Main {
  final int x = 10;
  final double PI = 3.14;

  public static void main(String[] args) {
    Main myObj = new Main();
    myObj.x = 50; // will generate an error: cannot assign a value to a final variable
    myObj.PI = 25; // will generate an error: cannot assign a value to a final variable
    System.out.println(myObj.x);
  }
}
```

### <span style="color: #ff5545;text-transform: capitalize;">Static</span>
A `static` method means that it can be accessed without creating an object of the class, unlike `public`:
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
  public static void main(String[ ] args) {
    myStaticMethod(); // Call the static method
    // myPublicMethod(); This would output an error

    Main myObj = new Main(); // Create an object of Main
    myObj.myPublicMethod(); // Call the public method
  }
}
```

### <span style="color: #ff5545;text-transform: capitalize;">Abstract</span>
An `abstract` method belongs to an `abstract` class, and it does not have a body. The body is provided by the subclass:

```ad-example
```java
// Code from filename: Main.java
// abstract classabstract class Main {
  public String fname = "John";
  public int age = 24;
  public abstract void study(); // abstract method
}

// Subclass (inherit from Main)
class Student extends Main {
  public int graduationYear = 2018;
  public void study() { // the body of the abstract method is provided here
    System.out.println("Studying all day long");
  }
}
// End code from filename: Main.java

// Code from filename: Second.java
class Second {
  public static void main(String[] args) {
    // create an object of the Student class (which inherits attributes and methods from Main)
    Student myObj = new Student();

    System.out.println("Name: " + myObj.fname);
    System.out.println("Age: " + myObj.age);
    System.out.println("Graduation Year: " + myObj.graduationYear);
    myObj.study(); // call abstract method  }
}
```

## Reference
[[Keywords]] | [[Classes and Objects]] | [[Methods]] | [[Variables]] | [[Java Packages]] | [[Constructors]] | [[Inheritance]]