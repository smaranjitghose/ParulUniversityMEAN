## Problem 1



 
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

**Problem Statement:**

Create a logging middleware for an Express application. The middleware should log detailed information about each incoming request, including the timestamp, HTTP method, URL, request headers, and request body.

**Function Signature:**

```javascript
/** 
* Logging middleware for Express 
* @param {Object} req - Express request object 
* @param {Object} res - Express response object
* @param {Function} next - Express next function */

const loggingMiddleware = (req, res, next) => { 
    // Your implementation here 
}
```
**Expected Output:**

- Each incoming request should be logged with detailed information.

**Test Cases:**

- Make multiple requests and check the server logs for detailed information.


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


## Problem 8

 
**Problem Statement:**

1) Create an Express application with MongoDB integration using Mongoose. Implement a function to establish a connection to a MongoDB database. Ensure that the connection is successful and log a success message.
 
**Function Signature:**
```javascript
/**
* Establishes a connection to MongoDB using Mongoose
*/
const connectToMongoDB = () => {
  // Your implementation here
}
```
 
**Expected Output:**
- If the connection is successful, log a success message.
 
**Test Cases:**
- Call `connectToMongoDB()` and check the server logs for a successful connection message.

2) Define a Mongoose schema for a "User" with properties: "username" (string) and "email" (string). 

3) Create a Mongoose model for the User schema. 

4) Create an Express route to add a new user to the MongoDB database 

 
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
- Call `addUserToDatabase({ username: 'smaranjit_ghose', email: 'hello@smaranjitghose.com' })` and check the server logs for a success message.

5) Create an Express route that retrieves all users from the MongoDB database and returns them as a JSON response.
 
**Function Signature:**
```javascript
/**
* Express route to get all users from MongoDB
* @param {Object} req - Express request object
* @param {Object} res - Express response object
*/
const getAllUsers = (req, res) => {
  // Your implementation here
}
```
 
**Expected Output:**
- Return a JSON response with an array of user objects.
 
**Test Cases:**
- Access the route `/users` and check if the response contains the expected user data.
 

Remember to connect Mongoose to your MongoDB database using mongoose.connect.

## Problem 9

**Problem Statement:**


1) Create an Express application with MongoDB integration using Mongoose. Implement a function to establish a connection to a MongoDB database. Ensure that the connection is successful and log a success message.
 
**Function Signature:**
```javascript
/**
* Establishes a connection to MongoDB using Mongoose
*/
const connectToMongoDB = () => {
  // Your implementation here
}
```
2)  Define a Mongoose schema for the product with properties like "name," "price," and "quantity."

3) Create a Mongoose Model for the Product Schema

4) Implement a set of CRUD (Create, Read, Update, Delete) operations for a "Product" entity using MongoDB and Mongoose Implement functions to create, read, update, and delete products.
 
**Function Signature:**
```javascript
/**
* Creates a new product in MongoDB
* @param {Object} product - Product object with properties name, price, and quantity
*/
const createProduct = (product) => {
  // Your implementation here
}
 
/**
* Retrieves all products from MongoDB
* @returns {Array} - Array of product objects
*/
const getAllProducts = () => {
  // Your implementation here
}
 
/**
* Updates a product in MongoDB
* @param {string} productId - ID of the product to update
* @param {Object} updatedProduct - Updated product object
*/
const updateProduct = (productId, updatedProduct) => {
  // Your implementation here
}
 
/**
* Deletes a product from MongoDB
* @param {string} productId - ID of the product to delete
*/
const deleteProduct = (productId) => {
  // Your implementation here
}
```
 
**Expected Output:**
- The functions should perform the respective CRUD operations on the "Product" collection in MongoDB.
 
**Test Cases:**
1. Create a product, retrieve all products, update a product, and then delete the product.
 

## Problem 10

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

## Problem 11

**Problem Statement:**

You are developing a complex web application with multiple routes and middleware in Node.js and Express. You want to implement a centralized error handling mechanism to catch and handle errors gracefully without crashing the server. Design a middleware function that intercepts errors thrown by route handlers or other middleware and sends an appropriate error response to the client.
 
**Function Signature:**
```javascript
const errorHandler = (err, req, res, next) => {
    // Your implementation here
}
```



## Problem 12

 
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

## Problem 13

- Fork the https://github.com/smaranjitghose/ParulUniversityMEAN Repo
- Create a clone of the forked repo
- Make a new branch mswd_exam
- Add a new file "DIVISION_ENROLLMENT_NO_Exam.MD"
- The file should contain a breif definition of What is Git? Features of Git
- Stage and Commit the Changes
- Push to Forked Repo on GitHub
- Make a Pull Request






