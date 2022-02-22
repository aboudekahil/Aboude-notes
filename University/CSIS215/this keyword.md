# this keyword
___

Created on: 2022-02-22-09:54
Last modified: 2022-02-22-09:54

___

### <span style="color: #ff5545;text-transform: capitalize;">What is the this keyword</span>

`this` is a self-referential keyword used inside a class to refer to either the class’ attributes or to call its constructor.

`this` is used when the argument of a method has the same name as a data attribute we want to use

```ad-example
```java
class Time{
	int hours;
	
	Time(int hours){
		this.hours = hours; // this.hours refers to the data attribute
							// while hours refers to the constructors
							// argument
	}
}
```

`this` can also be used to call a constructor by using `(arg-list)` operator on `this`

```ad-example
Here, we use `this` to call the three argument constructor in all the other constructos because it will be easier to maintain if we need to change the code AND it'll be easier to read.
```java
class Time {
	private int hours;
 	private int minutes;
 	private int seconds;

 	Time() {
 		this(0, 0, 0);
	}

 	Time(int hours) {
		this(hours, 0, 0);
	}

 	Time(int hours, int minutes) {
 		this(hours, minutes, 0);
	}

 	Time(int hours, int minutes, int seconds) {

 		if (0 <= hours && hours <= 23) {
 			this.hours = hours;
		}

 		if (0 <= minutes && minutes <= 59) {
 			this.minutes = minutes;
 		}
		
 		if (0 <= seconds && seconds <= 59) {
 			this.seconds = seconds;
 		}
 	}

 	Time(Time t) {
 		this(t.hours, t.minutes, t.seconds);
 	}
}
```

## Reference
[[Keywords]]