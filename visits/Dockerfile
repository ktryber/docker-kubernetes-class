# Get a base image, alpine is the minimalist version of an image
FROM node:alpine

# Create a working directory inside of the container
WORKDIR '/app'

# Copy the dependencies over to be installed
COPY package.json .

# Install dependencies into the container
RUN npm install

# Copy all local files in working directory into the WORKDIR
COPY . .


# Run the server, this is a command specified in the package.json
CMD ["npm", "start"]