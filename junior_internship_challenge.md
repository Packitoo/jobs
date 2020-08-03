# JUNIOR DEVELOPER code and learning challenge:

1. Install RubyOnRails 2.4.2 (preferably on a Linux or OSX environment, in a virtual machine if you wish, windows is also possible but harder). http://rubyonrails.org/

2. Install git and configure a gitlab account. https://www.youtube.com/watch?v=7p0hrpNaJ14
  * make sure your project is public so we can see your code.

3. Follow the RubyOnRails getting started: http://guides.rubyonrails.org/getting_started.html
  * Every step should be commited in git.
  * Bonus point will be accorded if you use git branches and merging between branches

4. Once the guide is complete, you should have an article model, controller and views:
  * 4.1 Add a "Rating" model and database migration with the following requirements:
    - Rating should have an attribute "score" (of the type of your choice).
    - One article can be associated to multiple ratings. (see https://guides.rubyonrails.org/association_basics.html for help)
  * 4.2 Add an action on 'app/views/articles/index.html.erb' to allow the user to give a rating on an article. Rating should be a number from 1 to 5.
  * 4.3 on 'app/views/articles/index.html.erb' add the average rating for each article. It should be based on all the ratings for the article.

5. The project needs tests, make a controller test using minitest for the following cases:
  * when a user creates a article, the body is expected.
  * when a user creates a rating of 2 and a rating of 5, the average rating is 3.5
  * See https://guides.rubyonrails.org/testing.html

6. Add a function to save article statistics to a CSV file (https://en.wikipedia.org/wiki/Comma-separated_values)

  * The output CSV file should have the first line reserved for headers
  * Following lines each represents an Article, all aticles need be exported
  * The CSV file should have the following attributes for each article:
    - first "column" : title of the article
    - second "column" : the lowest rating
    - third "column" : the highest rating
    - 4th "column" : the average rating
    - 5th "column" : the number of comments
    - 6th "column" :  the average number of characters in the article comments (ie: if the article has 2 comments, 1 first 20 characters long and the second is 40, the average is 30)

# Hints

* Ruby is dynamically typed language. This can be tricky for integer division.
* You can use git to make prototypes without losing your code.
* There is no time limit for this test but average duration for a student developer with no skills in is 2 to 8 hours.
* These steps are the very strict minimum to work as junior developer intern.
* Learn, search, ask questions, be curious and if everything fails ask-us a hint
