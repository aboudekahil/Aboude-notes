# this keyword
___

Created on: 2022-02-22-09:54
Last modified: 2022-02-22-09:54

___

### <span style="color: #ff5545;text-transform: capitalize;">What is the this keyword</span>

`this` is a self-referential keyword used inside a class to refer to either the class’ attributes or to call its constructor.

`this` is used when the argument of a method has the same name as a data attribute we want to use

```java
class Time{
	int hours;
	
	Time(int hours){
		this.hours = hours; //this.hours refers
	}
}
```

## Reference
[[Keywords]]