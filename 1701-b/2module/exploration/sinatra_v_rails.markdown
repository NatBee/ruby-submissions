## Sinatra versus Rails Exploration

### Setup:

First, clone down the Rails project:

```terminal
git clone https://github.com/turingschool/job-tracker.git rails_project
```

And then clone down the Sinatra project:

```terminal
git clone https://github.com/turingschool/bike-share.git sinatra_project
```
Now cd into each project, run `bundle` on each project, and you're ready to go. We will only be looking at the code base and not interacting with the app. If you wanted to run the server and interact with the app, you would need to create your database, migrate your migrations, etc.

### Exercise:

1. Take a look at this stripped down Sinatra app and this stripped down Rails app. How are they different and how are they similar? Identify 5 differences, and for each one describe 1-2 implications. What effect does that difference have for each framework? If you don't know exactly, draw on your knowledge and experience and make some educated guesses/inferences. Also, practice your research skills to look into the differences.

Rails app: The Rails app has 3 controller files that implement ActionController::Base. The rails app companies_controller and jobs_controller looks like CRUD functionality but there are no defined paths.

Sinatra app: The Sinatra app has only one controller file that implements Sinatra::Base. The Sinatra Bike_Share_app isn't built out but I would expect to see CRUD functionality with paths.

Similarities: CRUD, migration to build db and tables, 

5 differences :
  gems:
1 - Rails gem - full stack web framework that favors convention over configuration.

2 - Sinatra gem - Ruby specific DSL for quickly creating web apps.

3 - ActiveRecord gem - Databases on Rails. Tool to build domain model by mapping db tables to Ruby classes.

4 - rspec and rspec core gems - Behavior driven development (BDD) for Ruby 
  -rspec-rails gem - testing framework for Rails.
5 - byebug - anywhere in the code to stop execution and get a debugger console

1. Consulting blogs and commentary you find online, identify 3 similarities between Rails and Sinatra. 

Both are gems. Both frameworks are basically the same. Sinatra is more detailed and Rails simplifies things.  

1. Consulting blogs and commentary you find online, identify 3 things that distinguish Rails, advantages.

Sinatra is better for apis and rails is better for databases. Rails is better for full scale application because it's larger and more robust. It is better for applications with many expected users.

1. In your Rails project, what does the `routes.rb` file inside of the `/config` directory do? What does this correlate to in our Sinatra app?
This routes file defines the routes in one file. This correlates to defining each route in the controller in Sinatra.

1. We teach Sinatra by adding some structures that Sinatra doesn’t need, but help you make the transition between Sinatra and Rails. What does a stripped down implementation of Sinatra look like, and what are the pieces we’ve added for educational purposes?
