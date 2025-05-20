# Base image
FROM node:16-alpine

# Set working directory
WORKDIR /app

# Copy package files and install dependencies
COPY package*.json ./
RUN npm install --production

# Copy application code
COPY . .

# Expose application port
EXPOSE 3000

# Start the application
CMD ["node", "server.js"]
