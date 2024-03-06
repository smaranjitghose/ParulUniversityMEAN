<h1 align = "center">Practical 16</h1>

- Create a new project directory named `CineWow`
```

```

- Navigate inside the project directory
```

```

- Create an `index.js` file for server entrypoint

```

```

- Initialize npm inside the project directory

```

```

- Install the external modules `express`, `dotenv`, `mongoose`

```

```

- Create an environment file at the root of the project directory and store the environment variable `DATABASE_URL = "mongodb://localhost:27017/CineWow"`

```

```

- Now, create a `db.js` file at the root of the project directory. Import the environment variable and define a function `connectDB` that connects the ExpressJS application 
to MongoDB using mongoose ODM

```

```

- Import the `db.js` inside the `index.js` file and call the `connectDB` function to initialize a connection

```

```

Now, define the following routes with appropriate handler functions:

1. "/api/v1/getMovies" which recieves GET request and returns the list of all movies

```

```

2. "/api/v1/getMovie/:movieID" which recieves GET request and returns the movie matched with the particular movieID provided as router parameter

```

```

3. "/api/v1/addMovie", which recieves POST request with valid movie data in JSON format and inserts it into the database after validation

```

```

4. "/api/v1/updateMovie/:movieID", which recieves PATCH request with the fields to update JSON format, movieID as a route parameter and inserts it into the database after validation

```

```


5. "/api/v1/deleteMovie:movieID", which recieves DELETE request with the movieID as a route parameter and inserts it into the database after validation

```

```

6. Modify the "/api/v1/getMovies" defined in Q1, to enable filtering using query parameters such as rating, title, directors, etc

```

```
7. Modify the "/api/v1/getMovies" defined in Q6, to enable filtering using *only selective* query parameters : [director,rating,releaseYear,title]

```

```


8. Modify the "/api/v1/getMovies" defined in Q7, to allow advance filtering using the specified query paramaters: [director,rating,releaseYear,title] such that $gte, $gt, $lte, $lt operators can be invoked

```

```

9. Modify the "/api/v1/getMovies" defined in Q8, to allow sorting of the movie list by one or more fields specified by the `sort` query parameter

```

```

10. Modify the "/api/v1/getMovies" defined in Q9, to allow projection in the movie list by the `fields` query parameter. If the `fields` query parameter is not specified, exclude the "createdAt" field.

```

```

11. Modify the "/api/v1/getMovies" defined in Q10, to allow pagination specified by the `page` and `limit` query parameters.

```

```

12. Define a route "/api/v1/movieStats", where an aggregation pipeline is defined with a `$match` stage to display all movies where the rating is greater or equal to 7

```

```

13. Now, modify the "/api/v1/movieStats" in Q12, where an additional `$group` stage is used to compute and display the totalMovies`, `minYear`, `maxYear`, `averageRating`

```

```
14. Now, modify the "/api/v1/movieStats" in Q12, where an additional `$sort` stage is used to display the movies in descending order of `averageRating` field

```

```



**Bonus**: Test the functionalities of each of the routes using the [Postman](https://www.postman.com/downloads/)/[Thunderclient](https://www.thunderclient.com/) tool

```
Attach Screenshots for the same
```



