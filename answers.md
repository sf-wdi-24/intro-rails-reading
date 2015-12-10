## Answers

**1. What is a strength of Rails (or something you like about Rails)?**

It is very structured.

**2. What is the name of the server Rails comes with, and what is the name of the database it comes with?**

WEBrick is the server.
SQLite3 is the DB

**3. What is a "resource"?**

A collection of things stored in your DB

**4. What is a "controller"? How is it different from a "route"?**

A controller receives the requests.
There may be several routes on a controller.

**5. In Express, `server.js` contained our routes. Where was controller logic defined in our Express projects?**

In each route (app.get, app.post, app.put, app.delete)

**6. Look at `app/views/layouts/application.html.erb`. What does this file remind you of, and what does it contain?**

The boilerplate html page with cssandjavascript links.
(cssandjavascript is one word, right?)

**7. The `app/controllers/articles_controller.rb` file looks like this:**

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

Create a class ArticlesController, a subclass of ApplicationController.

  * How does the `new` method know which view to display?

It uses RESTful routing

  * Why does `@article` have that `@`?

Because it is an instance variable

**8. What is Active Record? What was the equivalent tool we used with Express?**

Active Record : SQLite3 :: Mongoose : MongoDB

**9. What is a "migration"?**

Flocks of birds that change the database structure.

**10. List at least one question you have about Rails (can go over 8 words if needed).**

What is the weird syntax for HTML?  And does Rails make styling your page more difficult?