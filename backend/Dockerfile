# Step 1: Use a base image
FROM node:20-alpine

# Step 2: Set the working directory in the container
WORKDIR /src

# Step 3: Copy files into the container
COPY package*.json ./

COPY tsconfig.json ./


COPY tailwind.config.js ./

# Step 4: Install dependencies
RUN npm install

# Step 5: Copy the rest of the project files
COPY . .

# Step 6: Expose the port the app runs on
EXPOSE 9000

# Step 7: Define the command to run the app
CMD ["npm", "run", "dev"]