# Active Record Code Challenge: Product Review

In this project, we're going to build an e-commerce domain that focuses on product reviews. We'll be working with three main models: User, Review, and Product. This project includes Active Record Migrations, Active Record Associations, Class and Instance Methods, and Active Record Querying.

## Getting Started.
 To get started, follow these instructions:

1. Clone this repository

2. Run bundle install to install all necessary gems

3. Create a SQLite3 database by running sqlite3 reviews.db

4. Run migrations using rake db:migrate to run the migrations and create the database schema

5. Run rake db:seed to seed the database with sample data

## Usage To use the application, run the following command to start a console session:

ruby app.rb

From there, you can test the various methods defined in the models. Here are some examples:

## To get all the reviews for a product:

product = Product.first reviews = product.reviews To get all the users who reviewed a product:

product = Product.first users = product.users To get all the reviews for a user:

user = User.first reviews = user.reviews To get all the products that a user reviewed:

user = User.first products = user.products To leave a review for a product:

product = Product.first user = User.first review = Review.create(rating: 4, description: "Great product!", user_id: user.id, product_id: product.id) To find the average rating for a product:

product = Product.first average_rating = product.average_rating 

## License 

This project is licensed under the MIT License - see the LICENSE.md file for details.