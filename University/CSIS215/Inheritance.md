---
author: aboude
---
# Inheritance
___

Created on: 2022-01-03-14:36
Last modified: 2022-01-03-14:36

___
### <span style="color: #ff5545;text-transform: capitalize;">What is inheritance?</span>
In Java, it is possible to inherit attributes and methods from one class to another. We group the "inheritance concept" into two categories:

-   **subclass** (child) - the class that inherits from another class
-   **superclass** (parent) - the class being inherited from

To inherit from a class, use the `extends` keyword.
```ad-example
In the example below, the `Car` class (subclass) inherits the attributes and methods from the `Vehicle` class (superclass)
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

```
## Reference