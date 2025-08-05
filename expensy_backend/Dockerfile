# Use the official Node.js image as a base
FROM node:19

# Set the working directory in the container
WORKDIR /app

# Copy package.json and install dependencies
COPY package*.json ./
RUN npm install

# Copy the rest of your application code
COPY . .

# Expose the port your application runs on
EXPOSE 5000

# Command to run your app
CMD ["npm", "run", "start"]