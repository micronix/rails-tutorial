[Video]()
Quiz: https://goo.gl/forms/7ObBJbRgATCY3jni2
Feedback Form: https://goo.gl/forms/rpoc3YWq33EpcOJ03

Reading: Watch Day20 video and do the project

## Questions
- get better at git (https://classroom.udacity.com/courses/ud775)
- get better at views (https://classroom.udacity.com/courses/ud304)

## Daily Exercise

Last time we created an app to keep track of products for our store. We didn't
have enough time to add validations and categories.

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
