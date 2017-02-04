[Class Video](https://www.youtube.com/watch?v=fOo7ceW-J2o)
## Embeded Ruby

```erb
<html>
  <%= "hello" %>
</html>
```

```erb
<html>
  <body>
    <%= 2 + (3 - 1) * 2 %>
  </body>
</html>
```

```erb
<html>
  <body>
    <% "hello" %>
  </body>
</html>
```

```erb
<html>
  <body>
    <%= list = [1, 2, 3] %>
  </body>
</html>
```

```erb
<html>
  <body>
    <% list = [1, 2, 3] %>
    <% list.each do |i| %>
      <div><%= i %></div>
    <% end %>
  </body>
</html>
```

```erb
<html>
  <body>
    <% if 5 > 2 %>
      <%= "YES" %>
    <% end %>
  </body>
</html>
```

```erb
<html>
  <body>
    <%= puts "hello there" %>
  </body>
</html>
```

```erb
<html>
  <body>
    <%= @person %>
  </body>
</html>
```

## Controller -> Views

A view is like a method that gets added to the controller. When you set an instance variable in the controller, that variable will be available in the view.
