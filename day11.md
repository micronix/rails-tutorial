# Daily ActiveRecord Exercise

In the toy app create a model to keep track of books you want to read, have read or are reading.

Your model Book should have the following attributes:

- title
- author
- published
- description
- state (read, reading, or future)

Create a model with these columns, and run the migration and add 3 books

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
