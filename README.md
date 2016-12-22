# Rails Commands Quiz

Fork, clone, and write your answers directly in this file. Then submit a pull request.

### Question 1

I want to start a new Rails project/app called `BunnyApp`. What command should I type in the terminal?

**rails new BunnyApp**

### Question 2

I want to create a new model called `Bunny`, with the following attributes: name (string), color (string), and age (integer). What command(s) should I type in the terminal and/or Sublime? (In your answer, create both a migration and the model file.)

**rails generate scaffold Bunny name:string color:string age:integer**

### Question 3

What does the command in Question 2 do, exactly? What files are created, where are they located, and what does the database look like at this time? Explain.

**a full set of model, database migration for that model, controller to manipulate it, views to view and manipulate the data, and a test suite for each of the above.

The generator checks that there exist the directories for models, controllers, helpers, layouts, functional and unit tests, stylesheets, creates the views, controller, model and database migration for Bunny (creating the table and fields), takes care of the route for the resource, and new tests for everything.**


### Question 4

I want to create a database and make it reflect the new model I created in Question 2. What command(s) should I type in the terminal?

**cd BunnyApp**
**rake db:create  or rails db:create**

### Question 5

I want to look at the actual database that has been created. What command should I type in the terminal?

**rails dbconsole**

### Question 6

I want to see a list of all the URLs available in my app, along with the HTTP requests and controllers associated with them. What command should I type in the terminal?

**rake route**

### Question 7

What line should I add to `config/routes.rb` to create a complete set of RESTful routes for a "bunnies" resource?

**resources :bunnies**


### Question 8

According to standard Rails conventions, what directory and filename would the BunniesController be located in, starting from the root of the project?

**BunnyApp/app/controllers**

### Question 9

According to standard Rails conventions, what directory and filename would the "show" view for bunnies be located in, starting from the root of the project?

**BunnyApp/app/views/bunnies**

### Question 10

I have worked on my app and finally want to see it in action. What command should I type in the terminal, and where should I navigate to in my browser?

**rails server**
**http://localhost:3000**
