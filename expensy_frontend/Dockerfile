# Use official Node.js image to build the frontend
FROM node:18 as build

# Set the working directory for the frontend build process
WORKDIR /app

# Copy package.json and install dependencies
COPY package*.json ./
RUN npm install

# Copy the rest of the frontend code
COPY . .

# Build the React application
RUN npm run build

# Expose port 80 for the app server
EXPOSE 3000

# Run the app
CMD ["npm", "start"]
