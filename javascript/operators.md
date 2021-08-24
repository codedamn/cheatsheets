# Operators 

## **Bitwise Operators**
    ### `&` ### AND
    ### `|` ### OR
    ### `~` ### NOT
    ### `^` ### XOR

### `,`(Comma) operator 
to evaluate multiple expressions in one line

```jsx
for (var i = 0,j = 10; i <= 3; i++ , j++ ) {
    console.log('Floor no : ' + i + 'Flat no : ' + j
}
```

### `new` operator 
create an instance of a user-defined object type or of one of the build-in object types that has a constructor function

```jsx
let currentDate = new Date();
```

### `delete` operator
removes a property from an object. If no more reference to the same property are held, it is eventually released automatically

```jsx
var admin = {
    isCoding : true,
    isLearning : false }
console.log(admin.isCoding) // true
delete admin.isCoding 
console.log(admin.isCoding) // undefined
```

### `in` operator 
returns true if hte specified property is in the specified object or its prototype chain

```jsx
const user = {
    name : 'John Doe',
    profession : 'web dev',
    age : 40,
    nationality : 'Indian'
}
console.log("name" in user) // true
console.log("salary" in user) // false
```

### `instanceof` operator 
to check the type of an object at run time. It returns a boolean value that indicates if an object is an instance of a particular class

```jsx
var newString = newString('This is a new string') // string object
console.log(newString instanceof String) // true
```

### `this` 
used to refer the current object. In general refers to the calling object in a method

```jsx
var person = {
    firstName : 'John',
    lastName : 'Doe',
    fullName : () => this.firstName + ' ' + this.lastName;
};
```

### `typeof` 
returns the data type of the operand

```jsx
let name = 'John Doe'
let myObj = {
    desktop : false,
    laptop : true}

console.log(typeof name) // string
console.log(typeof myObj) // object
```

### `?` Ternary Operator

### `??` Nullish coalescing operator 
returns its right-hand side operand when its left-hand side operand is `null` or `undefined`, and otherwise returns its left-hand side operand.

```jsx
undefined ?? 'something' // something
0 ?? 'something' //0
```

`??` is almost similar to `||` but `||` returns other value when `false` but `??` returns other value when the first value is `null` or `undefined`