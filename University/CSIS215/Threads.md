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

head
## Reference