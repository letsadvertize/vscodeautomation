# Use Node.js 20 as the base image
FROM node:20

# Set the working directory to /app
WORKDIR /app

# Copy the package.json and package-lock.json
COPY package.json package-lock.json ./

# Install dependencies
RUN npm install

# Copy the rest of the frontend application files
COPY . .

# Expose port 3000
EXPOSE 3000

# Set the default command to run the Next.js application
CMD ["npm", "run", "dev"]
