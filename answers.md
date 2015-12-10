Questions

1. What is a strength of Rails (or something you like about Rails)?

It's opinionated software that makes assumptions.

2. What is the name of the server Rails comes with, and what is the name of the database it comes with?

Server: WEBrick. Database: SQLite3

3. What is a "resource"?

A collection of similar objects, such as animals or people.

4. What is a "controller"? How is it different from a "route"? 

Receive specific requests for the application. A route decides which controller receives a request.

5. In Express, server.js contained our routes. Where was controller logic defined in our Express projects?

in the app.get function- app.get('route', function(req, res) {..})

6. Look at app/views/layouts/application.html.erb. What does this file remind you of, and what does it contain?

It reminds me of HTML and contains HTML

7. The app/controllers/articles_controller.rb file looks like this:

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

-What does the first line ArticlesController < ApplicationController mean?

A controller class inherits from Application controller

-How does the new method know which view to display?

The articles controller class above it

-Why does @article have that @?

Hold a reference to the article object

8. What is Active Record? What was the equivalent tool we used with Express?

Mongoose

9. What is a "migration"?

Ruby classes that make it simple to create and modify database tables

10. List at least one question you have about Rails (can go over 8 words if needed).

Does Rails ever get confused/ do the wrong thing with so many things being automated, like a gem stop working or something?