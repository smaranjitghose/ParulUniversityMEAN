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

- Now, define a route "/api/v1/movies" to handle GET request to get a list of the movies

```

```

- Now, for the route "/api/v1/movies", define a handle to handle POST request that creates a new movie

```

```

- Now, for the route "/api/v1/movies/:id", define a handle to handle PATCH request that updates the details for a particular movie using the ID field provided as 
route parameter

```

```


- Now, for the route "/api/v1/movies/:id", define a handle to handle PATCH request thaat deleted particular movie using the ID field provided as route paramter

```

```



