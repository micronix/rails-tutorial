[Video]()

Reading: Read until 9.1.3 [Params](https://www.youtube.com/watch?v=y57OnWV6dRE&t=15s)

## Questions

## Daily Exercise
You are going to create a recipe site. You are going to have a recipes table:

- title
- description

This is normal, just like we have done in the past.

### Recipes controller

I also want you to create a recipes controller with 3 actions:

- index: "/recipes" using a GET request
- new: "/recipes/new" using a GET request
- create "recipes" using a POST request

You need to add the following logic to each action
- index: load all recipes
- new: you should create a form to save the recipe
- create: you should save the recipe

## Params

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
