---
author: aboude
---
# Java Packages
___

Created on: 2022-01-03-18:00
Last modified: 2022-01-03-18:00

___
### <span style="color: #ff5545;text-transform: capitalize;">What’s a java package?</span>
A package in Java is used to group related [[Classes and Objects|classes]]. Think of it as **a folder in a file directory**. We use packages to avoid name conflicts, and to write a better maintainable code. Packages are divided into two categories:

-   Built-in Packages (packages from the Java API)
-   User-defined Packages (create your own packages)

### <span style="color: #ff5545;text-transform: capitalize;">Built in packages</span>
The Java API is a library of prewritten [[Classes and Objects|classes]], that are free to use, included in the Java Development Environment.

The library contains components for managing input, database programming, and much much more. The complete list can be found at Oracles website: [https://docs.oracle.com/javase/8/docs/api/](https://docs.oracle.com/javase/8/docs/api/).

The library is divided into **packages** and **[[Classes and Objects|classes]]**. Meaning you can either import a single [[Classes and Objects|class]] (along with its [[methods]] and [[Class attributes|attributes]]), or a whole package that contain all the [[Classes and Objects|classes]] that belong to the specified package.

To use a [[Classes and Objects|class]] or a package from the library, you need to use the `import` [[Keywords|keyword]]
```ad-example
title:Syntax
```java
import package.name.Class;   // Import a single class
import package.name.*;   // Import the whole package
```

### <span style="color: #ff5545;text-transform: capitalize;">Import a class</span>
If you find a [[Classes and Objects|class]] you want to use, for example, the `Scanner` [[Classes and Objects|class]], **which is used to get user input**, write the following code
```ad-example
In the example, `java.util` is a package, while `Scanner` is a class of the `java.util` package.
```java
import java.util.Scanner;
```

To use the `Scanner` [[Classes and Objects|class]], create an [[Classes and Objects|object]] of the [[Classes and Objects|class]] and use any of the available [[methods]] found in the `Scanner` [[Classes and Objects|class]] documentation. We will use the `nextLine()` method, which is used to read a complete line

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
There are many packages to choose from. In the previous example, we used the `Scanner` [[Classes and Objects|class]] from the `java.util` package. This package also contains date and time facilities, random-number generator and other utility [[Classes and Objects|classes]].

To import a whole package, end the sentence with an asterisk sign (`*`). The following example will import ALL the [[Classes and Objects|classes]] in the `java.util` package
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
To create a package, use the `package` [[Keywords|keyword]]
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
C:\Users\Your Name>javac MyPackageClass.java
```
Then compile the package
```cmd
C:\Users\Your Name>javac -d . MyPackageClass.java
```
This forces the compiler to create the "mypack" package.

The `-d` keyword specifies the destination for where to save the class file. You can use any directory name, like c:/user (windows), or, if you want to keep the package within the same directory, you can use the dot sign "`.`", like in the example above.

```ad-note
The package name should be written in lower case to avoid conflict with class names.
```

When we compiled the package in the example above, a new folder was created, called "mypack".

To run the **MyPackageClass.java** file, write the following:

```cmd
C:\Users\_Your Name_>java mypack.MyPackageClass
```
The output will be:
```cmd
This is my package!
```

## Reference
[[Classes and Objects]] | [[Methods]] | [[Class attributes]] | [[Keywords]]
