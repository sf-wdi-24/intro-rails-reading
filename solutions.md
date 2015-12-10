## Questions

1. What is a strength of Rails (or something you like about Rails)?

It feels very "guided".  And its easy to read. 

2. What is the name of the server Rails comes with, and what is the name of the database it comes with?

Rails server. 

SQL lite 3 is the database

3. What is a "resource"?

A set of files like a collection.   Similar objects. 

4. What is a "controller"? How is it different from a "route"?

The controller makes sense of the route.

The route is the path that the request goes through.  Like to LocalHost: 3000

5. In Express, `server.js` contained our routes. Where was controller logic defined in our Express projects?

Routes.rb

6. Look at `app/views/layouts/application.html.erb`. What does this file remind you of, and what does it contain?

Its like index.hbs.  It's the public, front end file.   It contains site structure like an HTML doc. 

7. The `app/controllers/articles_controller.rb` file looks like this:

	```ruby
	class ArticlesController < ApplicationController
	 	def new
		end

		def create
		  @article = Article.new(article_params)
		  @article.save
		  redirect_to @article
		end

		def show
		  @article = Article.find(params[:id])
		end

		private
		  def article_params
		    params.require(:article).permit(:title, :text)
		  end
	end
	```

  * What does the first line `ArticlesController < ApplicationController` mean?

  Allows for a new page.  A new resource.  Like Create. 

  * How does the `new` method know which view to display?

  We point resources at it. 

  * Why does `@article` have that `@`?

  It's an instance variable. 

8. What is Active Record? What was the equivalent tool we used with Express?

It holds the CRUD routes.   Like our server.js file in Express. 

9. What is a "migration"?

Ruby classes that make it simple to modify database tables. 

10. List at least one question you have about Rails (can go over 8 words if needed).

Is the front-end fully skinnable?  In the blog example, the .erb file seems to take over the client facing page. 

## Submission