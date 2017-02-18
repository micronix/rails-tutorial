# ActiveRecord Exercises

In the toy app we want an app that keeps track of different pets in a pet store

To specify the products we should have the following columns:

- name (i.e. Ruby, Roarie, Snurf)
- species (i.e. Cat, Dog, Rabbit)
- dob (i.e. 02/04/12)
- price (500.00)
- notes

Create a model with these column, try to guess what the types of the columns should be.

After updating the migration, open up the console and add 3 new pets.

What would be the ruby expression to

# Add another static page

Let's practice again the process of creating a static page. Here are the steps you need to take:

- Create a new action
- create a new view
- add route to the new action

In the sample app create a new static page that lists the things you will do tomorrow. You might find the ul and the li html elements useful.

# Routes

- convention for specifying a route

get "url" => "controller#action"

# Testing

assert_template
assert_select
