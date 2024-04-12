## Problem 1

<!-- Problem 2: File Writer -->

 
**Problem Statement:**
Create a function `writeToFile(filePath, content)` that takes the path to a file and user input content as input. The function should write the content to the specified file using the `fs` module.
 
**Function Signature:**
```javascript
const writeToFile = (filePath, content) => {
    // Implementation
}
```
 
**Expected Output:**
```
Data written to output.txt
```
 
**Test Cases:**
```javascript
writeToFile('test-files/log.txt', 'Today is MSWD Exam');
// Expected Output: Data written to log.txt
 
writeToFile('test-files/nonexistent-folder/output.txt', 'Content in a non-existent folder.');
// Expected Output: Error writing to file: ENOENT: no such file or directory...
```

## Problem 2

<!-- Problem 3: Execute Command -->
 
**Problem Statement:**
Create a function `executeCommand(command)` that takes a shell command as input and executes it using the `child_process` module. The function should print the output of the command to the console.
 
**Function Signature:**
```javascript
const executeCommand = (command) => {
    // Implementation
}
```
 
**Expected Output:**
```
Command Output:
File1.txt
File2.txt
```
 
**Test Cases:**
```javascript
executeCommand('ls -la');
// Expected Output: (output of ls -la)
 
executeCommand('echo "Hello, Node.js!"');
// Expected Output: Hello, Node.js!
```

## Problem 3

<!-- Problem 4: Resolve Path -->
 
**Problem Statement:**
Create a function `resolvePath(relativePath)` that takes a relative path as input and resolves it to an absolute path using the `path` module. The function should print the resolved path to the console.
 
**Function Signature:**
```javascript
const resolvePath = (relativePath) => {
    // Implementation
}
```
 
**Expected Output:**
```
Resolved Path: /Users/username/project/folder/file.txt
```
 
**Test Cases:**
```javascript
resolvePath('../project/folder/file.txt');
// Expected Output: Resolved Path: /Users/username/project/folder/file.txt
 
resolvePath('nonexistent-folder/file.txt');
// Expected Output: Resolved Path: /Users/username/nonexistent-folder/file.txt
```

## Problem 4

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


## Problem 5

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


## Problem 6

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

## Problem 7

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


## Problem 13

<!-- Problem 17: Mongoose Schema and Model -->

 
**Problem Statement:**
Define a Mongoose schema for a "User" with properties: "username" (string) and "email" (string). Create a Mongoose model for the User schema. Implement a function to add a new user to the MongoDB database.
 
**Function Signature:**
```javascript
/**
* Adds a new user to the MongoDB database
* @param {Object} user - User object with properties username and email
*/
const addUserToDatabase = (user) => {
  // Your implementation here
}
```
 
**Expected Output:**
- If the user is successfully added, log a success message.
 
**Test Cases:**
1. Call `addUserToDatabase({ username: 'smaranjit_ghose', email: 'hello@smaranjitghose.com' })` and check the server logs for a success message.
 

Remember to connect Mongoose to your MongoDB database using mongoose.connect.


## Problem 14

<!-- Problem 12: Express Rate Limiting -->

**Problem Statement:**
Implement a rate-limiting middleware for an Express application. The middleware should limit the number of requests from a single IP address to a specified rate, and return a 429 Too Many Requests status if the limit is exceeded.

**Function Signature:**
```javascript
/**
 * Rate-limiting middleware for Express
 * @param {Object} req - Express request object
 * @param {Object} res - Express response object
 * @param {Function} next - Express next function
 */
const rateLimitMiddleware = (req, res, next) => {
  // Your implementation here
}
```

**Expected Output:**
- If the number of requests from a single IP is below the limit, allow the request to proceed.
- If the limit is exceeded, return a 429 Too Many Requests status.

**Test Cases:**
1. Send requests within the limit; all should proceed.
2. Send requests exceeding the limit; some should return a 429 status.


## Problem 15

<!-- Problem 11: Express Authentication Middleware -->
 
**Problem Statement:**
Implement an authentication middleware for an Express application. The middleware should check for the presence of a valid JWT (JSON Web Token) in the request headers. If a valid token is present, allow the request to proceed; otherwise, return a 401 Unauthorized status.
 
**Function Signature:**
```javascript
/**
* Authentication middleware for Express
* @param {Object} req - Express request object
* @param {Object} res - Express response object
* @param {Function} next - Express next function
*/
const authenticationMiddleware = (req, res, next) => {
  // Your implementation here
}
```
 
**Expected Output:**
- If a valid JWT is present, allow the request to proceed.
- If no JWT is present or it's invalid, return a 401 Unauthorized status.
 
**Test Cases:**
1. Request with a valid JWT should proceed.
2. Request without a JWT or with an invalid JWT should return a 401 Unauthorized status.


