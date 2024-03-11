source "https://rubygems.org"
git_source(:github) { |repo| "https://github.com/#{repo}.git" }

ruby "3.0.6"

# Bundle edge Rails instead: gem "rails", github: "rails/rails", branch: "main"
gem "rails", "~> 7.0.8", ">= 7.0.8.1"

# The original asset pipeline for Rails [https://github.com/rails/sprockets-rails]
gem "sprockets-rails"

# Use sqlite3 as the database for Active Record
gem "pg", "~> 1.1"

# Use the Puma web server [https://github.com/puma/puma]
gem "puma", "~> 5.0"

# Use JavaScript with ESM import maps [https://github.com/rails/importmap-rails]
gem "importmap-rails"

# Hotwire's SPA-like page accelerator [https://turbo.hotwired.dev]
gem "turbo-rails"

# Hotwire's modest JavaScript framework [https://stimulus.hotwired.dev]
gem "stimulus-rails"

# Build JSON APIs with ease [https://github.com/rails/jbuilder]
gem "jbuilder"

# Windows does not include zoneinfo files, so bundle the tzinfo-data gem
gem "tzinfo-data", platforms: %i[ mingw mswin x64_mingw jruby ]

# Reduces boot times through caching; required in config/boot.rb
gem "bootsnap", require: false

# Use Sass to process CSS
# gem "sassc-rails"

# Use Active Storage variants [https://guides.rubyonrails.org/active_storage_overview.html#transforming-images]
gem "image_processing", "~> 1.2"
gem 'active_storage-postgresql'

# CMS
gem "camaleon_cms"
gem 'camaleon_ecommerce', github:  'owen2345/camaleon-ecommerce'
gem 'draper'

group :development do
  gem "web-console"
  gem "letter_opener"

  gem 'bcrypt_pbkdf', '>= 1.0', '< 2.0'
  gem 'ed25519', '>= 1.2', '< 2.0'

  gem 'capistrano', '~> 3.17.1', require: false
  gem 'capistrano-db-tasks', require: false
  gem 'capistrano-nvm', require: false
  gem 'capistrano-rails'
  gem 'capistrano-passenger'
  gem 'capistrano-rbenv'
end
gem 'capistrano-rails-collection'

#################### Camaleon CMS include all gems for plugins and themes #################### 
require_relative './lib/plugin_routes' 
instance_eval(PluginRoutes.draw_gems)