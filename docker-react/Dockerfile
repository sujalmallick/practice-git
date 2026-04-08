FROM node:22-alpine  
#Use the official Node.js 22 image based on Alpine Linux . alpine means light weight versions

WORKDIR /app
# Set the working directory inside the container to /app

COPY package*.json ./

# Copy the package.json file from the current directory to the /app directory in the container

RUN npm install

COPY . .
# Copy the rest of the application code to the /app directory in the container

EXPOSE 5173

CMD ["npm", "run", "dev"]