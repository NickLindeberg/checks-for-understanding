### Week 5 Questions

Re-pull from this repository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week (which is a TON!).

Note: When you're done, submit a PR.

### Week 5 Questions
1. How do we make flash messages display on a page?
in the controller we use flash[:notice] "message"

2. Where is cart information/temporary information usually stored? In the session

3. What might be some reasons not to store a cart in our database? Are there any reasons why we would want to persist that information? If our customer database is small, storing in our database wouldn't be that big of a deal.  However, if you app gets popular, that is a lot of information to store.  

4. What is the purpose of the asset pipeline? A place to store all of our javascript and other images that we'd like to access.

5. Why do we precompile our assets?  It takes all of our files such as mutliple style sheets and smashes them into one file to cut down on load time.  

6. What do each of the following tags do?

```ruby
<%= stylesheet_link_tag "application" %>
gives you access to application.css
<%= javascript_include_tag "application" %>
gives you access ot the javascript style sheet
<%= image_tag "rails.png" %>
loads an image from your public folder for rendering
```

7. What are some of the elements of a great read me? What are some of the benefits of taking the time to update a readme for our project?  The main takeaway i got was to explain your app and to make sure that people are able to install your app.  If they can't figure out how to look at your code, you won't get much feedback, if at all.

8. What are the top four accessibility issues that we as developers should be aware of?  I'm not sure if we covered that or not.  

9. `before_save` is an example of a what? Where in our Rails application would we find a `before_save`? Poro or call back at the top of our controllers.  

10. Given the following object, how would we create a scope for all users who are active?

```ruby
User.create(name: "Happy", active: true)
```
I'm not sure...

11. What is the difference between a scope and a class method?
Also not sure if we talked about this or not.  

### Review Questions:  
12. Given the following hash:  

```ruby
{cart: {"17" => 4, "204" => 52, "29" => 22}}
```

  12a. How would you add item with id of 48 with a quantity of 4?  hash[:cart]['48'] = 4
  12b. How would you increase the quantity of item 29?  hash[:cart][:29] += number
  12c. How would you find out how many items your user is thinking about purchasing?  
  hash[:cart].inject.Hash.new{} do |sum, (id, quantity)|
    sum += quantity
  end

13. What is polymorphism? How does it relate to duck-typing? What are two ways you use this in everyday Rails applications?  It's a classes ability to inherit from other class methods.  Such as ApplicationRecord and ApplicationController in our rails app.  
14. How would you clean the string "(630) 854-5483" to "630.854.5483"?  
string.strip

### Self Assessment:
Choose One:
** not sure if we even talked about a few of them.  
* I was able to answer most questions independently, but utilized outside resources for a few

Choose One:
* I feel comfortable with the content presented this week
