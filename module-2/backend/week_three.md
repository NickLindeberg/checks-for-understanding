## Week Three Recap

### Instructions
Fork this repository. Be sure to pull the latest changes to your local repo. Answer the questions to the best of your ability.

Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week.

Note: When you're done, submit a PR with a reflection in the comments about how this exercise went for you.

### Week 3 Questions

1. What is the entry at the command line to create a new rails app? $ rails new project_name -T -d="postgresql" --skip-turbolinks --skip-spring
2. What do Models generally inherit from in rails? ApplicationRecord
3. What do Controllers generally inherit from in a rails project? ApplicationController
4. How would I create a route if I wanted to see a specific horse in my routes file assuming I'm sticking to standard conventions and that I didn't want other CRUD functionality? resources :horse only [:specifichorse]
5. What rake task is useful when looking at routes, and what information does it give you? rake routes (rails routes).  Shows you paths that are avaliable to use
6. What is an example of a route helper? When would you use them?
7. What's the difference between what `_url` and `_path` return when combined with a routes prefix? `_path` is defined by rails and is used to call a certain path created by the migration  
8. What are strong params and why are they necessary?
9. What role does `form_for` play in helping us create our forms? creates form to be able to enter in information to create things in your app.  
10. How does `form_for` know where to submit the user's input? using teh create function
11. Create a form using a `form_for` helper to create a new `Horse`.

<%= form_for @horse do |f| %>
  <%= f.label :name %>
  <%= f.text_field :name %>

  <%= f.submit %>
<% end %>

12. Why do we want to validate our models? To make sure we have access to the correct relationships
13. What are the steps of the DNS lookup?

  -starts at the client
  -looks at local DNS server
  -if local doesn't know information it looks at the root
  -if root doesn't know it looks at the DNS server
  -passes information back to client

### Review Questions
14. Within a feature test and given the following HTML, write the code necessary to target the following section and check the person's name?

  `<section id="personal-info">
    <h3><%= @person.name%></h3>
   </section>
  `

  @person.name
15. How would you call the method `prance` from within the method `move` on a `Horse` instance? Horse.move.prance
16. Given the following hash:

```ruby
furniture = {table: {height: 3, color: "red"}, purchased: true}
```
What is the different between how you would return true vs returning 3?  
furniture[:purchased][3]
17. What is inheritance?
When a class can use methods defined by a parent or super class above.  

### Self Assessment:
Choose One:
* I was able to answer most questions independently, but utilized outside resources for a few

Choose One:
* I feel overwhelmed by the content presented this week
