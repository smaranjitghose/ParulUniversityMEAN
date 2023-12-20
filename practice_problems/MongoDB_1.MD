# Assignment 1

- Create a database `assignment1` and insert the following into a collection called `movies`

```js
[
    {
        "title": "Fight Club",
        "writer": "Chuck Palahniuk",
        "year": 1999,
        "actors": ["Brad Pitt", "Edward Norton"]
    },
    {
        "title": "Pulp Fiction",
        "writer": "Quentin Tarantino",
        "year": 1994,
        "actors": ["John Travolta", "Uma Thurman"]
    },
    {
        "title": "Inglorious Basterds",
        "writer": "Quentin Tarantino",
        "year": 2009,
        "actors": ["Brad Pitt", "Diane Kruger", "Eli Roth"]
    },
    {
        "title": "The Hobbit: An Unexpected Journey",
        "writer": "J.R.R. Tolkien",
        "year": 2012,
        "franchise": "The Hobbit"
    },
    {
        "title": "The Hobbit: The Desolation of Smaug",
        "writer": "J.R.R. Tolkien",
        "year": 2013,
        "franchise": "The Hobbit"
    },
    {
        "title": "The Hobbit: The Battle of the Five Armies",
        "writer": "J.R.R. Tolkien",
        "year": 2012,
        "franchise": "The Hobbit",
        "synopsis": "Bilbo and Company are forced to engage in a war against an array of combatants and keep the Lonely Mountain from falling into the hands of a rising darkness."
    },
    {
        "title": "Pee Wee Herman's Big Adventure"
    },
    {
        "title": "Avatar"
    }
]

```

Now give the queries to answer the following questions

1. List out all the movie names
2. Details of movies written by "Quentin Tarantino"
3. Name and year of movies in which "Brad Pitt" acted 
4. Movies from "The Hobbit" franchise
5. Movies released in the 90s
6. Movies releasted before 2000 or after 2010
7. Add the follwing synopsis to "The Hobbit: An Unexpected Journey" -

```
"A reluctant hobbit, Bilbo
Baggins, sets out to the Lonely Mountain with a spirited group of dwarves to reclaim their mountain home - and the gold within it - from the dragon Smaug."
```
8. Add the follwing synopsis to "The Hobbit: The Desolation of Smaug" -

```
"The dwarves, along with Bilbo Baggins and Gandalf the Grey, continue their quest to reclaim Erebor, their homeland, from Smaug. Bilbo Baggins is in possession of a mysterious and magical ring."
```

9. Add an actor named `Samuel L. Jackson` to the movie `Pulp Fiction`

10. Find all movies that have a synopsis that contains:
    1. the word "Bilbo"
    2. the word "Gandalf"
    3. the word "Bilbo" but not the word "Gandalf"
    4. the words "dwarves" *or* "hobbit"
    5. the words "gold" *and* "dragon"

11. Remove the records from the collection where the movie title is:
    1. "Pee Wee Herman's Big Adventure"
    2. "Avatar"
