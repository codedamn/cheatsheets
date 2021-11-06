# Error Handling

## try
```
try {
    // body of try
} 
catch(error) {
    // body of catch  
}
```
The main code is inside the `try` block. While executing the `try` block, if any error occurs, it goes to the `catch` block. </br>
If no error occurs, the code inside the `try` block is executed and the `catch` block is skipped.
## catch
```
try {
    // body of try
} 
catch(error) {
    // body of catch  
}
```
The `catch` block handles the errors as per the catch statements. There can be multiple `catch` followed by a `try` block. </br>
If error occurs, the code inside the `try` block is skipped and the `catch` block is executed.
## finally
```
try {
    // try_statements
} 
catch(error) {
    // catch_statements  
}
finally() {
    // codes that gets executed anyway
}
```
The `finally` block executes both when the code runs **successfully** or if an **error** occurs.
## throw
You can also use the `throw` statement with the `try...catch` statement to use **user-defined exceptions**.
