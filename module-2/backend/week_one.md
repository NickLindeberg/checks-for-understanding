## Week One - Module 2 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week (which is a TON!).

Note: When you're done, submit a PR.

### Week 1 Questions

1. List the five common HTTP verbs and what the purpose is of each verb.
  GET - Read
  PUT - Update/Replace
  PATCH - Update/modify
  DELETE - Delete
  POST - Create

2. What is Sinatra? A DSl written in Ruby.  It's a database framework

3. What is MVC? Model View Controller.  Coding setup meant to help connect backend data with user-interfaces.  

4. Why do we follow conventions when creating our actions/path names in our Sinatra routes? It helps the end user readability

5. What types of variables are accessible in our view templates without explicitly passing them? params

6. Given the following block of code, how would I pass an instance variable `count` with a value of `1` to my `index.erb` template?

  ```ruby
  get '/horses' do
    @count = 1
    erb :index
  end
  ```

7. In the same code block, how would I pass a local variable `name` with a value of `Mr. Ed` to the view? name = 'Mr. Ed'

8. What's the purpose of ERB? Ebedded ruby in HTML so we can do ruby functionality within HTML.  

9. Why do I need a development AND test database? A dev database my be quite large.  Test data can help speed up the test process

10. What is CRUD and why is it important? Create, Read, Update and Delete.  It helps programs run more efficiently.  

11. What does HTTP stand for? Hyper Text Transfer Proticol

12. What are the two ways to interpolate Ruby in an ERB view template? What's the difference between these two ways?  don't know at this point

13. What's an ORM? What does it do? Object Relational Maps. It helps us interact with databases

14. What's the most commonly used ORM in ruby (Sinatra & Rails)? SQL, mysql, activerecord

15. Let's say we have an application with restaurants. There are seven verb + path combinations necessary to provide full CRUD functionality for our restaurant application. List each of the seven combinations, and explain what each is for.

16. What's a migration?  Helps us create a table with certain parameters

17. When you create a migration, does it automatically modify your database? no. you have to run rake db:migrate

18. How does a model relate to a database?  Connected to the controller

19. What is the difference between `#new` and `#create`? new creates a instance of something, create saves it to a database

20. Given a table named `animals`, What is the SQL query that will return all info from that table?
    `id     name        number_of_legs
    -----   ------      --------------
      1     panda       4
      2     giraffe     4
      3     whale       0
      4     bird        2
    `
    SELECT * FROM animals;

21. Using the same table, What is the SQL query that will return only the animals that has 4 legs?

SELECT * FROM animals WHERE number_of_legs=4;


### Review Questions:  
22. Given a CSV file (“films.csv”) with these headers [id, title, description], how would you load these into your database to create new instances of Film?  

23. Given the following hash:
```
activities = {
  hiking: {cost: $0, supplies: ['hiking shoes', 'water', 'compass']},
  karaoke: {cost: $10, supplies: ['courage', 'microphone']},
  brunch: {cost: $35, supplies: ['mimosa flutes']},
  antiquing: {cost: $200, supplies: ['list of antique stores']}
}
```

activities[:hiking][:supplies] << "granola bar"
How would I add 'granola bar' to things you should have when hiking?

24. What are the 4 Principles of OOP? Give a one sentence explanation of each.



### Self Assessment:
Choose One: (erase the others)

* I was able to answer a few questions independently, but relied heavily on outside resources

Choose One:

* I feel overwhelmed by the content presented this week
