[Video]()

Reading: Finish Chapter 10

## Questions
- routes
- what to put into the views?
- what to put into the controller?

## Daily Exercise

The rest of the class we will also be using github so create an account on github.com.

Today the exercise will involve validations & drop downs. We are creating an online store. We will also be creating a new rails app and uploading our completed app to github. We will perform the following tasks:

### Prepare the code

- create a new rails app called rails-store
- run the command `git init` inside the directory to initialize the git repository
- create a github repository
- follow the instructions on the github page to upload your app to github

### Create the model

Our model `Product` should have the following columns:

- name
- description
- picture_url
- price

### Create the `Products` controller

You need to create a products controller with the following actions:

- index
- new
- create
- edit
- update
- show

Create the views for each action, and add the routes to the router.

At the end you should be able to add and update products

### Validations

Add validations to your model and check that the model was saved, if it was not
then show the form again with the errors.

Use `form_for` instead of form_tag and `text_field` instead of `text_field_tag`

### Categories

Create a categories model with a controller and create the CRUD actions for the
categories. The url to see the categories should be `/categories`.

### Associate Products to Categories

Each product should belong to only one category so we will add a column
`category_id` to the product.

We then want to add a dropdown so that we can select which category the product
belongs to.


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
