# Rails Textbook 

## Introduction
Expanded Rails Headline.<br/>
More headings added to clarify, expand and help understand Ruby on Rails textbook.

## Heading \#1 : Ruby on Rails 

### Ruby on Rails

#### What is Rails?
 * Rails Overview
 * The benefits of using Rails

#### Generating rails app
 * Create your first Ruby on Rails Web Application
 * Create and Configure GitHub Account
 * Install Rails, Yarn
 * Important Rails Commands
    * Rails new \[project_name\] : 
      >Creates a new Rails applications in subdirectory \[project_name\] 
    * Rails server :
      >tarts up a Web server on port 3000 running the current application; log messages from the        server will appear on standard output.
    * rails generate scaffold name attribute:type
      >The scaffold command magically generates all the common things needed for a new resource for you! This includes controllers, models and views. It also creates the following basic actions: create a new resource, edit a resource, show a resource, and delete a resource.
    * rake db:migrate
      >When you add a new migration, for example by creating a new scaffold, the migration has to be applied to your database. The command is used to update your database.
    * bundle install
      >If you just added a new gem to your Gemfile you should run bundle install to install it. Don't forget to restart your server afterwards!
    * rake routes
      >Shows complete list of available routes in your application.
 * Create the Application
 * Scaffolding
 * Start Up Your App
 * Initialize Git and Push to GitHub

#### What is MVC(Model View Controller)
 * Modal View Controller Overview

#### Understanding Views
 * Layouts
 * Preprocessors
 * View Partials

#### Understanding Controllers
 * Naming Convetions
 * Rendering and Redirecting
 * Params and Strong Parameters

#### Understanding Routes
 * RESTful Routes
 * Non-RESTful Routes

#### Connecting rail's app with database
 * Active Record Basics
 * Rails Models
 * Migrations
 * Basic Validations and  Associations

#### Authentication in rails
 * Forms and Validations
 * Cookies , Sessions and Flashes
 * Basic and Digest Authentication
 * Devise

#### Rails app deployment
 * Create and Configure Heroku Account
 * Create a Heroku Application
 * Configure the Gemfile and Install new Gems
 * Add Changes to Git
 * Push and Migrate the database to Heroku

### Goal of this text
 1. The benefits of using Rails  
 2. Learning Why is it important what you name your models, controllers, and views?
 3. Knowing What’s the difference between a “view template” and a “layout”?
 4. Learning Why is Active Record more useful than just using SQL?
 5. Learning How can you view what was submitted by a form?
 6. Knowing What is a CSRF Token and why is it necessary?
 7. Knowing What’s the difference between authentication and authorization?

