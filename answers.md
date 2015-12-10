1. What is a strength of Rails (or something you like about Rails)?

I really like the simple way to create all we need for the app directly from the terminal in few lines.


2. What is the name of the server Rails comes with, and what is the name of the database it comes with?

Server - config.ru
DB - db/

3. What is a "resource"?

Resource is a collection of similar objects. 

4. What is a "controller"? How is it different from a "route"?

controller receive specific requests for the application. Routing decides which controller receives which requests. 

5. In Express, `server.js` contained our routes. Where was controller logic defined in our Express projects?

In the req.body

6. Look at `app/views/layouts/application.html.erb`. What does this file remind you of, and what does it contain?

It remindes me the html/hbs views. it contain the structure of the view and connection links to the stylseet and JS.

7. 
a. What does the first line ArticlesController < ApplicationController mean?
ArticlesController is a class that inherit from ApplicationController.
We will define in the ArticlesController class methods that will become the actions for this specific controller. These actions will perform CRUD operations on the articles within our system.

b. How does the new method know which view to display?
We send with the function new the params[:article].

c. Why does @article have that @
article is an instance variable and it has the capability of storing data for each instance of a class.

8. What is Active Record? What was the equivalent tool we used with Express?

Active Record supplies functionality to the Rails models, including basic database CRUD operations, data validation, as well as sophisticated search support and the ability to relate multiple models to one another.
In express we have get/post/put/delete and also for data validation we use jQyery validation

9. What is a "migration"?

Rails provides a domain-specific language for managing a database schema called migrations. Migrations are stored in files which are executed against any database that Active Record supports using rake. 
Migration track of which files have been committed to the database and provides rollback features.

10. At this point I really confused about the role of each step to create the app. I would be happy to learn more and understand the equivalent of each operation to Express. Also I don't understant the views structure and what part is front end and what part is the backend (where is my main JS and where I use jQuery?????) 