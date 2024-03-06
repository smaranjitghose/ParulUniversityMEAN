<h1 align="center">Practical 15</h1>

- For this endeavor, continue with the codebase created in Practical 12 & 13 & 14 for QuickFresh project.
- Open VS Code inside the project directory.
- Create a sub-directory called `routes`
  ```
  
  ```
- Now, inside the `routes` sub-directory define create four router files `mainRouter.js`, `productRouter.js`, `cartRouter.js` and  `orderRouter.js`

- For each, router file
  - Initialize a `express.Router` object
  - Using this router object, create the appropriate route handling functions (keeping the response logic same for all the routes)
  - export this router object

      ```
      
      
      ```


- Now, inside the `index.js` file, perform the following:
  - Remove any route handling operations perfomed using `app.HTTPMETHOD` where HTTPMETHOD = GET, PATCH, PUT, POST, DELETE
  - Import the relevant router objects
  - Mount the router objects at the relevant paths using the router middleware

      ```
      
      
      ```

**Bonus**: Test the functionalities of each of the new refactored backend using the [Postman](https://www.postman.com/downloads/) OR [Thunderclient](https://www.thunderclient.com/) tool

```
Attach Screenshots for the same
```
