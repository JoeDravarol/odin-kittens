# Odin-kittens

This project is an introduction to APIs in Rails. It's a simple project where you can create a kitten with: name, age, cuteness, softness attributes. The Rest action can render as HTML or JSON format.

## To run this app locally

1. Fork this repository on Github.
1. Clone your forked repository onto your local computer.
1. Use cd `odin-kittens` to move into the project folder.
1. Run `bundle install` to get required gems.
1. Run `rails db:migrate` to setup the database.
1. Run `rails server` to start the server.
1. In your browser, navigate to [http://localhost:3000](http://localhost:3000)

## To Interface with the API (Command-line)

* Disclamer: You can only interface with the index and show action.

1. In your command line, run `irb`
1. Once in irb, type `require 'rest'client`.
1. To make a get request to the index action type `response = RestClient.get('http://localhost:3000/kittens', accept: :json)`
1. To view the response body type `puts reponse.body`

## Development versions

* Ruby 2.6.1
* Rails 5.2.3

## Acknowledgement

Created as part of the Odin Project's [curriculum](https://www.theodinproject.com/courses/ruby-on-rails/lessons/apis?ref=lnav#project-1-building-a-simple-kittens-api)