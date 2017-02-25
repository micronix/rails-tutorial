# Daily ActiveRecord Exercise

You are in charge of coordinating a guest list for a birthday party. Here is the information that you want to keep from each guest:

- first_name
- last_name
- address
- city
- state
- zip
- guests (number of extra guests they are bringing)
- contribution (the dish/drink they are bringing to share, i.e. "pizza", "carrots", "soda")

Complete the following tasks:

- create the model using `rails g` the name of the model should be Invitation
- edit the migration file to add the columns listed above
- run the migration with rails db:migrate
- run the following code to create several guests in the rails console

```ruby
Invitation.create(first_name: 'Bob', last_name: 'Burks', address: '123 Pine St', city: 'Raleigh', state: 'NC', zip: '27605', guests: 0, 'Rice')
Invitation.create(first_name: 'Paul', last_name: 'Olive', address: '777 Cina Way', city: 'Durham', state: 'NC', zip: '27717', guests: 1, 'Sodas')
Invitation.create(first_name: 'Jean', last_name: 'Smith', address: '823 Ilene Rd', city: 'Raleigh', state: 'NC', zip: '27604', guests: 3, 'Pizza')
Invitation.create(first_name: 'Daniel', last_name: 'Jenkins', address: '324 Tess St', city: 'Cary', state: 'NC', zip: '27513', guests: 0, 'Cups & Plates')
Invitation.create(first_name: 'Olga', last_name: 'Smith', address: '321 Pine St', city: 'Cary', state: 'NC', zip: '27513', guests: 1, 'Cake')
Invitation.create(first_name: 'Mary', last_name: 'Burks', address: '7 Olyx Way', city: 'Raleigh', state: 'NC', zip: '27605', guests: 0, 'Salad')
Invitation.create(first_name: 'Ashley', last_name: 'Walker', address: '127 Inca Rd', city: 'Apex', state: 'NC', zip: '27502', guests: 2, 'Pasta')
Invitation.create(first_name: 'Todd', last_name: 'Gravel', address: '877 White Rd', city: 'Raleigh', state: 'NC', zip: '27603', guests: 0, 'Carrots')
```

Your task is to write code to get the following information:

- Load the invitation for Bob
- Load the invitation for Mr. Jenkins
- Load all the invitations from Raleigh
- Load the invitation bringing Pasta
- Load all the invitations with last name Smith
- Load all the invitations from Raleigh
- Write code that returns total number of invitations
- Write code that returns number of invitations from Raleigh
- Write code that returns number of invitations with last name Smith
- Write code that returns number of invitations from zip code 27603
- Write code that returns number of invitations from Florida
- Load all guests bringing guests with them
- Write code that returns number of total guests coming to the party (remember the guests column only shows the number of extra guests)
