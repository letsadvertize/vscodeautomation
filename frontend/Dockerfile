# Use a compatible Node.js version for Next.js
FROM node:20

# Set the working directory
WORKDIR /app

# Copy package.json and package-lock.json first
COPY package.json package-lock.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application
COPY . .

# Build the Next.js app
RUN npm run build

# Expose the port where the Next.js app will run
EXPOSE 3000

# Start the Next.js app
CMD ["npm", "start"]
