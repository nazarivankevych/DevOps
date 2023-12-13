# Pull image node for running a server
FROM node:14
# Set up a working directory for files in image
WORKDIR /app
# Make a new layer for reloading changes
COPY package.json /app
# The command which need to run after coping
RUN npm install
# Copy files from your folder into an image container with the path which set up as WORKING before
COPY . /app
# Set up a port which to use for running a service
EXPOSE 80
# Run a multiple tasks inside of the container
CMD [ "node", "server.js" ]
