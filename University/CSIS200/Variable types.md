---
author: aboude
---
# Variable Types

---

Date created: 2021-12-04-19:47
Last Modified: 2021-12-05-13:58

---

### <span style="color: #ff5545;text-transform: capitalize;">How any variable types are there?</span>
There exist a plethora of [[Variables|variable]] types. The types themselves are divided into two categories, **[[Variable types#span style color ff5545 text-transform capitalize Primitive data types span|Primitive]]** and **[[Variable types#span style color ff5545 text-transform capitalize none-primitive types span|None-Primitive]]** 

`8` primitive data types exist.

None-primitive data types are `USUALLY` defined by the user which means there isn't set amount of them.

### <span style="color: #ff5545;text-transform: capitalize;">Primitive data types</span>
| Type    | Size    | Description                                                                       |
| ------- | ------- | --------------------------------------------------------------------------------- |
| byte    | 1 byte  | Stores whole [[numbers]] from -128 to 127                                             |
| short   | 2 bytes | Stores whole [[numbers]] from -32,768 to 32,767                                       |
| int     | 4 bytes | Stores whole [[numbers]] from -2,147,483,648 to 2,147,483,647                         |
| long    | 8 bytes | Stores whole [[numbers]] from -9,223,372,036,854,775,808 to 9,223,372,036,854,775,807 |
| float   | 4 bytes | Stores fractional [[numbers]]. Sufficient for storing 6 to 7 decimal digits           |
| double  | 8 bytes | Stores fractional [[numbers]]. Sufficient for storing 15 decimal digits               |
| boolean | 1 byte  | Stores true or false values                                                       |
| char    | 2 bytes | Stores a single character/letter or ASCII values                                  |

### <span style="color: #ff5545;text-transform: capitalize;"> none-primitive types</span>
An example of a None-Primitive Data type are [[Strings]], [[Strings]] aren't primitive because they refer to an object.

Non-primitive data types are called **reference types** because they refer to objects.

```ad-example
title:Examples of none-primitive types:
Examples of non-primitive types are [[Strings]], [[Arrays]], [[Interfaces]], etc.
```
### <span style="color: #ff5545;text-transform: capitalize;"> what's the difference between primitive and non-primitive variable types?
The main difference between **[[Variable types#span style color ff5545 text-transform capitalize Primitive data types span|primitive]]** and **[[Variable types#span style color ff5545 text-transform capitalize none-primitive types span|non-primitive]]** data types are:

-   Primitive types are predefined (already defined) in Java. Non-primitive types are created by the programmer and is not defined by Java (except for `String`).
-   Non-primitive types can be used to call [[methods]] to perform certain operations, while primitive types cannot.
-   A primitive type has always a value, while non-primitive types can be `null`.

-   A primitive type starts with a lowercase letter, while non-primitive types starts with an uppercase letter.

-   The size of a primitive type depends on the data type, while non-primitive types have all the same size.


## Relevant:
[[Strings]] | [[Classes and Objects]] | [[Arrays]] | [[Interfaces]]