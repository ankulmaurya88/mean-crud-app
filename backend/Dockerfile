# Use official Node.js LTS image
FROM node:18

# Set working directory
WORKDIR /app

# Copy package.json and package-lock.json
COPY package*.json ./

# Install dependencies
RUN npm install --production

# Copy backend code
COPY . .

# Expose the port your server runs on
EXPOSE 8080

# Start the server
CMD ["node", "server.js"]