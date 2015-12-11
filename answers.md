## Questions

1. What is a strength of Rails (or something you like about Rails)?
	
	It gives a consistent, semi-preordained shape to the project 


2. What is the name of the server Rails comes with, and what is the name of the database it comes with?

	WEBrick is the default server; SQLite is the db.


3. What is a "resource"?

	

4. What is a "controller"? How is it different from a "route"?

	It is where info/data is collected to be provided by the view. 



5. In Express, `server.js` contained our routes. Where was controller logic defined in our Express projects?

	

6. Look at `app/views/layouts/application.html.erb`. What does this file remind you of, and what does it contain?
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
  * How does the `new` method know which view to display?
  * Why does `@article` have that `@`?

8. What is Active Record? What was the equivalent tool we used with Express?

9. What is a "migration"?

10. List at least one question you have about Rails (can go over 8 words if needed).

