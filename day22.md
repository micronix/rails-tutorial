[Video](https://www.youtube.com/watch?v=T4ftN3GIFQ8)

Feedback Form: https://goo.gl/forms/8c4Vy1eFbXfvFT9X2

Reading: Complete until section 11.2.3

## Daily Exercise

When we did our app, I created the app ignoring some of the magic that can happen in rails. This was on purpose so that you can understand the magic better. Every time you are trying grasp a concept ask yourself what is the deeper meaning and try to really understand how it works, not just emulate what is being presented.

We will look at some of the shortcuts that would have aid us in writing an app

### use of resources in routes to generate routes

```
  resources :products
```

### named routes

```
  products_path
```

### form_for

```
form_for vs form_tag
```

### Review of Categories

We will go over any questions related to how to add a product to a category

### Create a show Category Page

### Creating Tests for our App

### Rubocop addition

## Homework

For next Saturday you will need to create an app that keeps track of books with
the following properties:

- title
- description
- pages
- author_id
- amazon_url
- picture_url

Also create an author model with the following properties:

- first_name
- last_name
- picture_url
- bio

Think about the similar patterns in the products app and how it would relate to our books app. In this example instead of products we have books, instead of categories we have authors. Think about the similarities between the two patterns but also try to be creative with how display information differently.
