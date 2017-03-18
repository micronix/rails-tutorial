[Video]()

Reading: Finish Chapter 9

## Questions

## Daily Exercise

A todo list is one of the first apps that people do when learning a platform. We will go over the same procedure as last time here is the model:

**Task**
- title
- complete

Like last time create the following actions

- index: "/tasks" using a GET request
- new: "/tasks/new" using a GET request
- create "tasks" using a POST request

You need to add the following logic to each action
- index: load all tasks
- new: you should create a form to save the recipe
- create: you should save the recipe

## Make the tasks more user friendly
- make a url /todo instead of tasks
- add a form to the index view to create tasks from the index view
- ability to edit inline
- ability to complete task from the application

## Params Review

### GET request parameters

```ruby
Rails.application.routes.draw do
  get "/blog", to: "blog#index"
end
```

If we go to the url `blog?test=1` we get the following params

```
params: {"test": "1"}
```


### PATH request parameters

```ruby
Rails.application.routes.draw do
  get "/blog", to: "blog#index"
  get "/blog/:id", to: "blog#show"
end
```

If we go to the url `blog/asf` we will get the following params

```
params: {"id": "asf"}
```

### POST/PATCH parameters

```erb
<% form_tag %>
<%= text_field_tag :name %>
<%= text_field_tag :body %>
<%= submit_tag "submit"
<% end %>
```

```
params: {"name": "asd", body:"abc"}
```


## Meta

## Possible Topics
- Flash
- Params
- Session
- Environments
- Gravatar
- Unsuccessful signups
- Strong Params
- SSL
