# ES6+ Features
ES6 stands for ECMA Script Standards 6 / ES6 / ES 2015. The following features were approved by the ECMA International / ECMA technical committee in the year 2015 and is called ES6 because it is the sixth release of features / rules.

## Arrow Functions `ES6`
### Single Line Functions


## Destructuring 
#### Destructuring Object - 1

```jsx
let myObj = {
    name : "John Doe",
    dob : " 13012004",
    height: 176,
    weight : 79,
    eyes : "brown"}

// Destructuring the object 
let {name, dob, height, weight, eyes} = myObj;
console.log(name) // John Doe
console.log(eyes) // brown
```

#### Destructuring Object - 2 `Spread syntax (...)`

```jsx
let myObj = {
    name : "John Doe",
    dob : " 13012004",
    height: 176,
    weight : 79,
    eyes **: "brown"}
let {name, dob, ...rest} = myObj;
console.log(name) //John Doe
console.log(rest) /*{height: 176,
                     weight : 79,
                     eyes: "brown"} */
```
### Array Destructuring
### Object Destructuring
### What happens to Overlapping keys ?

## Exporting 
There are basically two export statements

#### `export`

```jsx
// filename : heading.js
export const heading = "This is my heading";
```

If we export just using the `export` statement then at the time of import the variable name should match and we must keep the variable in `{}` to import it as an object.

```jsx
// filename : index.js
import {heading} from './heading';
```

#### `export default`

```jsx
// filename : heading.js
const heading = "This is my heading";
export default heading;
```

If we use the `default export` statement then at the time of import we can have our own variable i.e. the export variable need not be the same as import variable

```jsx
// filename : index.js
import newHeading from './heading';
```

## Short Circuit Evaluation
### `||`

```jsx
const firstValue = '' || 'myName'; // myName
```
If the first value is `falsy` then the second value is returned. If the first value is `truthy` then the first value is returned
### `&&`

```jsx
const firstName = 'myName' && 'myNickName'; // myNickName
```
If the any of the value is `falsy` then nothing will be returned. if both the values are `truthy` then the second value is returned.