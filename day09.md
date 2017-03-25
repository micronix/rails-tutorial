## Rails HTML helper methods

[Class Video](https://www.youtube.com/watch?v=jttDNC2PPf0)

- link_to
- image_tag

## SCSS

Things to know about scss:

- scss compiles to css on the server
- css is a subset of scss (you can use just plain old css, plus more)
- scss is closer to a language (think variables, inheritance, etc.)

## Partials vs View vs Layout

When rendering an html rails takes the following steps:

- render layout
  - render action view
    - render partial
      - rander partial
    - render partial

```erb
<html>
  <head>
    <title><%= "Home | Rails tutotirla" %></title>
  </head>
  <body>
    <%= yield %>
  </body>
</html>
```

```erb
<h1><%= "Heading" %></h1>
<%= render 'menu' %>
<p>Content</p>
```

```erb
<ul>
  <li>Home</li>
  <li>Users>/li>
  <li>Assignments</li>
</ul>
<%= @user.email %>
```

## Asset Pipeline

A way to manage css, javascript, and images

Browsers like HTML, CSS and Javascript. Sometimes, programmers don't like HTML or Javascript. Don't like CSS, you can use SCSS or LESS. Don't like javascript? You can use coffescript or Typescript.

Reasons for the assets pipeline:

- prevents browser caching problem when developing
- automatically compile scss into css or coffeescript into javascript
- uglify & minify css & javascript in production

## ActiveRecord Exercises

In the toy app create a new model:

```bash
rails g model Car
```

Open the migration in the folder db/migrations and add the following columns to the table creation:

- make of type string
- model of type string
- year of type integer
- price of type float
- color of type string

Run the migration:

```bash
rails db:migrate
```

The table should have been created now.

open up the rails console:

```bash
rails c
```

Create a new car with the following attributes and save to the database:

- make: "Toyota"
- model: "Camry"
- year: 2010
- color: "Green"
- price: 10,012.22

Count how many cars are in the database:

```ruby
Car.count
```
