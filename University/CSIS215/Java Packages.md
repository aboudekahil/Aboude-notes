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

To use the `Scanner` class, create an object of the class and use any of the available methods found in the `Scanner` class documentation. We will use the `nextLine()` method, which is used to read a complete line

```ad-example
```java
import java.util.Scanner;

class MyClass {
  public static void main(String[] args) {
    Scanner myObj = new Scanner(System.in);
    System.out.println("Enter username");

    String userName = myObj.nextLine();
    System.out.println("Username is: " + userName);
  }
}
```

### <span style="color: #ff5545;text-transform: capitalize;">import a package</span>
There are many packages to choose from. In the previous example, we used the `Scanner` class from the `java.util` package. This package also contains date and time facilities, random-number generator and other utility classes.

To import a whole package, end the sentence with an asterisk sign (`*`). The following example will import ALL the classes in the `java.util` package
```ad-example
```java
import java.util.*;
```

### <span style="color: #ff5545;text-transform: capitalize;">User defined classes</span>

To create your own package, you need to understand that Java uses a file system directory to store them. Just like folders on your computer
```ad-example
└── root
$\quad$└── mypack
$\qquad$└── MyPackageClass.java
```
To create a package, use the `package` keyword
```ad-example
```java
package mypack;
class MyPackageClass {
  public static void main(String[] args) {
    System.out.println("This is my package!");
  }
}
```
Save the file as **MyPackageClass.java**, and compile it
```cmd
C:\Users\_Your Name_>javac MyPackageClass.java
```
## Reference