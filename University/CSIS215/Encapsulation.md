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

-   declare class variables/attributes as `private`
-   provide public **get** and **set** methods to access and update the value of a `private` variable

### <span style="color: #ff5545;text-transform: capitalize;">Get and Set</span>
`private` variables can only be accessed within the same class (an outside class has no access to it). However, it is possible to access them if we provide public **get** and **set** methods.

The `get` method returns the variable value, and the `set` method sets the value.


## Reference