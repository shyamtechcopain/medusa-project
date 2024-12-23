FROM node:20-alpine
WORKDIR /medusa
COPY package*.json ./
RUN npm install
COPY . .
EXPOSE 8000
CMD ["npm", "run", "start"]
