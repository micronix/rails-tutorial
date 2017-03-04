# Daily Active Record practice

You are an airline company and want to keep track of passenger tickets.

- first_name
- last_name
- source airport
- destination airport
- seat
- flight#

For this exercise create a model called Ticket, edit the migration and run the migration. Then run the following code to create a few items in the database


```ruby
Ticket.create(first_name: 'Bob', last_name: 'Burks', source: '', destination: '', seat: 'A3', flight: '764')
Ticket.create(first_name: 'Paul', last_name: 'Olive', source: '', destination: '', seat: 'A7', flight: '764')
Ticket.create(first_name: 'Jean', last_name: 'Smith', source: '', destination: '', seat: 'A19', flight: '87')
Ticket.create(first_name: 'Daniel', last_name: 'Jenkins', source: '', destination: '', seat: 'E7', flight: '87')
Ticket.create(first_name: 'Olga', last_name: 'Smith', source: 'LAX', destination: '', seat: 'E19', flight: '123')
Ticket.create(first_name: 'Mary', last_name: 'Burks', source: 'LAX', destination: '', seat: 'E5', flight: '123')
Ticket.create(first_name: 'Ashley', last_name: 'Walker', source: 'RDU', destination: '', seat: 'E5', flight: '87')
Ticket.create(first_name: 'Todd', last_name: 'Gravel', source: 'RDU', destination: '', seat: 'B3', flight: '99')
```