# Arrays


## Array Methods 

### `.push()`

```jsx
let fruits = ['Apple','Banana'];
let newLength = fruits.push('Orange');
console.log(fruits) // ['Apple','Banana']
console.log(newLength) // ['Apple','Banana','Orange']

```

### `.shift()`
### `.unshift()`
### `.pop()`
### `.findLast()`
### `.findLastIndex()`
### `.splice()`

splice has 2 mandatory arguments [index, no of elements to be removed]

splice also returns the list of the removed elements

splice can have n number of arguments after the first two mandatory arguments. all the n number of arguments are added to the array from the index as mentioned in the first argument

### `.slice()`

takes two arguments [start index, stop index]

slice leaves the passed array untouched and returns the elements as mentioned in the argument

### `.map()`

map calls a provided callbackFn function once for each element in an array, in order, and constructs a new array from the results. callbackFn is invoked only for indexes of the array which have assigned values (including undefined).

```jsx
let numbers = [1, 4, 9]
let roots = numbers.map(function(num) {
    return Math.sqrt(num)
})
// roots is now     [1, 2, 3]
// numbers is still [1, 4, 9]
```

### `.filter()`

.filter() method creates a new element in the new array if the return statement of the element in the callback function is true 

```jsx
const words = ['spray', 'limit', 'elite', 'exuberant', 'destruction', 'present'];

const result = words.filter(word => word.length > 6);

console.log(result);
// expected output: Array ["exuberant", "destruction", "present"]
```

### `.reduce()`

[Learn JavaScript Array Reduce In 10 Minutes](https://www.youtube.com/watch?v=s1XVfm5mIuU)

### `.forEach()`

takes a callback and traverses to the entire array. 

```jsx
const array1 = ['a', 'b', 'c'];

array1.forEach(element => console.log(element));

// expected output: "a"
// expected output: "b"
// expected output: "c"
```

### `.indexOf()`

argument : value 

if the argument exists in the given list the `index` of the element which matches with the argument is returned else `-1` is returned

### `.includes()`   `**ES 6**`

.includes simply returns boolean. Returns true if the argument passed exists in the array or return false if not found in the array

### `.find()`

takes a callback function and