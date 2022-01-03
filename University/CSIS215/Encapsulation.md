---
author: aboude
---
# Encapsulation
___

Created on: 2022-01-03-13:52
Last modified: 2022-01-03-13:52

___

### <span style="color: #ff5545;text-transform: capitalize;">What is encapsulation?</span>
The meaning of **Encapsulation**, is to make sure that "sensitive" data is hidden from users. To achieve this, you must:

-   declare [[Classes and Objects|class]] [[variables]]/[[Class attributes|attributes]] as `private`
-   provide public **get** and **set** [[methods]] to access and update the value of a `private` variable

### <span style="color: #ff5545;text-transform: capitalize;">Get and Set</span>
`private` [[variables]] can only be accessed within the same [[Classes and Objects|class]] (an outside [[Classes and Objects|class]] has no access to it). However, it is possible to access them if we provide public **get** and **set** [[methods]].

The `get` method returns the variable value, and the `set` method sets the value.

Syntax for both is that they start with either `get` or `set`, followed by the name of the variable, with the first letter in upper case:

```ad-example
```java
public class Person {
  private String name; // private = restricted access

  // Getter
  public String getName() {
    return name;
  }

  // Setter
  public void setName(String newName) {
    this.name = newName;
  }
}
```
```ad-definition
title: Explanation
The `get` method returns the value of the variable `name`.

The `set` method takes a parameter (`newName`) and assigns it to the `name` variable. 

The `this` [[Keywords|keyword]] is used to refer to the current [[Classes and Objects|object]].

However, as the `name` variable is declared as `private`, we **cannot** access it from outside this [[Classes and Objects|class]]
```
## Reference