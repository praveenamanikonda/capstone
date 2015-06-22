## Capstone: A social micro blogging site.  
Made with my mentor at [Bolc] (http://bloc.io).

About Capstone: This app allows users to create password-secured accounts, login/logout , User Authorization i.e ability to create/edit/delete Topics , posts , comment on posts, Vote i.e like/unlike posts, ranks posts,Favoriting posts , data validations, upload images, follow/unfollow users.

This README would normally document whatever steps are necessary to get the
application up and running.

Ruby Version : rails 4.1.0

To view the app:
  start Rails server : rails s 
  Visit 'https://localhost:3000/'
  
To check app's available routes : rake routes 

Database creation : The development and production environments have different databases. Update your gem file such that it has the following:
  group :production do 
    gem 'pg'
    gem 'rails_12factor'
  end 

  group :development do 
    gem 'sqlite3'
  end 
  
  group :development, :test do
    gem 'byebug'
    gem 'web-console', '~> 2.0.0.beta2'
    gem 'spring', '1.1.3'
  end
  
Configuring production : 
  To configure email functionality for this app , you need to addon 'Sendgrid' on production. 
  Command for configuring : 
    heroku addons:create sendgrid:starter
    
Gems required for this app: 
 gem 'bcrypt', '3.1.7'
gem 'faker', '1.4.2'
gem 'mini_magick', '3.8.0'
gem 'fog', '1.23.0'
gem 'figaro'
gem 'will_paginate', '3.0.7'
gem 'bootstrap-will_paginate', '0.0.10'
gem 'bootstrap-sass', '~> 3.1.1'
gem 'carrierwave', '0.10.0'
gem 'cloudinary'
 
