FROM node:16.18.1-bullseye-slim

RUN apt update && apt install -y cowsay

WORKDIR /usr/src/app
COPY package.json ./
COPY package-lock.json ./
RUN npm install

COPY . .

USER node

EXPOSE 3000
CMD ["node", "src/index.js"]