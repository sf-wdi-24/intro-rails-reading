**What is a strength of Rails (or something you like about Rails)?

Write less code but accomplish a lot more.

**What is the name of the server Rails comes with, and what is the name of the database it comes with?

WEBrick Server, SQLite3 Database

**What is a "resource"?

A collection of similar objects

**What is a "controller"? How is it different from a "route"?

-A controller receives specific requests for the app
-A route reorganize URLs and dispatches them to controllers's action

**In Express, server.js contained our routes. Where was controller logic defined in our Express projects?

In each routes such as GET, POST, PUT, DELETE

**Look at app/views/layouts/application.html.erb. What does this file remind you of, and what does it contain?

Handlebars. But in Ruby, we use ERB Templatting

**The app/controllers/articles_controller.rb file looks like this:

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

Class ArticlesController inherits from class ApplicationController

-How does the new method know which view to display?
RESTful routes

-Why does @article have that @?

It's an instance variable

**What is Active Record? What was the equivalent tool we used with Express?

It's a model which represent data and its logic. 
It's like Model in Express, specificlly Schema

**What is a "migration"?

Class used to create or modifiy databases table

**List at least one question you have about Rails

As new developers in the industry, are we being expected to understand all the syntaxs of Rails packages after init a Rails project?

