FROM ruby:2.6


RUN apt-get update -yqq
RUN apt-get install -yqq --no-install-recommends nodejs

COPY . /usr/src/app

WORKDIR /usr/src/app
RUN gem install bundler
RUN bundle install

CMD ["rails", "server", "-b", "0.0.0.0"]