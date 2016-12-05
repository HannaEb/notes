$ rails new
$ bundle install
$ rails server

# MVC
=> model, view, controller
Keeping your model, view and controller code isolated ensures that you can change one part without the rest. It keeps the code clean, makes it semantic and easy to understand, and makes it break less.

Models refer to the 'nouns' of the app - the things it deals with and their details.

Controllers contain the 'verbs' - what we can do to the 'nouns' and how they can be interacted with.

Views are used ot actually show your users something.

# ORM
=> object-relational mapping
A way of getting your web app talking to a database. E.g. DataMapper in Sinatra, Active Record in Rails.


Active Record is a peice of software that interprets Ruby commands and turns them into SQL queries.

The active record pattern is an architectural design pattern for software that works with databases. In this pattern, each database table becomes a class, and in instance of that class refers to a specific row within that table.

Migrations describe a set of changes you are making to your database - Rake can interpret them and run the actual SQL commands that make those changes happen. If something goes wrong, you can roll your database back to a previous state by using those migration files as they provide a record of every change to your data.

params[:example] passes in all the params received from a submitted form even if the form has been modified by a user. We therefore have to explicitly state which params we are going to allow our controller to accept, using 'permit'.

Devise is an authentication system that allows users to sign up, login, reset their passwords etc.
=> devise gem

Onmiauth allows a user to log into your site using a 3rd party login. 
