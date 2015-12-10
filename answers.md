#Rails Questions
1. What is a strength of Rails (or something you like about Rails)?
  - Rails allows for quick setups, fewer typo mistakes

2. What is the name of the server Rails comes with, and what is the name of the database it comes with?
 - SQLite3 is the DB
 - WEBrick  is the server

3. What is a "resource"?
 - A collection of similar objects

4. What is a "controller"? How is it different from a "route"?
 - Where info is collected, multiple route

5. In Express, server.js contained our routes. Where was controller logic defined in our Express projects?
 - On the client js page

6. Look at app/views/layouts/application.html.erb. What does this file remind you of, and what does it contain?
 - Handlebars, html and the data "tags"

7.1 What does the first line ArticlesController < ApplicationController mean?
 - ArticlesController inherits from ApplicationController, its a subclass

7.2 . How does the new method know which view to display?
 - From the routes.rb file

7.3Why does @article have that @?
 - It's an instance variable

8. What is Active Record? What was the equivalent tool we used with Express?
 - It formats the article, like the Schema

9. What is a "migration"?
 - Create and modify tables in db

10. List at least one question you have about Rails (can go over 8 words if needed).
 - Is it like handlebars where its easier to get started but changing/overriding something is complicated?