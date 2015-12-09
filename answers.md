What is a strength of Rails (or something you like about Rails)?
- easily spin up a fairly complex app in a short amount of time (aka it does a lot of backend processes for you)

What is the name of the server Rails comes with, and what is the name of the database it comes with?
- server: 
- db: sqlite3

What is a "resource"?
- a collection of similar objects

What is a "controller"? How is it different from a "route"?
- A "controller" executes code between the server and the view

In Express, server.js contained our routes. Where was controller logic defined in our Express projects?
- Inside of each server route

Look at app/views/layouts/application.html.erb. What does this file remind you of, and what does it contain?
- hbs, and it contains html/css/some minor logic

The app/controllers/articles_controller.rb file looks like this:

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

What does the first line ArticlesController < ApplicationController mean?
- it's inheriting from the ApplicationController (which is built into RoR)

How does the new method know which view to display?
- routes

Why does @article have that @?
- because it's an instance variable

What is Active Record? What was the equivalent tool we used with Express?
- the "Model" part of MVC, works with the business objects

What is a "migration"?
- Ruby classes that create and modify database tables

List at least one question you have about Rails (can go over 8 words if needed).
- When should code go outside a model, controller or view?