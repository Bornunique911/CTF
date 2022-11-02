FROM node:19.0-buster-slim
WORKDIR /app
COPY package*.json ./
COPY index.js ./
RUN npm install
CMD ["node", "index.js"]
