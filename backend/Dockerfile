FROM node:16-alpine
WORKDIR /app
COPY package*.json ./
RUN npm install
COPY . .
WORKDIR /app/src
EXPOSE 5000
CMD ["node", "app.js"]
