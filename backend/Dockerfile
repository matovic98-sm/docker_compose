
# Use Node.js 18 Alpine as the base image
FROM node:18-alpine

# Set the working directory inside the container
WORKDIR /app

# Copy package files
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the application files
COPY . .

# Create a directory for the SQLite database
RUN mkdir -p /app/data

# Expose the backend port
EXPOSE 5000

# Start the backend application
CMD ["npm", "start"]
