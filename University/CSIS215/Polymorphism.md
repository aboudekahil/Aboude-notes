---
author: aboude
---
# Polymorphism
___

Created on: 2022-01-03-14:54
Last modified: 2022-01-03-14:54

___
### <span style="color: #ff5545;text-transform: capitalize;">what is polymorphism?</span>
Polymorphism means "many forms", and it occurs when we have many [[Classes and Objects|classes]] that are related to each other by [[inheritance]].

**[[Inheritance]]** lets us inherit [[Class attributes|attributes]] and [[methods]] from another [[Classes and Objects|class]]. **Polymorphism** uses those [[methods]] to perform different tasks. This allows us to perform a single action in different ways.

For example, think of a superclass called `Animal` that has a method called `animalSound()`. Subclasses of Animals could be Pigs, Cats, Dogs, Birds - And they also have their own implementation of an animal sound (the pig oinks, and the cat meows, etc.)

```ad-example
```java
class Animal {
  public void animalSound() {
    System.out.println("The animal makes a sound");
  }
}

class Pig extends Animal {
  public void animalSound() {
    System.out.println("The pig says: wee wee");
  }
}

class Dog extends Animal {
  public void animalSound() {
    System.out.println("The dog says: bow wow");
  }
}

class Main {
  public static void main(String[] args) {
    Animal myAnimal = new Animal();  // Create a Animal object
    Animal myPig = new Pig();  // Create a Pig object
    Animal myDog = new Dog();  // Create a Dog object
    myAnimal.animalSound(); // prints “The animal makes a sound”
    myPig.animalSound(); // prints “The pig says: wee wee”
    myDog.animalSound(); // prints “The dog says: bow wow”
  }
}
```

### <span style="color: #ff5545;text-transform: capitalize;">Why use polymorphism</span>
It is useful for code reusability, reuse [[Class attributes|attributes]] and [[methods]] of an existing [[Classes and Objects|class]] when you create a new [[Classes and Objects|class]].

## Reference
[[Classes and Objects]] | [[Inheritance]] | [[Class attributes]] | [[Methods]]