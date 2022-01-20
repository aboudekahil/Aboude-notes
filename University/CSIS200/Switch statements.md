---
author: aboude
---
# Switch statements
___

Created on: 2021-12-0715:07
Last modified: 2022-01-20-10:31

___

### <span style="color: #ff5545;text-transform: capitalize;"> When do we use the switch statement?</span>

we use the `switch` statement to select one of many code blocks to be executed.

```ad-example
title:Syntax
```java
switch(expression) {
  case x:
    // code block
    break;
  case y:
    // code block
    break;
  default:
    // code block
}
```

##### How it works:

-   The `switch` expression is evaluated once.

-   The value of the expression is compared with the values of each `case`.
-   If there is a match, the associated block of code is executed.
-   The `break` and `default` [[keywords]] are optional, and will be described later in this chapter
___
The example below uses the weekday number to calculate the weekday name.
```ad-example
```java
int day = 4;
switch (day) {
  case 1:
    System.out.println("Monday");
    break;
  case 2:
    System.out.println("Tuesday");
    break;
  case 3:
    System.out.println("Wednesday");
    break;
  case 4:
    System.out.println("Thursday");
    break;
  case 5:
    System.out.println("Friday");
    break;
  case 6:
    System.out.println("Saturday");
    break;
  case 7:
    System.out.println("Sunday");
    break;
}
// Outputs "Thursday" (day 4)
```

```ad-note
You can use multiple cases in the same line

```java
switch(variable/expression){

	case value1: case value2: case value3:
		break;
	
	default:
		break;

}
```

### <span style="color: #ff5545;text-transform: capitalize;">break keyword</span>

When Java reaches a `break` keyword, it breaks out of the switch block.

This will stop the execution of more code and case testing inside the [[Java Syntax|block]].

When a match is found, and the job is done, it's time for a break. There is no need for more testing.

break keyword prevents `fall-through` errors (i.e java will execute everything under the case block you’re in ignoring the rest of the case checks)
	
```ad-info
A `break` can save a lot of execution time because it "ignores" the execution of all the rest of the code in the switch block.
```

### <span style="color: #ff5545;text-transform: capitalize;">default keyword</span>
The `default` keyword specifies some code to run if there is no case match:

```ad-example
```java
int day = 4;
switch (day) {
  case 6:
    System.out.println("Today is Saturday");
    break;
  case 7:
    System.out.println("Today is Sunday");
    break;
  default:
    System.out.println("Looking forward to the Weekend");
}
// Outputs "Looking forward to the Weekend"
```

```ad-note
Note that if the `default` statement is used as the last statement in a switch block, it does not need a break.
```

### <span style="color: #ff5545;text-transform: capitalize;">if statements → switch statements</span>

Switch statements can be used instead of [[If statements|if statements]] in certain situations, for example:

```ad-Dont
title: Before
```Java
int grade = 10;
char letter;
if(grade == 10){
	letter = 'A';
}else if (grade == 9){
	letter = 'B';
}else if (grade == 8){
	letter = 'C';
}else if (grade == 7){
	letter = 'D';
}else if (grade == 6){
	letter = 'E';
}else{
	letter = 'F';
} // letter will be 'A'
```
```ad-Do
```Java
int grade = 9;
char letter;
switch(grade){
	case 10:
		letter = 'A';
		break;
	case 9:
		letter = 'B';
		break;
	case 8:
		letter = 'C';
		break;
	case 7:
		letter = 'D';
		break;
	case 6:
		letter = 'E';
		break;
	default:
		letter = 'F';
		break;
}
```

## Relevant
[[If statements]] | [[Java Syntax]]