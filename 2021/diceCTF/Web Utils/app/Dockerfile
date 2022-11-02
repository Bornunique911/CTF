FROM node:19.0-buster-slim AS build

WORKDIR /app

RUN apt-get update && \
    apt-get install -y --no-install-recommends \
    build-essential python && \
    rm -rf /var/lib/apt/lists/*

COPY package.json /app/

RUN yarn

COPY . .

FROM node:19.0-buster-slim

WORKDIR /app

ENV NODE_ENV production

COPY --from=build /app /app

EXPOSE 3000

CMD ["node", "/app/index.js"]
