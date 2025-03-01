# Use Node.js as base image
FROM node:20

# Set working directory in container
WORKDIR /app

# Copy package.json and package-lock.json into container
COPY frontend/package.json frontend/package-lock.json ./

# Install dependencies
RUN npm install

# Copy all frontend files
COPY frontend/ .

# Expose port 3000
EXPOSE 3000

# Run the frontend
CMD ["npm", "start"]
