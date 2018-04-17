# Junior Internship code and learning challenge

1. Install RubyOnRails (preferably on a Linux or OSX environment, in a virtual machine if you wish, windows is also possible but harder). http://rubyonrails.org/
2. Install git and configure a gilab account. https://www.youtube.com/watch?v=7p0hrpNaJ14
3. Follow the RubyOnRails getting started: http://guides.rubyonrails.org/getting_started.html
  * Every step should be commited in git.
  * Only the steps on this page are required. You can, but are not expected, to go through the other pages of the guide.
4. BONUS : Once the guide is complete, you should have an article model, controller and views:
  * 4.1 Add a Rating model and database migration with the following requirements:
    - Rating should have an attribute "score" (of the type of your choice).
    - One article can be associated to multiple ratings.
  * 4.2 Add an action on 'app/views/articles/index.html.erb' to allow the user to give a rating on an article. Rating should be a number from 1 to 5.
  * 4.3 Bonus point : on 'app/views/articles/index.html.erb' add the average rating for each article. It should be based on all the ratings for the article.