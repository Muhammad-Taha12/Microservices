<<<<<<< HEAD
FROM node:18-alpine

WORKDIR /usr/src/app

COPY package*.json ./
RUN npm install --production

COPY . .

EXPOSE 5000

CMD ["node", "server.js"]
=======
# Use Node.js as base image
FROM node:18
# Giving some errors related to bcrypt when use node:18-alpine
# Set working directory
WORKDIR /app

# Copy package.json and package-lock.json
COPY package.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application files
COPY . .

# Expose port
EXPOSE 5000

# Start the application
CMD ["node", "server.js"]
>>>>>>> 3cce4fb98539634bdc6dee815ec04540bc426c77
