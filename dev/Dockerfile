FROM ruby:2.3.3-slim

RUN apt update && \
  apt install -y \
    sqlite3 libsqlite3-dev \
    nodejs \
    npm && \
  rm -rf /var/lib/apt/lists/*

RUN gem install bundler

WORKDIR /app
VOLUME /app

EXPOSE 3000
