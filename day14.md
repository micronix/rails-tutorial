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
Ticket.create(first_name: 'Bob', last_name: 'Burks', source: 'SFA', destination: '', seat: 'A3', flight: '764')
Ticket.create(first_name: 'Paul', last_name: 'Olive', source: 'SFA', destination: '', seat: 'A7', flight: '764')
Ticket.create(first_name: 'Jean', last_name: 'Smith', source: 'JFK', destination: 'RDU', seat: 'A19', flight: '87')
Ticket.create(first_name: 'Daniel', last_name: 'Jenkins', source: 'JFK', destination: 'RDU', seat: 'E7', flight: '87')
Ticket.create(first_name: 'Olga', last_name: 'Smith', source: 'LAX', destination: 'LAX', seat: 'E19', flight: '123')
Ticket.create(first_name: 'Mary', last_name: 'Burks', source: 'LAX', destination: 'LAX', seat: 'E5', flight: '123')
Ticket.create(first_name: 'Ashley', last_name: 'Walker', source: 'RDU', destination: 'LAX', seat: 'E5', flight: '87')
Ticket.create(first_name: 'Todd', last_name: 'Gravel', source: 'RDU', destination: 'LAX', seat: 'B3', flight: '99')
```

- SFA tickets are missing destrination to Miami
- LAX tickets should actually go to chicago
- Daniel Jenkins should actually go from RDU to JFK


```ruby
Flight.create(number: '764', aircraft: '747', departure: '2017-03-05 11:10 AM')
Flight.create(number: '87', aircraft: '737', departure: '2017-03-05 12:05 AM')
Flight.create(number: '123', aircraft: '747', departure: '2017-03-05 1:10 PM')
Flight.create(number: '99', aircraft: '747', departure: '2017-03-05 9:00 AM')

```
