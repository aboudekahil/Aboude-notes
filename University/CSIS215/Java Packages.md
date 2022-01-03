---
author: aboude
---
# Java Packages
___

Created on: 2022-01-03-18:00
Last modified: 2022-01-03-18:00

___
### <span style="color: #ff5545;text-transform: capitalize;">What’s a java package?</span>
A package in Java is used to group related classes. Think of it as **a folder in a file directory**. We use packages to avoid name conflicts, and to write a better maintainable code. Packages are divided into two categories:

-   Built-in Packages (packages from the Java API)
-   User-defined Packages (create your own packages)

### <span style="color: #ff5545;text-transform: capitalize;">Built in packages</span>
The Java API is a library of prewritten classes, that are free to use, included in the Java Development Environment.

The library contains components for managing input, database programming, and much much more. The complete list can be found at Oracles website: [https://docs.oracle.com/javase/8/docs/api/](https://docs.oracle.com/javase/8/docs/api/).

The library is divided into **packages** and **classes**. Meaning you can either import a single class (along with its methods and attributes), or a whole package that contain all the classes that belong to the specified package.

To use a class or a package from the library, you need to use the `import` keyword
```ad-example
title:Syntax
```java
import package.name.Class;   // Import a single class
import package.name.*;   // Import the whole package
```

### <span style="color: #ff5545;text-transform: capitalize;">Import a class</span>
If you find a class you want to use, for example, the `Scanner` class, **which is used to get user input**, write the following code
```ad-example
In the example, `java.util` is a package, while `Scanner` is a class of the `java.util` package.
```java
import java.util.Scanner;
```



## Reference