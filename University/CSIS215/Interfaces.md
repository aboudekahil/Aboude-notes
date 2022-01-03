---
author: aboude
---
# Interfaces
___

Created on: 2022-01-03-15:13
Last modified: 2022-01-03-15:13

___
Another way to achieve [[abstraction]] in Java, is with interfaces.

### <span style="color: #ff5545;text-transform: capitalize;">What are interfaces?</span>
An `interface` is a completely "**abstract [[Classes and Objects|class]]**" that is used to group related [[methods]] with empty bodies

```ad-example
```java
// interface
interface Animal {
  public void animalSound(); // interface method (does not have a body)
  public void run(); // interface method (does not have a body)
}
```

To access the interface [[methods]], the interface must be "implemented" (kinda like inherited) by another [[Classes and Objects|class]] with the `implements` [[Keywords|keyword]] (instead of `extends`). The body of the interface method is provided by the "implement" [[Classes and Objects|class]]

```ad-example
```java
// Interface
interface Animal {
  public void animalSound(); // interface method (does not have a body)
  public void sleep(); // interface method (does not have a body)
}

// Pig "implements" the Animal interface
class Pig implements Animal {
  public void animalSound() {
    // The body of animalSound() is provided here
    System.out.println("The pig says: wee wee");
  }
  public void sleep() {
    // The body of sleep() is provided here
    System.out.println("Zzz");
  }
}

class Main {
  public static void main(String[] args) {
    Pig myPig = new Pig();  // Create a Pig object
    myPig.animalSound();
    myPig.sleep();
  }
}
```

```ad-note
-   Like **abstract [[Classes and Objects|classes]]**, interfaces **cannot** be used to create [[Classes and Objects|objects]] (in the example above, it is not possible to create an "Animal" [[Classes and Objects|object]] in the MyMainClass)

-   Interface [[methods]] do not have a body - the body is provided by the "implement" [[Classes and Objects|class]]
-   On implementation of an interface, you must override all of its [[methods]]
-   Interface [[methods]] are by default `abstract` and `public`
-   Interface [[Class attributes|attributes]] are by default `public`, `static` and `final`
-   An interface cannot contain a constructor (as it cannot be used to create [[Classes and Objects|objects]])
```

### <span style="color: #ff5545;text-transform: capitalize;">Why use interfaces?</span>
1) To achieve security - hide certain details and only show the important details of an [[Classes and Objects|object]] (interface).

2) Java does not support "multiple [[inheritance]]" (a [[Classes and Objects|class]] can only inherit from one superclass). However, it can be achieved with interfaces, because the [[Classes and Objects|class]] can **implement** multiple interfaces. 

### <span style="color: #ff5545;text-transform: capitalize;">Multiple Interfaces</span>
To implement multiple interfaces, separate them with a comma:
```ad-example
```java
interface FirstInterface {
  public void myMethod(); // interface method
}

interface SecondInterface {
  public void myOtherMethod(); // interface method
}

class DemoClass implements FirstInterface, SecondInterface {
  public void myMethod() {
    System.out.println("Some text..");
  }
  public void myOtherMethod() {
    System.out.println("Some other text...");
  }
}

class Main {
  public static void main(String[] args) {
    DemoClass myObj = new DemoClass();
    myObj.myMethod();
    myObj.myOtherMethod();
  }
}
```

## Reference
[[Abstraction]] | [[Classes and Objects]] | [[Methods]] | [[Keywords]] | [[Inheritance]]