FROM node:4-onbuild

# Author
MAINTAINER Alexander Nguyen

# Set app directory
RUN mkdir -p /app
WORKDIR /app

# Install dependencies
ADD package.json /app/package.json
RUN npm install

# Bundle app source
ADD . /app

# Expose port
ENV PORT 8080
EXPOSE 8080

# Start app
# CMD npm run dev -s
CMD npm run prod -s
