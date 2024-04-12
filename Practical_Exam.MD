### Problem 1

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
function requestLoggerMiddleware(req, res, next) {
  // Your implementation here
}
```

**Expected Output:**
Log entries in the server console should be in the format: `{timestamp} - {HTTP method} request received`.

**Test Cases:**
1. Any incoming request should trigger the middleware and log the appropriate message.

## Problem 2

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
function positiveIntegerHandler(req, res) {
  // Your implementation here
}
```
 
**Expected Output:**
- If "number" is a positive integer: Return a success message.
- If "number" is not a positive integer: Trigger an error handled by the error handling middleware.
 
**Test Cases:**
1. Request to `/positive?number=5` should return a success message.
2. Request to `/positive?number=-2` should trigger the error handling middleware.
