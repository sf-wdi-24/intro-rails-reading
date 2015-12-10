# 1. What is a strength of Rails (or something you like about Rails)?

Easy to understand, code and execute 

# 2. What is the name of the server Rails comes with, and what is the name of the database it comes with?

SQLite database and bin/rails server

# 3. What is a "resource"?

Collection of objects - create, read, update and delete 

# 4. What is a "controller"? How is it different from a "route"?

An inherited class that performs CRUD and defines new methods. 

# 5. In Express, server.js contained our routes. Where was controller logic defined in our Express projects?

Main.js

# 6. Look at app/views/layouts/application.html.erb. What does this file remind you of, and what does it contain?

Looks like the html.hbs page with handlebars. Contains html layouts


# 7. What does the first line ArticlesController < ApplicationController mean?
# How does the new method know which view to display?
# Why does @article have that @?

1st line - controller
new method - controllers are empty by default, so actions need be stated
@article - instance variable, attribute 

# 8. What is Active Record? What was the equivalent tool we used with Express? 

Provides functionality to Rails Models. In Express: Node

# 9. What is a "migration"?

Ruby classes to create and change database tables

# 10. List at least one question you have about Rails (can go over 8 words if needed).

1. Will we need PostMan or any other external site to help guide us through making our apps as we learn Ruby? 

