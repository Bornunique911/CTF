FROM node:18.12-buster-slim

RUN mkdir -p /app

WORKDIR /app

COPY package.json .

RUN yarn

COPY . .

USER node

CMD ["node", "index.js"]
