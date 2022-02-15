# Grabage collector
___

Created on: 2022-02-15-09:50
Last modified: 2022-02-15-09:50

___
### <span style="color: #ff5545;text-transform: capitalize;">What is a reference type</span>
Before defining what is a garbage collector we need to define what’s a refence type first, any non-primitve type (i.e anything that isn’t a number, a boolean or a character) is a reference type. 

Being a reference type variable means that instead of the variabe holding the value of the type (for exemple an `int` variable can hold the value of `5` ), it holds a reference or address to where the value is being stored in the memory.

Reference type are more difficult to handle for many reasons, one of them is when passing a reference type as a parameter to a method, instead of passing a copy of the value, you pass a copy of the address/reference, which means you can edit the value of the variable directly within the method.

```ad-note
`ANY` reference type can be assigned the value of `null`.

The value `null` means the variable points to nowhere.
```

### <span style="color: #ff5545;text-transform: capitalize;">The garbage collector</span>
The garbage collector is an automated operation that happens when executing a file to help free up memory when a value is no longer needed.

The garbage collector keeps up with all the reference variables in the program, and when a value is no longer referenced to, i.e the variable is now of the value `null`, the garbage collector tells your pc that the address of the previous value in the memory is now free for any other program to use.

## Reference
[[Variable types]]