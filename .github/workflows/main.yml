# Use the official Node.js 20 LTS image
FROM node:20

# Set working directory
WORKDIR /app

# Copy package.json and package-lock.json first for caching
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the project files
COPY . .

# Expose the port (change if your app uses a different one)
EXPOSE 3000

# Start the application
CMD ["npm", "start"]
