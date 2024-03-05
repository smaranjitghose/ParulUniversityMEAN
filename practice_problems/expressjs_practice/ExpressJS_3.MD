<h1 align="center">Practical 14</h1>

- For this endeavor, continue with the codebase created in Practical 12 & 13 for QuickFresh project.
- Open VS Code inside the project directory.
- Inside the `index.js` file, perform the following:

1. Create a global middleware that logs all incoming HTTP requests to all the routes and prints it on the terminal in the format `DATETIME | HTTP METHOD | PATH`

    ```

    ```

2. Create a middleware that handles HTTP requests to all undefined routes and returns a message `We don't have this page yet!` with a status code 404

    ```

    ```

3. Create a middleware that handles all server errors, prints the error to the terminal and returns a mesage `Sorry! Something went wrong` with a Status Code 500

    ```

    ```

4. a) Create a sub-directory called `public` at the root level of the project directory

   b) Download the referenced [image](https://github.com/smaranjitghose/ParulUniversityMEAN/blob/main/practice_problems/datasets/static_file_demo.png)

   c) Place the downloaded image inside the `public` sub-directory'

   d) Now, creae a middleware that serves the image from the sub-directory `public` while being accessed from a virtual path `assets`

    ```


    ```


**Bonus**: Test the functionalities of each of the middleware using the POSTMAN tool

    ```

    Attach Screenshots for the same

    ```
