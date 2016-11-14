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
Models are in charge of dealing with data. They communicate with the database
and pass off their information to the controller.

resources used:
http://betterexplained.com/articles/intermediate-rails-understanding-models-views-and-controllers/
http://betterexplained.com/articles/starting-ruby-on-rails-what-i-wish-i-knew/
```

## Define Controller Responsiblities

In your own words, define what the responsibilities of the controller layer are
in Rails.

```md
Controllers are the go-betweens which transfer information back and forth between
the aspects of the application which the user touches and the model. The
controller interprets the information, coming from either side, and processes it
in a way that makes it accessable to either the user or the model.

resources used:
http://guides.rubyonrails.org/action_controller_overview.html
http://guides.rubyonrails.org/routing.html
http://betterexplained.com/articles/intermediate-rails-understanding-models-views-and-controllers/
http://betterexplained.com/articles/starting-ruby-on-rails-what-i-wish-i-knew/
```

## Define Router Responsiblities

In your own words, define what the router does in Rails.

```md
Routers are in charge of matching incoming HTTP requests with specific
controller actions.They also sometimes create file paths and URLs.

resources used:
http://guides.rubyonrails.org/routing.html
http://betterexplained.com/articles/intermediate-rails-understanding-models-views-and-controllers/
http://betterexplained.com/articles/starting-ruby-on-rails-what-i-wish-i-knew/
```

## The Request-Response Cycle in Rails

Starting with a client making a GET request to a particular URL, describe how
the parts of Rails interact to produce and send a response.

```md
1.) The client sends a GET request to a URL.
2.) The router recieves the GET request and matches it with a Controller and
constroller action.
3.) The controller uses its action(s)/ methods to process the information so
that the request is in a format that the model can understand.
4.) The controller requests specific information from the Model.
5.) The Model interacts with the database to retreive the requested information.
6.) The Model passes the requested information to the controller.
7.) The Controller processes the information from the model and makes it useable
for the client.
8.) The Client recieves the information that was requested.

resources used:
http://guides.rubyonrails.org/action_controller_overview.html
http://guides.rubyonrails.org/routing.html
http://betterexplained.com/articles/intermediate-rails-understanding-models-views-and-controllers/
http://betterexplained.com/articles/starting-ruby-on-rails-what-i-wish-i-knew/
```
