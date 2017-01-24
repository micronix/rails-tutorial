# Git Exercise

- create directory
- initialize git directory
- create a text file called **README.md** and add some text to it
- commit the file

Make sure that at this point **git log** gives you a history of your first commit

- create a new branch called **feature1**
- create a ruby file called **main.rb** and make it print "hello world"
- add some more text to **README.md**
- commit the new file **main.rb** and **README.md**
- merge branch **feature1** into the **master** branch

At this point **git log** should have 3 entries what are they?

Useful commands
```
git status
git log
git checkout -b <branch-name>
git checkout master
git add .
git commit -m "<message>"
```

# Remote Git Repositories

All the git information, in this case history is stored locally in your computer. When working with other developers we want to store

## Exercise

- create a repository on bitbucket
- add a link from your repository to the bitbucket repository
- push the master branch to the bitbucket repository

Usefule Commands
```
git remote -v
git remote add origin <remote-url>
git push -u origin master
```


# Thinking about models

When creating any application you have to think about storing information. Even the simplest programs can store some sort of information. There are many ways of storing information. You can store information in a file in human readable format for example:

```
tuesday
2 scoops of straberry
Wed
1 scoop of chocolate
1 scoop of vanilla
thursday
half a scoop of chocolate
2 scoops of straberry
```

This is how much ice cream and what flavors I at each day in the past week. This is easy to understand for us, but it's not for a computer. There is no structure to the data. One way to organize data is to use a grid, think of an excel or google spreadsheet.

| Day | Amount | Flavor |
|-----|--------|--------|
| Tue |  2     | straberry |
| Wed | 1      | chocolate |
| Wed | 1      | vanilla |
| Thu | 0.5    | chocolate |
| Thu | 2      | straberry |

This is a lot easier for a computer to understand and a lot easier for a computer to search and manipulate the data. The main reason to organize data like this is to be able to perform **queries** or questions to the database.

Example questions:

- How much total ice cream did I eat on Wednesday?
- How much total chocolate ice cream did I eat this week?
- What is my favorite ice cream flavor?

The above *spreadsheet* we created is called a **table** in the database world.

# Exercise

Let's say that I have a whole bunch of rare movies that my friends love to borrow. Let's take a look at piece of paper I've been using to keep track of the movies my friends borrowed


- Bob borrowed the Matrix on 12/08
- Lent Marry Star Wars Monday
- ~~Steve - Sharknado 02/11~~
- Bob borrowed Gravity 2/11

Create a spreadsheet table that organizes the import parts of the information
