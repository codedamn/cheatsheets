# Document Object Model

## Browser Object
## Document Object
## .getElementById()
## .getElementsByClassName()
## .getElementsByTagName()
## document.head
## document.body
## parentNode, childNode
## document.getElementById 

### document.getElementById() v/s document.querySelector()
document.getElementById() is faster compared to querySelector when compared in performance because getElementById  uses hashmaps & indexes

But querySelector can traverse on any other NodeLinks because they are also part of the DOM Tree. 

```jsx
const ul = document.querySelector('ul');
const li = ul.querySelector('li');

const li = ul.getElementById('#list-item') // this won't work because getElementById can't traverse the NodeList
```

### ElementNode.innerHTML v/s ElementNode.appendChild
innerHTML resets some properties and can refresh the DOM while appendChild does not disturb other parts of the DOM
## document.createElement('li')
## document.appendChild()
## document.removeChild()
## setAttribute()
## removeAttribute()