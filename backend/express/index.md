# Express JS 


Express is a Node.Js library that helps us in writing back-end support for your application


## Setting up a basic server with Express
With the three lines of code you can setup a functional server in Node.js. Now you can open your browser and visit `localhost:3000`, then you'll get a text saying that `Cannot GET /`. If you get this message that means you have successfully setup the server.
```JavaScript
const express = require('express');
const app = express();

app.listen(3000);
```

The reason why we get the message  `Cannot GET /` is because we are not returning a file or status at the `/` route, which is the starting route for any server. 

## Setting up a basic Route - GET request
```JSX
const express = require('express');
const app = express();

app.get('/', (req, res, next) => {
    res.send('Hello Client!');
} )
app.listen(3000);
```

`req` and `res` are standard naming conventions for the callback function as they stand for request and response respectively. 

The third parameter `next` is pretty optional and is not used for 99% of the time. 

