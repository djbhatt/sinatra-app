# Start from a small base
FROM alpine/bundle

# Add our application binary
ADD app /app

# Change WorkDir
WORKDIR /app

# Run command to build package
RUN bundle install

# Run our application!
CMD [ "bundle","exec","rackup","-o","0.0.0.0" ]

# Our application runs on port 9292
# so allow hosts to bind to that port
EXPOSE 9292
