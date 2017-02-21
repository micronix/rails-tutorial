# Daily ActiveRecord Exercise

In the toy app create a model to keep track of books you want to read, have read or are reading.

Your model Book should have the following attributes:

- title
- author
- published
- description
- state (read, reading, or future)

Create a model with these columns, and run the migration and add 3 books

Step 1

```bash
rails generate model <ModelName>
```

Step 2
Edit the migration file

Step 3
```bash
rails db:migrate
```

Step 4
```bash
rails c
```

Step 5
```bash
b = Book.new
b.title = "The Iliad"
b.author = "Homer"
b.published = "1987-10-01"
b.description = "Voyage story"
b.state = "read"
b.save
```



What will the following ruby expressions be?

- Book.count
- Book.first
- Book.last
- Book.find_by title: "The Iliad"
- Book.find_by title: "ABC"
- Book.where(title: "The Illiad")
- Book.where(title: "ABC")
- Book.where(author: "Homer")
- Book.where(state: "read")
- Book.where(state: "read").count


# Model inheritance

User inherets from ApplicationRecord
ApplicationRecord inherets from ActiveRecord::Base

# Validations

- types of validations
- validation error messages
