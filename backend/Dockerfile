# Base image
FROM node:18-alpine

# Create app directory
WORKDIR /usr/src/app

# Bundle app source
COPY . /usr/src/app

# Install app dependencies
RUN npm install

# Creates a "dist" folder with the production build
RUN npm run build

# Start the server using the production build
CMD ["npm", "run", "start:prod"]