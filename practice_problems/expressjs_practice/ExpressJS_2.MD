<h1 align="center">Practical 13</h1>

- For this endeavor, continue with the codebase created in Practical 13 for QuickFresh project.
- Open VS Code inside the project directory.
- Inside the `index.js` file, perform the following:

1. Create a JSON array called `orderList` which has the following records:

    ```js
    [
        { id: 1, product: 'Apples', quantity: 2 },
        { id: 2, product: 'Bananas', quantity: 1 },
        { id: 3, product: 'Milk', quantity: 3 }
    ]
    ```

2. Now, for the route "/orders/:orderID", define a handler function such that for every GET request, extracts the `orderID` as a route parameter and:
    - Returns the order if there is a matching `orderID` in the `orderList` with a Status Code 200
    - Otherwise, returns `Order Not Found` with a Status Code 404

3. Create a JSON array called `productList` which has the following records:

    ```js
    [
        { id: 11, name: "Eggs", price: 30, availableQty: 50 },
        { id: 12, name: "Flour", price: 180, availableQty: 3 },
        { id: 14, name: "Butter", price: 70, availableQty: 100 },
        { id: 15, name: "Chocolate", price: 100, availableQty: 20 }
    ]
    ```

4. Now, for the route "/products", define a handler function such that for every GET request, it returns:
    - The original product list when the client does not provide any query parameter
    - A filtered product list when the client provides a query parameter called `name`. Example: `name=Duck Eggs`
    - A filtered product list when the client provides a query parameter called `maxPrice`. Example: `maxPrice=50`
    - A filtered product list when the client provides both the query parameters - `name` and `maxPrice`

5. Now create an empty JSON array called `shoppingCart`

6. Now, for the route "/cart", for every:
    - GET request, it returns the `shoppingCart` as JSON 
    - POST request, it processes the request body as JSON, looks up for the fields `id`, `name`, `price`, `qty`, and
        - If all the required fields are present, it adds the data to the shopping cart,
        - Otherwise, sends a message "Please provide all the required fields" with a status code 400

**Bonus**: For each of the routes - "/orders", "/products", "/cart", perform API testing using  the [Postman](https://www.postman.com/downloads/) OR [Thunderclient](https://www.thunderclient.com/) tool

```
Attach Screenshots for the same
```
