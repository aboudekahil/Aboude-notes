---
author: aboude
---
# Abstraction
___

Created on: 2022-01-03-15:06
Last modified: 2022-01-03-15:06

___
### <span style="color: #ff5545;text-transform: capitalize;">what is abstraction?</span>
Data **abstraction** is the process of hiding certain details and showing only essential information to the user.  

Abstraction can be achieved with either **abstract [[Classes and Objects|classes]]** or **[[interfaces]]**

The `abstract` [[Keywords|keyword]] is a non-access modifier, used for [[Classes and Objects|classes]] and [[methods]]:
-   **Abstract [[Classes and Objects|class]]:** is a restricted [[Classes and Objects|class]] that cannot be used to create [[Classes and Objects|objects]] (to access it, it must be inherited from another [[Classes and Objects|class]]).
  
-   **Abstract method:** can only be used in an abstract [[Classes and Objects|class]], and it does not have a body. The body is provided by the subclass (inherited from).

An abstract [[Classes and Objects|class]] can have both abstract and regular [[methods]]
```ad-example
```java
abstract class Animal {
  public abstract void animalSound();
  public void sleep() {
    System.out.println("Zzz");
  }
}
```
From the example above, it is not possible to create an [[Classes and Objects|object]] of the Animal [[Classes and Objects|class]]:
```ad-Dont
```java
Animal myObj = new Animal(); // will generate an error
```

To access the abstract [[Classes and Objects|class]], it must be inherited from another [[Classes and Objects|class]].

```ad-example
```java
// Abstract class
abstract class Animal {
  // Abstract method (does not have a body)
  public abstract void animalSound();
  // Regular method
  public void sleep() {
    System.out.println("Zzz");
  }
}

// Subclass (inherit from Animal)
class Pig extends Animal {
  public void animalSound() {
    // The body of animalSound() is provided here
    System.out.println("The pig says: wee wee");
  }
}

class Main {
  public static void main(String[] args) {
    Pig myPig = new Pig(); // Create a Pig object
    myPig.animalSound();
    myPig.sleep();
  }
}
```

### <span style="color: #ff5545;text-transform: capitalize;">Why use abstraction?</span>
To achieve security - hide certain details and only show the important details of an [[Classes and Objects|object]].


## Reference
[[Classes and Objects]] | [[Interfaces]] | [[Keywords]] | [[Methods]]