FROM ruby:2.5
RUN mkdir /myapp
WORKDIR /myapp
COPY Gemfile /myapp/Gemfile
RUN bundle install
COPY test.rb /myapp

# Start the main process.
CMD ["ruby", "/myapp/test.rb"]