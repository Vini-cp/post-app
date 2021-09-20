# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...

### Creating a database table with a migration

The command to generate a table expects two key arguments:

1. the name of the migration: the name actually tells rails what kind of migration it is going to be.

2. a list of the columns in the table. In this list of column arguments, the name of each column is followed by the type of the column.

``` shell
 bin/rails generate migration CreatePost title:string body:text
 ```

### Creating a model

We can create the Ruby model and its migrations at the same time with:

``` shell
bin/rails generate model Post title:string body:text
```

### Run migrations

``` shell
bin/rails db:migrate
```