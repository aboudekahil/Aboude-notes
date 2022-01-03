---
author: aboude
---
# Threads
___

Created on: 2022-01-03-19:03
Last modified: 2022-01-03-19:03

___

### <span style="color: #ff5545;text-transform: capitalize;">What are threads?</span>
Threads allows a program to operate more efficiently by doing multiple things at the same time.

Threads can be used to perform complicated tasks in the background without interrupting the main program.

### <span style="color: #ff5545;text-transform: capitalize;">Creating a thread</span>
There are two ways to create a thread.

It can be created by extending the `Thread` class and overriding its `run()` method
```ad-example
```java
public class Main extends Thread {
  public void run() {
    System.out.println("This code is running in a thread");
  
```

Another way to create a thread is to implement the `Runnable` interface:
```ad-example
```java
public class Main implements Runnable {
  public void run() {
    System.out.println("This code is running in a thread");
  }
}
```

### <span style="color: #ff5545;text-transform: capitalize;">Running threads</span>
If the class extends the `Thread` class, the thread can be run by creating an instance of the class and call its `start()` method
```ad-example
```java
public class Main extends Thread {
  public static void main(String[] args) {
    Main thread = new Main();
    thread.start();
    System.out.println("This code is outside of the thread");
  }
  public void run() {
    System.out.println("This code is running in a thread");
  }
}
```
If the class implements the `Runnable` interface, the thread can be run by passing an instance of the class to a `Thread` object's constructor and then calling the thread's `start()` method
```ad-example
```java
public class Main implements Runnable {
  public static void main(String[] args) {
    Main obj = new Main();
    Thread thread = new Thread(obj);
    thread.start();
    System.out.println("This code is outside of the thread");
  }
  public void run() {
    System.out.println("This code is running in a thread");
  }
}
```

### <span style="color: #ff5545;text-transform: capitalize;">Concurrency problems</span>
Because threads run at the same time as other parts of the program, there is no way to know in which order the code will run. When the threads and main program are reading and writing the same variables, the values are unpredictable. The problems that result from this are called concurrency problems.
```ad-example
A code example where the value of the variable **amount** is unpredictable
```java
public class Main extends Thread {
  public static int amount = 0;

  public static void main(String[] args) {
    Main thread = new Main();
    thread.start();
    System.out.println(amount);
    amount++;
    System.out.println(amount);
  }
}
```

## Reference