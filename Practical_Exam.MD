## Problem 1

### Problem 1: File Reader
 
**Problem Statement:**
Create a function `readFileContent(filePath)` that takes the path to a file as input and reads its content asynchronously using the `fs` module. The function should print the content to the console.
 
**Function Signature:**
```javascript
function readFileContent(filePath) {
    // Implementation
}
```
 
**Expected Output:**
```
File Content:
This is the content of the file.
Hello, Node.js!
```
 
**Test Cases:**
```javascript
readFileContent('test-files/file1.txt');
// Expected Output: Content of file1.txt
 
readFileContent('test-files/empty-file.txt');
// Expected Output: (empty string)
 
readFileContent('test-files/nonexistent-file.txt');
// Expected Output: Error reading file: ENOENT: no such file or directory...
```

### Problem 2: File Writer
 
**Problem Statement:**
Create a function `writeToFile(filePath, content)` that takes the path to a file and user input content as input. The function should write the content to the specified file using the `fs` module.
 
**Function Signature:**
```javascript
function writeToFile(filePath, content) {
    // Implementation
}
```
 
**Expected Output:**
```
Data written to output.txt
```
 
**Test Cases:**
```javascript
writeToFile('test-files/output1.txt', 'Sample content.');
// Expected Output: Data written to output1.txt
 
writeToFile('test-files/nonexistent-folder/output.txt', 'Content in a non-existent folder.');
// Expected Output: Error writing to file: ENOENT: no such file or directory...
