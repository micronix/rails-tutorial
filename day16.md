[Video]()

**Reading: Finish Chapter 8**

## Questions

## Daily Exercise

Today's exercise builds on last time's movie database. Today we will 2 tables. You will have to delete the previous movie model with the command `rails d model`.

**Movies**
- title
- description
- year

**Actors**
- first_name
- last_name
- dob
- biography

Our goal is now to create a way to express which actors were in a movie. We want to be able to do something like this in our code to load all the movie actors:

```
movie = Movie.find_by name: '24 Days Later'
actors = movie.actors
```

For this we will need to create a way to store the movie_id, actor_id pairs. This will go in a third table.

**Movies**

| id| title | description | year |
|:--:|:-----:|:-----------:|:----:|
|1 | Lord of the Rings | Hobbits take a ring to a volcano | 2003 |
|2 | Harry Potter | Wizards battle bad guys | 2001 |
|3 | Pirates of the Caribbean | Dead pirates seek treasure | 2003 |

**Actors**

| id| first_name | last_name | dob | biography |
|:--:|:-----:|:-----------:|:----:|:--:|
|1 | Daniel | Radcliff | 1989-07-23 | Born in London |
|2 | Orlando | Bloom | 1977-01-13 | Born in Canterbury England |
|3 | Sean | Austin | 1971-01-25 | From California |
|4 | Johnny | Depp | 1963-06-09 | From Kentucky |

**MovieActors**

|movie_id|actor_id|
|:--:|:--:|
| 1 | 2 |
| 1 | 3 |
| 2 | 1 |
| 3 | 2 |
| 3 | 4 |

## Meta

Introduction the concept of deep work: https://www.youtube.com/watch?v=gTaJhjQHcf8

## Possible Topics
- Flash
- Params
- Session
- Environments
- Gravatar
- Unsuccessful signups
- Strong Params
- SSL
