# Use official Node.js image as the base image
FROM node:18

# Set the working directory inside the container
WORKDIR /app

# Copy package.json and install dependencies first
COPY package.json package-lock.json ./
RUN npm install

# Copy the entire project
COPY . .

# Expose port 3000 for the React development server
EXPOSE 3000

# Start the React app
CMD ["npm", "start"]

