FROM ruby:latest
RUN apt-get update -y && \
    apt-get install -y build-essential libpq-dev nodejs sqlite3

MAINTAINER lmkhwana <lmkhwana@student.wethinkcode.co.za>

ONBUILD COPY app /opt/app
ONBUILD WORKDIR /opt/app

ONBUILD EXPOSE 3000
ONBUILD RUN bundle install