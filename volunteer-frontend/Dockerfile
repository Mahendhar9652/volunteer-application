# Use an official Node.js runtime as a parent image
FROM node:21-alpine

# Set the working directory to /app
WORKDIR /app

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install app dependencies
RUN npm install

# Copy the current directory contents to the container at /app
COPY . .

# Make port 3000 available to the world outside this container
EXPOSE 3000


# Run npm start when the container launches
CMD ["npm", "start"]
