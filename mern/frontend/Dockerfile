# Basically this file has instructions to build a docker-image of our application. 

# Use an official NodeJS runtime as the base image
FROM node:18.9.1

# Set the working directory in the container
WORKDIR /app 

# Copy the file into the container
COPY package.json .

# Install dependencies (NodeModules in our case)
RUN npm install 

# Expose port 5173 for the Vite React app
EXPOSE 5173

# Copy the rest of your app's source code from your host to your image filesystem
COPY . . 

# Run the application when the container starts
CMD ["npm", "run", "dev"] 