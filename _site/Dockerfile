# # Base image: Ruby with necessary dependencies for Jekyll
# FROM ruby:3.2

# # Install dependencies
# RUN apt-get update && apt-get install -y \
#     build-essential \
#     nodejs \
#     && rm -rf /var/lib/apt/lists/*

# # Set the working directory inside the container
# WORKDIR /usr/src/app

# # Copy Gemfile into the container (necessary for `bundle install`)
# COPY Gemfile ./

# # Install bundler and dependencies
# RUN gem install bundler:2.3.26 && bundle install

# # Command to serve the Jekyll site
# CMD ["jekyll", "serve", "-H", "0.0.0.0", "-w", "--config", "_config.yml,_config_docker.yml"]

FROM ruby:2.7

# 安装依赖
RUN apt-get update && apt-get install -y \
  build-essential \
  nodejs \
  && rm -rf /var/lib/apt/lists/*

WORKDIR /usr/src/app

COPY Gemfile* ./

RUN gem install bundler -v 2.2.19 && bundle _2.2.19_ install

COPY . .

EXPOSE 4000

CMD ["bundle", "exec", "jekyll", "serve", "--host", "0.0.0.0", "--watch", "--force_polling"]


