# Specify a base image
FROM node:alpine  

# Create a directory to store all local files so that you don't overwrite
# files/folders inside of the base image.
WORKDIR /usr/app

# Copy local directory into docker base directory. In order to not rebuild the container
# with all dependencies, copy only the package.json/dependency file. (requirements.txt, piplock)
COPY ./package.json ./

# Install some dependencies
RUN npm install

# Default command
CMD ["npm", "start"]