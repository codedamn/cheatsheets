# Variables

Variable is a a data item / placeholder for a certain data type that may take on more than one value during the runtime of a program.

There are three keywords for declaring variables in JS. 

1. `var` (Deprecated) : Declares the variable in global space
2. `let` : declare the variable. 

    If a variable is declared in a block that variable is not accessible in global space

    ```jsx
    let myvar = 34;
    ```

3. `const` : declare a variable but once declared can not be changed



## Variable Shadowing
blocking the access to the top level scope variable by defining a variable in the local scope

```jsx
const myAge = 17;
function (checkAge) {
	let checkAge = 25;
	return checkAge > 18 ? true : false; // this is always return true because the function already has a checkAge variable so this function can never access the varaible in the Top Level
```