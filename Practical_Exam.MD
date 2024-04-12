## Problem 1

## Problem 2

<!-- Problem 5: File Extension Checker -->

**Problem Statement:**
Create a function `checkFileExtension(filePath, expectedExtension)` that takes a file path and an expected file extension as input. The function should check if the file has the expected extension using the `path` module and print the result to the console.

**Function Signature:**
```javascript
const checkFileExtension = (filePath, expectedExtension)  => {
    // Implementation
}
```

**Expected Output:**
```
File has the expected extension: .txt
```

**Test Cases:**
```javascript
checkFileExtension('test-files/report.pdf', '.pdf');
// Expected Output: File has the expected extension: .txt

checkFileExtension('test-files/profile_pic.png', '.jpg');
// Expected Output: File does not have the expected extension. Expected: .jpg, Actual: .png
```


## Problem 3

<!-- Problem 6: Express Route Handling -->
 
**Problem Statement:**
You are building a web application using Express in Node.js. Create an Express route to handle GET requests to the endpoint "/greet" that takes a query parameter "name" and returns a personalized greeting. If the name parameter is not provided, the default greeting should be "Namaskar, Guest!".
 
**Function Signature:**
```javascript
/**
* Handles GET requests to "/greet" endpoint
* @param {Object} req - Express request object
* @param {Object} res - Express response object
*/
const greetHandler = (req, res) => {
  // Your implementation here
}
```
 
**Expected Output:**
- If the "name" parameter is provided: "Namaskar, {name}!"
- If the "name" parameter is not provided: "Namaskar, Guest!"
 
**Test Cases:**
1. Request to `/greet?name=Girish` should return "Namaskar, Girish!"
2. Request to `/greet` should return "Namaskar, Guest!"


## Problem 4

<!-- Problem 7: Express Middleware -->

**Problem Statement:**
Implement an Express middleware function that logs the timestamp and the HTTP method of every incoming request to the server.

**Function Signature:**
```javascript
/**
 * Express middleware to log incoming requests
 * @param {Object} req - Express request object
 * @param {Object} res - Express response object
 * @param {Function} next - Express next function
 */
const requestLoggerMiddleware = (req, res, next) => {
  // Your implementation here
}
```

**Expected Output:**
Log entries in the server console should be in the format: `{timestamp} - {HTTP method} request received`.

**Test Cases:**
1. Any incoming request should trigger the middleware and log the appropriate message.

## Problem 5

<!-- Problem 8: Express Error Handling -->

**Problem Statement:**
Create an Express route that throws an error if the request parameter "number" is not a positive integer. Implement an error handling middleware to catch and handle this specific error, returning a custom error message and a 400 Bad Request status.
 
**Function Signature:**
```javascript
/**
* Express route to handle requests with a positive integer parameter
* @param {Object} req - Express request object
* @param {Object} res - Express response object
*/
const positiveIntegerHandler = (req, res) => {
  // Your implementation here
}
```
 
**Expected Output:**
- If "number" is a positive integer: Return a success message.
- If "number" is not a positive integer: Trigger an error handled by the error handling middleware.
 
**Test Cases:**
1. Request to `/positive?number=5` should return a success message.
2. Request to `/positive?number=-2` should trigger the error handling middleware.
