---
author: aboude
---
# Inheritance
___

Created on: 2022-01-03-14:36
Last modified: 2022-01-03-14:36

___
### <span style="color: #ff5545;text-transform: capitalize;">What is inheritance?</span>
In Java, it is possible to inherit [[Class attributes|attributes]] and [[methods]] from one [[Classes and Objects|class]] to another. We group the "inheritance concept" into two categories:

-   **subclass** (child) - the [[Classes and Objects|class]] that inherits from another [[Classes and Objects|class]]
-   **superclass** (parent) - the [[Classes and Objects|class]] being inherited from

To inherit from a [[Classes and Objects|class]], use the `extends` [[Keywords|keyword]].
```ad-example
In the example below, the `Car` [[Classes and Objects|class]] (subclass) inherits the [[Class attributes|attributes]] and [[methods]] from the `Vehicle` [[Classes and Objects|class]] (superclass)
```java
class Vehicle {
  protected String brand = "Ford";        // Vehicle attribute
  public void honk() {                    // Vehicle method
    System.out.println("Tuut, tuut!");
  }
}

class Car extends Vehicle {
  private String modelName = "Mustang";    // Car attribute
  public static void main(String[] args) {

    // Create a myCar object
    Car myCar = new Car();

    // Call the honk() method (from the Vehicle class) on the myCar object
    myCar.honk();

    // Display the value of the brand attribute (from the Vehicle class) and the value of the modelName from the Car class
    System.out.println(myCar.brand + " " + myCar.modelName);
  }
}
```
```ad-note
We set the **brand** [[Class attributes|attribute]] in **Vehicle** to a `protected` access [[Modifiers|modifier]]. If it was set to `private`, the Car [[Classes and Objects|class]] would not be able to access it.
```
### <span style="color: #ff5545;text-transform: capitalize;">Why use inheritance?</span>
It is useful for code reusability, reuse [[Class attributes|attributes]] and [[methods]] of an existing [[Classes and Objects|class]] when you create a new [[Classes and Objects|class]].
### <span style="color: #ff5545;text-transform: capitalize;">Final keyword</span>
If you don't want other [[Classes and Objects|classes]] to inherit from a [[Classes and Objects|class]], use the `final` [[Keywords|keyword]].
```ad-Dont
This will produce an error
```java
final class Vehicle {
  ...
}

class Car extends Vehicle {
  ...
}
```
## Reference
[[Classes and Objects]] | [[Methods]] | [[Classes and Objects]] | [[Keywords]]