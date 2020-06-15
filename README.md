# README

This README would normally document whatever steps are necessary to get the
application up and running.

First time to run:

docker-compose build
docker-compose run --rm web bundle exec rails g spree:install --user_class=Spree::User
docker-compose run --rm web bundle exec rails g spree:auth:install
docker-compose run --rm web bundle exec rails g spree_gateway:install
docker-compose up

Later on:

docker-compose build
docker-compose up

Clean all docker file:

docker system prune -a --volumes