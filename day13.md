# Daily ActiveRecord Practice

Your ActiveRecord model you will keep track of patients at a hospital. Here are the columns:

- first_name
- last_name
- dob (when they were born)
- admitted (when they were admitted to the hospital)
- released (when they were released from the hospital)
- illness (reason for being admitted to the hospital)

- create the model Patient
- run `rails db:migrate`
- run the following code to populate some data in your database

```ruby
Patient.create(first_name: 'Bob', last_name: 'Burks', dob: '1992-10-01', admitted: '2016-12-04', released: '2017-02-25', illness: 'cancer')
Patient.create(first_name: 'Paul', last_name: 'Olive', dob: '1962-09-05', admitted: '2016-12-02', released: '2016-12-13', illness: 'flu')
Patient.create(first_name: 'Jean', last_name: 'Smith', dob: '1992-10-01', admitted: '2016-12-20', released: '2017-02-15', illness: 'cancer')
Patient.create(first_name: 'Daniel', last_name: 'Jenkins', dob: '1984-04-05', admitted: '2017-02-01', released: '2017-02-01', illness: 'broken bone')
Patient.create(first_name: 'Olga', last_name: 'Smith', dob: '1982-05-05', admitted: '2017-01-01', released: '2017-01-04', illness: 'flu')
Patient.create(first_name: 'Mary', last_name: 'Burks', dob: '1972-04-01', admitted: '2017-02-25', released: nil, illness: 'flu')
Patient.create(first_name: 'Ashley', last_name: 'Walker', dob: '2005-04-01', admitted: '2017-02-10', released: nil, illness: 'broken bone')
Patient.create(first_name: 'Todd', last_name: 'Gravel', dob: '1942-02-14', admitted: '2017-02-20', released: nil, illness: 'crash')
```

- how many Smiths were patients?
- how many patients are still in the hospital?
- how many patients were admitted in 2016
- how many patients were admitted in 2017
- create a hash that tells us how many patients got each illness
- who is the oldest patient?
- who is the youngest patient?
- write code that calculates the age of a patient
- write code that determines how many days a patient has been in the hospital
- come up with 3 other types of questions you could ask about the patients

[Video](https://www.youtube.com/watch?v=vJG698U2Mvo)
