FROM node:20-alpine

# Set working directory
WORKDIR /app

# Copy package files and install dependencies
COPY package.json package-lock.json . 
RUN npm install

# Copy the rest of the app
COPY . .

# Expose the required port
EXPOSE 4000

# Run the app in development mode
CMD ["npm", "run", "dev"]
