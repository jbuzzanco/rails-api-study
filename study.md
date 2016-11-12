# Rails as an API Study

Use your favorite search engine and the provided readings to research and answer
the following questions (no prior knowledge is expected).

In your answers, be sure to cite any relevant sources you consulted in your
search. We ask you to write answers in your own words in order to see how you
process what you've read. Please do not answer with direct quotes from source
material. Instead, digest what you've read and repeat it in your own voice.

Please note:

-   Many of the readings will mention the "view" layer. We won't be covering the
    view layer in this program.
-   We'll use our [rails-api-template](https://github.com/ga-wdi-boston/rails-api-template)
    repository as the basis for our rails applications.
    This template excludes the "view" layer.

## Required Readings

-   [Starting Ruby on Rails: What I Wish I Knew | BetterExplained](http://betterexplained.com/articles/starting-ruby-on-rails-what-i-wish-i-knew/)
-   [Intermediate Rails: Understanding Models, Views and Controllers | BetterExplained](http://betterexplained.com/articles/intermediate-rails-understanding-models-views-and-controllers/)
-   [Getting Started with Rails — Ruby on Rails Guides](http://guides.rubyonrails.org/getting_started.html)
-   [The Rails Command Line — Ruby on Rails Guides](http://guides.rubyonrails.org/command_line.html)
-   [Rails Routing from the Outside In — Ruby on Rails Guides](http://guides.rubyonrails.org/routing.html)
-   [Action Controller Overview — Ruby on Rails Guides](http://guides.rubyonrails.org/action_controller_overview.html)

## Define Model Responsiblities

In your own words, define what the responsibilities of the model layer are in
Rails.

```md
what helps to store information and does the processing. I like
how it kind of gave an office model, and gave a model as the guy in the back who actually has to get the dirty work done. Kind of like the read, write, of and to the database.
```

## Define Controller Responsiblities

In your own words, define what the responsibilities of the controller layer are
in Rails.

```md
Makes everything work. Like a higher up manager, it sees something a client wants, and orders people to get it done without really micromanaging the details of how it happens. It just gets told and is expected to be done.
```

## Define Router Responsiblities

In your own words, define what the router does in Rails.

```md
When given a url, it decides whether to get, patch, post, or delete and works with the controller in order to process a url request properly.
```

## The Request-Response Cycle in Rails

Starting with a client making a GET request to a particular URL, describe how
the parts of Rails interact to produce and send a response.

```md
a server receives the GET request, which gets sent to the controller. The controller is what then sees it as  a get request, gives it to the model which gets the URL requested from the database, and the view puts what the controller was given to display the HTML, and finally the HTML requested is given to the server again from the controller. And then the server gives that to the user, and hopefully the user will see what they requested or else there will be an error in the HTTP if say it's not there.
```
