FROM ruby:2.6.5

RUN apt-get update && apt-get install -y \
  build-essential \
  libpq-dev \
  nodejs \
  default-mysql-client \
  yarn

WORKDIR /rails-app

COPY Gemfile Gemfile.lock /rails-app/

RUN bundle install