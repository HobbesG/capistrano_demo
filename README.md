# README

# Installing Capistrano

> gem install capistrano

# To add capistrano and capistrano-rails support, in Gemfile add

'''ruby
group :development do
  gem "capistrano", "~> 3.10", require: false
  gem "capistrano-rails", "~> 1.3", require: false
end
'''

Then run bundle install

# Capifying your project

run in the root of your project

>bundle exec cap install

This will initialize your project with two stages, staging and production

'''
├── Capfile
├── config
│   ├── deploy
│   │   ├── production.rb
│   │   └── staging.rb
│   └── deploy.rb
└── lib
    └── capistrano
            └── tasks
'''

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
