# <img src="https://cloud.githubusercontent.com/assets/7833470/10899314/63829980-8188-11e5-8cdd-4ded5bcb6e36.png" height="60"> Intro Rails Reading

**Objective:** Rails has excellent learning resources available online. Today, you'll look at your first of many <a href="http://guides.rubyonrails.org" target="_blank">Rails Guides</a>:

  * <a href="http://guides.rubyonrails.org/getting_started.html" target="_blank">Getting Started</a> (through section 5.7)
  * <a href="http://guides.rubyonrails.org/active_record_basics.html" target="_blank">Active Record Basics</a> (chapters 1, 2, and 5)

Get in the habit of exploring Rails Guides as you approach new topics in Rails!

## Getting Started

1. Fork this repo, and clone it into your `develop` folder on your local machine. Create a new file called `answers.md`.

2. In a different directory (outside `intro-rails-reading`), **read and complete** the <a href="http://guides.rubyonrails.org/getting_started.html" target="_blank">Getting Started</a> tutorial steps through section 5.7 (Showing Articles). Don't worry if you don't quite understand everything you're doing yet.

3. Also, read chapters 1, 2, and 5 of the <a href="http://guides.rubyonrails.org/active_record_basics.html" target="_blank">Active Record Basics</a> guide. You don't need to incorporate these into your Getting Started project; just look over the syntax.

4. **As you work through the guides**, answer the following [questions](#questions) in your `answers.md` file (in your `intro-rails-reading` directory). **Each answer should be 8 words or less!**

## Questions

1. What is a strength of Rails (or something you like about Rails)?

2. What is the name of the server Rails comes with, and what is the name of the database it comes with?

3. What is a "resource"?

4. What is a "controller"? How is it different from a "route"?

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

## Submission

* As you make code changes, frequently commit and push to GitHub.
* Once you've finished the assignment and pushed your work to GitHub, make a pull request from your fork to the original repo.
