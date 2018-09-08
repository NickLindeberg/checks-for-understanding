## Week Four Recap

### Instructions
Fork or re-pull this repository. Answer the questions to the best of your ability.

Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week.

Note: When you're done, submit a PR with a reflection in the comments about how this exercise went for you.

### Week 4 Questions

1. What is a cookie? A cookie is a small amount of information, stored by the client, that is used by websites to remember information about the user.   
2. What’s the difference between a session and a cookie? A session is like a cookie except that it's stored by the website instead of the client.  
3. What’s a flash and when do you want to use flashes? Its a way to display information to your user.  I generally use them in create or delete methods in my controller to let people know that the button actually did something.  
4. Why do people say “HTTP is stateless”? It means the connection between the server and brower is lost as soon as the transaction is ended.  
5. What’s authentication? Explain. See below.  
6. What’s the difference between authentication and authorization? Authentication is a way to figure out if your user is who they say they are by logging in to your app or signing up as a new user.  Authorization is what they are able to do once they have logged in. For instance, your admin may be able to delete information on your website but you wouldn't want a standard user having that kind of power.  
7. What’s a before filter? It goes in your controller and it is a way you can limit information used in authorization.  You can also use them for a setup method in testing.  I'm sure there are other things you can do with them.   
8. How do we keep track of a user once they’ve logged in?  You save their information in the session.  
9. When do you want to namespace a resource? When do you want to nest a resource? What's the differences between those two approaches?  We use namespace as a shortcut for scope + module + as.  It cleans up our routes file and makes it easier to read.  The downside is that it's less configurable than scope + module + as.  
10. At a high level, what tools can you use to implement authorization? How would you use them? You store the information in the session and then limit the user to what you deem they can or can't see.  You can say "if current_user" before methods and pages you would like them to be able to see or interact with.  
11. What's an enum, and what advantages does it offer? What data type needs to be in your database to use an enum? Where do you declare an enum?It's an active record method that can help us give authorizations to users or admins through our our user model.  
12. What are some strategies you can use to keep your views DRY? I use form_for to call from my other views within a certain type of views.  


### Reviews Questions
13. Given the following array of hashes, how would I print an alphabetical list of holidays?
```ruby
[
 {holiday: {name: "St Patrick's Day", supplies: ["Corned Beef and Cabbage"]}},
 {holiday: {name: "Halloween", supplies: ["Candy", "Costume"]}},
 {holiday: {name: "Hanukkah", supplies: ["Menorah"]}}
]
```  
hash.each do |t|
  t.[0]
end
14. How would you clean incoming data to ensure "$300" or "300.00" is stored as 300? .to_i


### Self Assessment:
Choose One:
* I was able to answer most questions independently, but utilized outside resources for a few

Choose One:
* I feel comfortable with the content presented this week
