FROM node:boron

MAINTAINER Ivan Font <ifont@redhat.com>

# Create app directory
RUN mkdir -p /tmp/src/app
WORKDIR /tmp/src/app

# Clone game source code
RUN git clone https://github.com/tgubeli/pacman.git .

# Install app dependencies
RUN npm install

# Expose port 8080
EXPOSE 8080

# Run container
CMD ["npm", "start"]
