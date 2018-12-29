---
layout: post
title:      "Starting a Sinatra App"
date:       2018-12-29 22:29:37 +0000
permalink:  starting_a_sinatra_app
---


The beginning of the Sinatra section helped me further understand the web flow - how requests are received from a browser and the way data is sent back to be rendered in the browser instantly. There are a lot of aspects of this flow that come together to make this happen. In the section, I've learned a good order for myself to adopt when building my app and test it. This order is as follows:


#### Step 1 - Create folders and files that are needed for the app

* Nested in the `app` directory - create `models`, `views`, and `controllers` directories

* `models` directory contains all the `model` classes you are creating for the app *(ie. artist.rb)*

* `views` directory contains all the files that use HTML for the app's user interfaces *(ie. index.erb, edit.erb)*

* `controllers` directory contains all the controller files that have various routes that user can visit & executes an action

* `config` directory with `environment` file that requires all app files and establishes `ActiveRecord::Base` connection

* `config.ru` file mounts the controllers, and requires `environment` file

* `Gemfile` contains all the gems that will be used throughout the app

* `Rakefile` contains rake tasks and requires `environment` file + rake

* `Spec` directory includes all the rspec test files - *not a requirement*

* Create dabatase `db` directory for the migrations - execute migrations in terminal: `rake db:create_migration` 


#### Step 2 - Map out your models and their associations

* Make sure to plan the `models` you intend to use and their relationships with each other

* Determine which columns you will need for your tables before executing `rake db:migrate` *(you can always add more later)*


#### Step 3 - Setup Database

* Use ActiveRecord + SQLite3 to persist data

* Establish connection to database in your `environment.rb`
```
ActiveRecord::Base.establish_connection(
  :adapter => "sqlite3",
  :database => "db/#{ENV['SINATRA_ENV']}.sqlite") 
```
 
* Create table migrations in the `db` files

* Create sample objects in `seeds.rb` file in `db` folder to test

* Go into `tux` and test that you are able to persist data and create objects + more


#### Step Last 
**Add all the many remaining files and be fine with looking back at your labs for help.**





**One tip:** Do not fall too deep into the rabbit hole. It is very easy to want to add more functionality than there is on the specifications which is great (go, you!) but know where to draw the line.



